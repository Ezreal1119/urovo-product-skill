# CT48C — Source Hub

This page is the exhaustive discovery entry for the product's currently synchronized local sources. Read it before answering any CT48C question.

## Current Source Coverage

| Type | Document key | Document | Markdown | Original |
| --- | --- | --- | --- | --- |
| brochure | `default_202601010000` | CT48C — Enterprise Mobile Computer | `CT48C/brochure/default_202601010000/CT48C(EN)-PB-20250206.md` | `CT48C/brochure/default_202601010000/CT48C(EN)-PB-20250206.pdf` |
| specs | `default_202608111352` | CT48C — Handheld Terminal Specification | `CT48C/specs/default_202608111352/CT48C(EN)-SPEC-20250219.md` | `CT48C/specs/default_202608111352/CT48C(EN)-SPEC-20250219.pdf` |
| presentation | `product-introduction_202608111352` | CT48C Product Introduction Presentation | `CT48C/presentation/product-introduction_202608111352/CT48C Product Introduction Presentation.md` | `CT48C/presentation/product-introduction_202608111352/CT48C Product Introduction Presentation.pptx` |
| others | `internal-model-mapping_202608121411` | CT48C / SQ48C Internal Model Mapping | `CT48C/others/internal-model-mapping_202608121411/CT48C_internal_models.md` | Authored Markdown (canonical source) |

## Vault Knowledge

- [[spec/CT48C|CT48C Specification]]
- [[pb/CT48C|CT48C Brochure / Product Page]]
- [[categories/handheld-terminal|Handheld Terminal]]

## Shared Knowledge

- [[shared/device-and-accessories-guide|Device and Accessories Guide]] — portfolio-wide device/accessory configurations, codes, material numbers, and status
- [[shared/gms-google-key-factory-programming-status|GMS Google Key Factory Programming Status]] — Google Key requirement and factory writing status by internal project

- [[shared/pda-info-summary|PDA Platform, Memory, and Android Summary]] — user-authored project, platform, memory, and Android mapping

- [[shared/gms-certification-reuse-statistics|GMS Certification Reuse Statistics]] — which internal models reuse (套用) another model's GMS certification, keyed by ro.product.device with application time
- [[shared/urovo-product-price-book-2026-7-25|Urovo Product Price Book (2026-07-25)]] — dated commercial USD price list; not a live spec

- [[shared/urovo-product-brochure-europe-20260904|UROVO Product Brochure — Europe Edition (2026-09-04)]] — dated multi-product marketing claims, configurations, accessories, and UEE ecosystem

## Active Local Source Discrepancies

| Field | Value A | Source A | Value B | Source B | Status |
| --- | --- | --- | --- | --- | --- |
| Weight | 268 g with standard battery | `CT48C/specs/default_202608111352/CT48C(EN)-SPEC-20250219.md`; `CT48C/brochure/default_202601010000/CT48C(EN)-PB-20250206.md` | 252 g | `CT48C/presentation/product-introduction_202608111352/CT48C Product Introduction Presentation.md` | Unresolved; the presentation does not state whether its weight excludes the battery |
| AnTuTu score | 200K+ | `CT48C/others/internal-model-mapping_202608121411/CT48C_internal_models.md` | 250K | `CT48C/brochure/default_202601010000/CT48C(EN)-PB-20250206.md` | Unresolved; use the product brochure for the published benchmark while preserving the authored internal mapping |

## Query Coverage Rule

- Treat the source table above as the complete discovery set for this product.
- Read every source of the relevant type; for a broad or exhaustive request, read every listed Markdown source.
- If routing remains uncertain, search all Markdown under `CT48C/` and linked `_shared/` sources before concluding that information is unavailable.
