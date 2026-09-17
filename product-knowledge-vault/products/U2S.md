# U2S — Source Hub

This page is the exhaustive discovery entry for the product's currently synchronized local sources. Read it before answering any U2S question.

## Current Source Coverage

| Type | Document key | Document | Markdown | Original |
| --- | --- | --- | --- | --- |
| brochure | `default_202601010000` | U2S — Wearable Computer | `U2S/brochure/default_202601010000/U2S(EN)-PB-20260526.md` | `U2S/brochure/default_202601010000/U2S(EN)-PB-20260526.pdf` |
| specs | `default_202601010000` | U2S — Wearable Computer Specification | `U2S/specs/default_202601010000/U2S(EN)-SPEC-20260526.md` | `U2S/specs/default_202601010000/U2S(EN)-SPEC-20260526.pdf` |
| user_guide | `default_202608151537` | U2S — Wearable Computer User Guide | `U2S/user_guide/default_202608151537/U2S (EN)-User Guide_20250703.md` | `U2S/user_guide/default_202608151537/U2S (EN)-User Guide_20250703.pdf` |
| others | `internal-model-mapping_202608121411` | U2S / SQ46S Internal Model Mapping | `U2S/others/internal-model-mapping_202608121411/U2S_internal_models.md` | Authored Markdown (canonical source) |

## Vault Knowledge

- [[spec/U2S|U2S Specification]]
- [[pb/U2S|U2S Brochure / Product Page]]
- [[categories/other-devices|Wearable Computer]]

## Shared Knowledge

- [[shared/device-and-accessories-guide|Device and Accessories Guide]] — portfolio-wide device/accessory configurations, codes, material numbers, and status
- [[shared/gms-google-key-factory-programming-status|GMS Google Key Factory Programming Status]] — Google Key requirement and factory writing status by internal project
- [[shared/gms-aer-certification-summary|GMS and AER Certification Summary]] — EDLA and SMR history for the SQ46S project
- [[shared/mdm-certification-summary|MDM Certification Summary]] — MDM validation for the SQ46S project

- [[shared/pda-info-summary|PDA Platform, Memory, and Android Summary]] — user-authored project, platform, memory, and Android mapping
- [[shared/urovo-pda-battlecard|Urovo PDA Battlecard 2025-12-05]] — dated U2S comparison against Zebra, Honeywell, Newland, and Seuic wearables
- [[shared/urovo-product-price-book-2026-7-25|Urovo Product Price Book (2026-07-25)]] — dated commercial USD price list; not a live spec

- [[shared/urovo-product-brochure-europe-20260904|UROVO Product Brochure — Europe Edition (2026-09-04)]] — dated multi-product marketing claims, configurations, accessories, and UEE ecosystem

## Active Local Source Discrepancies

| Field | Value A | Source A | Value B | Source B | Status |
| --- | --- | --- | --- | --- | --- |
| Battery | 3500 mAh | `_shared/comparison/urovo-pda-battlecard_202608111913/Urovo PDA Battlecard_20251205.md`; `U2S/others/internal-model-mapping_202608121411/U2S_internal_models.md`; `_shared/brochure/urovo-product-brochure-europe_202609111045/UROVO Product brochure - 20260904 (EU).md` (page 9) | 3360 mAh | `U2S/specs/default_202601010000/U2S(EN)-SPEC-20260526.md`; `U2S/brochure/default_202601010000/U2S(EN)-PB-20260526.md` | Unresolved |
| Sealing | IP67 | `_shared/comparison/urovo-pda-battlecard_202608111913/Urovo PDA Battlecard_20251205.md` | IP65 | `U2S/specs/default_202601010000/U2S(EN)-SPEC-20260526.md`; `U2S/brochure/default_202601010000/U2S(EN)-PB-20260526.md` | Unresolved |
| Camera configuration / position | Side, 13 MP | `_shared/comparison/urovo-pda-battlecard_202608111913/Urovo PDA Battlecard_20251205.md` | Top 13 MP in specs; rear 13 MP in brochure; front/rear switching in the guide's Camera UI | `U2S/specs/default_202601010000/U2S(EN)-SPEC-20260526.md`; `U2S/brochure/default_202601010000/U2S(EN)-PB-20260526.md`; `U2S/user_guide/default_202608151537/U2S (EN)-User Guide_20250703.md` | Unresolved terminology/configuration difference; the guide warns that screens and available features vary by model/OS |
| Scan engine | No scan engine | `U2S/others/internal-model-mapping_202608121411/U2S_internal_models.md` | Built-in professional scan engine with multiple options and scanner operation guidance | `U2S/specs/default_202601010000/U2S(EN)-SPEC-20260526.md`; `U2S/brochure/default_202601010000/U2S(EN)-PB-20260526.md`; `U2S/user_guide/default_202608151537/U2S (EN)-User Guide_20250703.md` | Unresolved variant/configuration difference; preserve the authored Wi-Fi-only context and do not generalize it to every U2S configuration |

## Query Coverage Rule

- Treat the source table above as the complete discovery set for this product.
- Read every source of the relevant type; for a broad or exhaustive request, read every listed Markdown source.
- If routing remains uncertain, search all Markdown under `U2S/` and linked `_shared/` sources before concluding that information is unavailable.
