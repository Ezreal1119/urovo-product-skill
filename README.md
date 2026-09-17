# UROVO Product Documents

This package contains official UROVO product documents, faithful Markdown companions, and the Obsidian-compatible `product-knowledge-vault/` used by the product expert.

## Normal use

Normal product Q&A is read-only. The Agent starts from `product-knowledge-vault/index.md`, reads every target product Hub to discover the complete source set, then loads only the relevant source types. Files waiting in `newly_added/` are never authoritative.

## Source structure

Each product uses only six canonical type parents:

```text
<ProductName>/
├── brochure/<document-key>_<timestamp>/
├── specs/<document-key>_<timestamp>/
├── user_guide/<document-key>_<timestamp>/
├── presentation/<document-key>_<timestamp>/
├── accessories/<document-key>_<timestamp>/
└── others/<document-key>_<timestamp>/

_shared/<semantic-type>/<document-key>_<timestamp>/
```

The first five product type parents each contain at most one current document directory; `others` may contain multiple distinct documents. A normal document directory has one original and one same-stem Markdown. A standalone Markdown explicitly identified by the user as personally authored or approved canonical knowledge is stored unchanged as a one-file source slot, without a duplicate companion. Sources covering more than one product always use `_shared/`. The baseline timestamp `202601010000` records migration time, not publication time. Extracted images are not stored.

## Simple sync workflow

1. Put new original PDF, PPT/PPTX, Word, Excel, or other official product documents in `newly_added/`. Personally authored Markdown is also accepted when the user explicitly identifies or approves it as canonical knowledge.
2. Explicitly ask an Agent with repository write access to follow `SYNC_PROMPT.md`.
3. The Agent groups same-lineage inputs first, keeps only the explicitly newer revision when several arrive together, classifies scope and semantic type, cautiously decides add versus replacement, creates a semantically lossless companion when needed, updates exhaustive product Hubs and affected Vault pages, records local discrepancies, validates, and removes successful inbox files.
4. Ambiguous files remain in `newly_added/` until the user decides how they should be classified.
5. Review the resulting Git diff before committing.

No manifest or custom sync script is required. Git history provides change review and recovery.

## Important files

| Path | Purpose |
| --- | --- |
| `SKILL.md` | Product-expert retrieval and response behavior |
| `SYNC_PROMPT.md` | Explicit, user-triggered maintenance workflow |
| `newly_added/` | Inbox for unsynchronized original documents |
| `product-knowledge-vault/index.md` | Stable RAG entry point and Obsidian catalog |
| `product-knowledge-vault/products/` | Exhaustive current-source Hub for each product |
| `product-knowledge-vault/shared/` | Knowledge-graph nodes for multi-product sources |
| `product-knowledge-vault/SCHEMA.md` | Vault page and linking conventions |

The synchronized local official source documents are the sole evidence base for product facts. The Vault summarizes them; it does not add a separate web evidence layer.
