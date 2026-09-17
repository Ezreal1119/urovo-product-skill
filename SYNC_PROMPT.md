# UROVO Product Document Sync

Use this file only when the user explicitly asks to sync the product knowledge package. Normal product Q&A is read-only and ignores `newly_added/`. Reply in the user's language.

## Goal

Process each input under `skills/urovo-product-expert/newly_added/`, preserve the canonical source, create or apply a semantically lossless Markdown companion when needed, update the exhaustive product source Hubs and affected Vault knowledge, and remove only successfully processed inbox inputs.

Do not use a manifest or custom sync script. Inspect the current files and content directly.

## Canonical source layout

Single-product sources use only these parents:

```text
<ProductName>/
├── brochure/
│   └── <document-key>_<YYYYMMDDHHmm>/
├── specs/
│   └── <document-key>_<YYYYMMDDHHmm>/
├── user_guide/
│   └── <document-key>_<YYYYMMDDHHmm>/
├── presentation/
│   └── <document-key>_<YYYYMMDDHHmm>/
├── accessories/
│   └── <document-key>_<YYYYMMDDHHmm>/
└── others/
    ├── <document-key>_<YYYYMMDDHHmm>/
    └── <another-key>_<YYYYMMDDHHmm>/
```

`brochure`, `specs`, `user_guide`, `presentation`, and `accessories` may each contain at most one current document directory. `others` may contain multiple distinct document directories.

Canonical identity override: route legacy 4G product-specific material identified by `SQ53S` or `SQ53ST` to the `DT50S` root and Product Hub, even when the retained source calls the market model `DT50`. Preserve the source filename and source-specific label. Do not fold `DT50 5G` (`SQ53B` / `SQ53BV`) into `DT50S`; it is a separate lineage.

Normal extracted documents contain exactly:

```text
<unchanged-original-file>
<same-stem>.md
```

When the user explicitly states that a standalone Markdown file is personally authored or approved as canonical knowledge, its document directory instead contains exactly that one unchanged `.md` file. That Markdown is both the canonical source and the retrieval form; do not create a duplicate companion. Do not apply this exception to an orphan conversion, temporary note, AI-generated summary, or unconfirmed Markdown merely because it has a `.md` extension.

Any source that substantively describes more than one canonical product goes under:

```text
_shared/<semantic-type>/<document-key>_<YYYYMMDDHHmm>/
```

Shared type parents may contain multiple distinct documents. The historical baseline timestamp is `202601010000`; new syncs use current Asia/Shanghai time as `YYYYMMDDHHmm`.

## Semantic type normalization

Classify by content, title, document code, and purpose—not extension alone:

| Input terms or purpose | Canonical type |
| --- | --- |
| spec, specification, datasheet, data sheet, technical sheet | `specs` |
| brochure, PB, leaflet, catalog, product brief | `brochure` |
| user manual, user guide, operation manual, instruction manual, quick start | `user_guide` |
| presentation, PPT, slide deck, sales deck | `presentation` |
| accessory list, accessory guide, compatible accessories | `accessories` |
| certificate, release note, FAQ, or any unmatched single-product material | `others` |

Use a short stable `document-key` describing identity, language, region, or variant when needed. Do not create a new top-level product type for a synonym.

## Classification and replacement

For every input:

1. Ignore `newly_added/README.md` and hidden files. Stop with a no-op report if there are no real inputs.
2. Determine whether the source is single-product or multi-product. Mentioning accessories or variants of one canonical product does not make it shared; substantively covering two or more canonical product directories does.
3. Determine canonical type, document identity, language, region/edition, product/configuration variant, document code, revision, and publication date when available.
4. Compute or compare file bytes. If byte-identical to an existing original, treat it as a duplicate and remove only the inbox copy.
5. Group all inbox candidates that map to the same document lineage before selecting a destination. If the batch contains multiple revisions, synchronize only the newest revision using explicit revision/date evidence and content changes; treat older candidates as superseded inbox copies. If their ordering remains ambiguous, leave the group in the inbox and ask the user.
6. Match document lineage using content and metadata, not filename alone. Strong replacement evidence includes the same document code/title/purpose/language/region/variant with a later revision, or substantially overlapping sections with updated facts.
7. Never infer replacement merely because two documents share a canonical type.
8. For the five single-slot types:
   - replace the existing slot only when the new input is clearly its newer version;
   - if the input is a legitimate secondary document of that broad type, place it under `others/` with a descriptive key;
   - if it is unclear which document should be primary, leave it in the inbox and ask the user.
9. For `others` and `_shared`, replace only the matching document identity. Otherwise add another document directory.
10. Classify standalone Markdown explicitly:
   - if the user states that it is personally authored or approves it as canonical knowledge, synchronize the unchanged Markdown directly as a one-file source slot;
   - if it is explicitly a correction to an existing companion, apply it only when the corrected facts are supported by the retained original, preserve the original, and do not create a new slot;
   - otherwise treat it as unconfirmed and leave it in the inbox until the user supplies the source original or explicitly adopts the Markdown as canonical.

## Add or replace safely

1. Create the new timestamped document directory first. If its name already exists, append `_02`, `_03`, and so on.
2. Copy or move the canonical source without changing its bytes or filename. For explicitly approved authored Markdown, keep the single file unchanged and skip companion generation.
3. For non-Markdown originals, create the same-stem Markdown with all extractable textual and numeric information preserved:
   - PDF/DOCX: preserve headings, paragraphs, tables, lists, footnotes, qualifiers, and page-relevant labels;
   - PPT/PPTX: preserve slide order, slide titles, body text, speaker notes, tables, labels, and meaningful chart data;
   - XLS/XLSX: preserve every non-empty sheet name, table, meaningful cell value, formula or note needed to interpret it, and units/qualifiers;
   - PNG/JPG/WebP and other standalone images: preserve all readable text, tables, labels, UI states, callouts, and the meaning of diagrams, screenshots, or product imagery;
   - preserve exact model names, values, options, certifications, and uncertainty;
   - never invent, silently correct, or enrich facts from memory;
   - do not generate extracted images or thumbnails merely to decorate the companion. The unchanged original preserves layout, while the Markdown must still make its visual evidence searchable and understandable.
4. Verify either the original/companion pair or the one-file authored Markdown slot. Verify important hard facts against all affected current sources.
5. Compare the new facts with the previous slot, affected product-specific sources, and relevant shared sources.
6. Only after verification succeeds, remove the replaced old directory. Git history is the archive.

## Mandatory visual-source protocol

Apply this protocol to standalone images, scanned or image-only PDF pages, image-dominant slides, screenshots, diagrams, charts, and any page whose text extraction is empty or materially incomplete.

1. Determine the page, slide, or image count before conversion. Inspect every item in order with a vision-capable tool at a legible resolution; a PDF text layer, Office XML extraction, filename, alt text, or surrounding caption does not prove that the visible image was read.
2. For mixed text-and-image documents, use normal extraction for the text layer and visual inspection for every image that carries product facts, labels, tables, UI states, workflow steps, compatibility, dimensions, ports, accessories, or other meaning.
3. In the same-stem Markdown, transcribe all legible visual text and numeric values, reconstruct tables and ordered steps, and briefly describe meaningful diagrams, screenshots, charts, and product callouts. Preserve page or slide order and identify the corresponding page/slide when it helps provenance.
4. Never use an image link, embedded-image reference, filename, placeholder, “see image/original,” or a generic statement such as “visual content omitted” as a substitute for recognition. Image references may appear only as supplemental provenance after the visible evidence has been transcribed.
5. Mark genuinely unreadable or ambiguous content explicitly with its page/slide/image location. Do not infer missing text or values from nearby products, prior knowledge, or filenames.
6. Before declaring success, compare the inspected item count with the original count and confirm that every visual item has either substantive Markdown coverage or an explicit unreadable marker. Spot-check hard facts against the rendered source, not only the extracted text.
7. If a vision-capable tool is unavailable, rendering fails, any item remains uninspected, or the coverage check fails, leave the original in `newly_added/`, make no canonical/Vault claims for it, and report the exact blocker. Do not remove the inbox input or announce a successful sync.

## Vault and graph maintenance

For every successful change:

1. Update each affected `product-knowledge-vault/products/<product>.md` Hub first:
   - make `Current Source Coverage` exactly match every current source directory for that product;
   - link relevant Vault spec/PB/category pages;
   - link every synchronized shared Vault node that covers the product.
2. For a multi-product source, create or update `product-knowledge-vault/shared/<document-key>.md` with:
   - the exact original and Markdown paths for a converted pair, or the exact canonical Markdown path and authored-source form for a one-file source;
   - wiki links to every covered product Hub;
   - a faithful summary and the facts used by Vault pages.
3. Update only affected semantic pages: `spec/`, `pb/`, categories, comparisons, matrices, features, overview, synthesis, or index.
4. Detect same-context factual differences such as BT 5.1 versus BT 5.2. First determine whether region, variant, optional configuration, or document date explains them.
5. If unresolved, add or update an `Active Local Source Discrepancies` table in every affected product Hub. Include field, both values, exact source paths, and status. Do not silently choose a winner.
6. When later evidence resolves a discrepancy, remove it or mark it resolved during that sync so Query does not surface stale warnings.
7. Append a concise entry to `product-knowledge-vault/log.md`.

## Validation

Before removing successful inbox inputs, verify all of the following:

- product roots contain only `brochure`, `specs`, `user_guide`, `presentation`, `accessories`, and `others`;
- each of the five single-slot parents contains at most one document directory;
- every document directory contains either exactly one original plus one same-stem Markdown companion, or one explicitly approved authored canonical Markdown file;
- every standalone image and every visually meaningful page or slide has substantive Markdown transcription or an explicit location-specific unreadable marker; bare image references and placeholders fail validation;
- the verified page/slide/image coverage count matches the original source;
- every current single-product source appears exactly once in its product Hub;
- every shared source has a `shared/` Vault node and backlinks from all covered product Hubs;
- edited Wiki links and provenance paths resolve;
- active discrepancy records match current sources;
- no unrelated product, source, or Workspace output changed.

Leave ambiguous or failed inputs in `newly_added/`. Do not create commits, tags, or pushes unless explicitly requested.

## Final response

Report added/replaced/corrected documents, classification decisions, removed old slots, Vault/Hub pages changed, active discrepancies, unresolved inbox files, and validation results.
