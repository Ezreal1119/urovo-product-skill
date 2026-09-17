# SCHEMA.md — Product Knowledge Vault Schema

This file defines the wiki structure, conventions, and workflows for the UROVO Product Knowledge Base.

## Directory Structure

```
product-knowledge-vault/
├── SCHEMA.md          — this schema
├── index.md           — master catalog of all pages
├── log.md             — chronological operation log (append-only)
├── overview.md        — high-level synthesis of the entire product portfolio
├── synthesis.md       — key patterns, insights, and cross-product observations
├── products/          — exhaustive source Hub for each canonical product
├── shared/            — graph nodes for multi-product source documents
├── spec/              — one specification page per product
├── pb/                — one brochure/marketing page per product
├── categories/        — product category overview pages
├── comparisons/       — comparative analysis across products
├── features/          — cross-cutting feature dimension pages
├── matrices/          — quantitative comparison matrices
├── technology/        — technology-specific deep-dive pages
└── entity/            — entity pages for key components (chipsets, scan engines, etc.)
```

The official source corpus lives beside the Vault in canonical product type parents:

```text
<ProductName>/
├── brochure/<document-key>_<YYYYMMDDHHmm>/
├── specs/<document-key>_<YYYYMMDDHHmm>/
├── user_guide/<document-key>_<YYYYMMDDHHmm>/
├── presentation/<document-key>_<YYYYMMDDHHmm>/
├── accessories/<document-key>_<YYYYMMDDHHmm>/
└── others/<document-key>_<YYYYMMDDHHmm>/

_shared/<semantic-type>/<document-key>_<YYYYMMDDHHmm>/
```

Only the six canonical parents may appear directly under a product. `brochure`, `specs`, `user_guide`, `presentation`, and `accessories` each contain at most one current document directory; `others` may contain multiple distinct documents. A normal document directory has exactly one unchanged original plus one same-stem, semantically lossless Markdown companion. A standalone Markdown explicitly identified by the user as personally authored or approved canonical knowledge instead forms a one-file source slot; the unchanged Markdown is both the source and retrieval form. Multi-product sources always use `_shared/`. The fixed timestamp `202601010000` marks the historical migration baseline. Unsynchronized inbox files are not knowledge sources. Do not store extracted page images.

## Page Naming Conventions

- Product source Hubs: `products/<ProductName>.md`
- Product summary pages: `spec/<ProductName>.md`, `pb/<ProductName>.md`
- Shared source nodes: `shared/<document-key>.md`
- Category pages: `categories/<category-name>.md`
- Comparison pages: `comparisons/<group-name>-comparison.md`
- Feature pages: `features/<feature-name>.md`
- Technology pages: `technology/<tech-name>.md`
- Entity pages: `entity/<entity-name>.md`

## Page Content Standards

### Product Source Hubs (products/)

Every canonical product has one Hub. It is the mandatory Query entry and must contain:

- an exhaustive `Current Source Coverage` row for every current product source directory;
- links to the product's spec, PB, category, and relevant shared pages;
- every unresolved local source discrepancy with field, conflicting values, exact paths, and status;
- the rule to search all product and linked shared Markdown when normal routing is insufficient.

Progressive disclosure may reduce what is loaded, but never what is discovered. A Hub is incomplete if any current product source is missing from its coverage table.

### Shared Source Nodes (shared/)

Create one Vault node per synchronized multi-product document. Record exact original/Markdown paths for a converted pair, or the exact canonical Markdown path and authored-source form for a user-approved one-file source. Link every covered product Hub, summarize supported facts faithfully, and record unresolved cross-source differences. Every covered product Hub must link back to the shared node.

### Product Spec Pages (spec/)

Format:

```markdown
# <Product Name> — <Type Tagline>

## Overview

[One-paragraph summary of the product's purpose and key positioning]

## Specifications

[Structured tables organized by: Performance → Physical → Display → Power → Data Capture → Connectivity → Durability → Accessories]

## Key Differentiators

[What makes this product unique in its category]

## Target Industries

[Industries this product serves]

## Related Products

[Links to comparison pages or sibling products]
```

### Product Brochure Pages (pb/)

Format:

```markdown
# <Product Name>

## Product Highlights

[Tagline bar with key stats]

## Key Features

[Feature sections with descriptive paragraphs]

## Specifications

[Essential specs table]

## Accessories

[Accessories list if applicable]

## Target Industries
```

### Category Pages

Format:

```markdown
# <Category Name>

## Overview

[What defines this category, typical use cases]

## Products in this Category

[Table with models, generations, key differences]

## Key Technologies

[Technologies prevalent in this category]

## Cross-Reference

[Links to comparison pages, feature pages]
```

## Operations

### Ingest

Routine ingestion is an explicit maintenance workflow governed by `../SYNC_PROMPT.md`:

1. The user places original documents in `../newly_added/` and explicitly requests sync.
2. The Agent classifies single-product versus multi-product scope, canonical type, document identity, language, region, and variant.
3. It semantically normalizes aliases such as user manual/operation manual to `user_guide`.
4. It replaces a current single-slot document only with strong same-lineage evidence; secondary documents go to `others`, while ambiguity stays in the inbox.
5. It creates and verifies either the new original/Markdown pair or the explicitly approved one-file canonical Markdown slot before deleting a replaced directory.
6. It updates every affected product Hub first, then only semantic Vault pages whose facts or links changed.
7. Multi-product inputs create/update a `shared/` node and backlinks from every covered product Hub.
8. Same-context factual differences become active Hub discrepancies instead of silent merges.
9. Provenance uses exact synchronized paths. The Agent validates links/coverage, appends to `log.md`, and removes only successful inbox inputs.

Routine sync does not require a manifest, custom sync script, full portfolio audit, or web pass. Ambiguous inputs remain in the inbox for user judgment.

### Query

- Read `index.md`, then the Hub for every target product.
- Enumerate every Hub source and linked shared node before choosing what to load.
- Route specs, operation, accessories, and positioning questions to their canonical source types; search `others` and `_shared` when needed.
- Read every relevant-type source; for broad or exhaustive requests, read every source in the Hub.
- Use comparison pages and matrices for fast context, then verify against source Markdown.
- Surface relevant active Hub discrepancies and any disagreement found in loaded sources.
- Do not claim information is unavailable until product and linked shared Markdown have been searched.
- Keep normal Q&A read-only. Update Vault pages only through an explicit maintenance request governed by `../SYNC_PROMPT.md`.

## Link Format

Use relative wiki links: `[[spec/CT48|CT48 Specification]]` or `[CT48](spec/CT48.md)`.

Wiki links must point to real markdown pages in `product-knowledge-vault/`. Use the actual filename, including hyphens and case:

- Correct: `[[spec/DT50P-Lite|DT50P Lite]]`
- Incorrect target text: `spec/DT50P Lite`

When a specific category page does not exist, link to the closest existing aggregate page instead of inventing a broken page. For example, enterprise tablets, wearables, RFID sleds, and price checkers currently link to `[[categories/other-devices|Other Devices]]`.

When a page identifies its official source, use the exact Skill-relative product path:

```markdown
> Source: i9100/specs/default_202601010000/i9100(EN)-SPEC-MB 20260130.pdf
```

## Frontmatter

Optional YAML frontmatter on key pages for metadata:

```yaml
---
category: handheld-terminal
generation: current
os: Android 12
rfid: HF/NFC
ip_rating: IP67
---
```
