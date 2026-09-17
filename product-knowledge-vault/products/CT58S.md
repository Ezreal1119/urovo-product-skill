# CT58S — Source Hub

This page is the exhaustive discovery entry for the product's currently synchronized local sources. Read it before answering any CT58S question.

## Current Source Coverage

| Type | Document key | Document | Markdown | Original |
| --- | --- | --- | --- | --- |
| brochure | `default_202601010000` | CT58S — Enterprise Mobile Computer | `CT58S/brochure/default_202601010000/CT58S(EN)-PB-20241207.md` | `CT58S/brochure/default_202601010000/CT58S(EN)-PB-20241207.pdf` |
| specs | `default_202601010000` | CT58S — Handheld Terminal Specification | `CT58S/specs/default_202601010000/CT58S(EN)-SPEC-20241204.md` | `CT58S/specs/default_202601010000/CT58S(EN)-SPEC-20241204.pdf` |
| user_guide | `default_202608151554` | CT58S — Mobile Computer User Guide | `CT58S/user_guide/default_202608151554/CT58S(EN)-User Guide-20241119.md` | `CT58S/user_guide/default_202608151554/CT58S(EN)-User Guide-20241119.pdf` |
| others | `internal-model-mapping_202608121411` | CT58S / SQ58S Internal Model Mapping | `CT58S/others/internal-model-mapping_202608121411/CT58S_internal_models.md` | Authored Markdown (canonical source) |
| others | `after-sales-bom_202609111450` | CT58S (SQ58S) After-Sales Spare Parts BOM (Eurasia edition; filename date 20260101) | `CT58S/others/after-sales-bom_202609111450/CT58S(SQ58S)_After_Sales_Spare_Parts_BOM-20260101.md` | `CT58S/others/after-sales-bom_202609111450/CT58S(SQ58S)_After_Sales_Spare_Parts_BOM-20260101.xlsx` |
| others | `service-manual_202609121520` | CT58S Service Manual (after-sales teardown; HS7 / 2030S scan engines; consumables header prints DT58S) | `CT58S/others/service-manual_202609121520/CT58S Service Manual.md` | `CT58S/others/service-manual_202609121520/CT58S Service Manual.doc` |

## Vault Knowledge

- [[spec/CT58S|CT58S Specification]]
- [[pb/CT58S|CT58S Brochure / Product Page]]
- [[categories/handheld-terminal|Handheld Terminal]]

## Shared Knowledge

- [[shared/device-and-accessories-guide|Device and Accessories Guide]] — portfolio-wide device/accessory configurations, codes, material numbers, and status
- [[shared/gms-google-key-factory-programming-status|GMS Google Key Factory Programming Status]] — Google Key requirement and factory writing status by internal project
- [[shared/gms-aer-certification-summary|GMS and AER Certification Summary]] — certification status and regional context by project
- [[shared/mdm-certification-summary|MDM Certification Summary]] — SOTI validation by project and Android version

- [[shared/pda-info-summary|PDA Platform, Memory, and Android Summary]] — user-authored project, platform, memory, and Android mapping

- [[shared/gms-certification-reuse-statistics|GMS Certification Reuse Statistics]] — which internal models reuse (套用) another model's GMS certification, keyed by ro.product.device with application time

- [[shared/urovo-product-brochure-europe-20260904|UROVO Product Brochure — Europe Edition (2026-09-04)]] — dated multi-product marketing claims, configurations, accessories, and UEE ecosystem
- [[shared/urovo-spec-comparison|Urovo Spec Comparison 241030]] — dated 2024-10-30 competitive sheet (CT58S column); not a live competitor-spec feed

## Active Local Source Discrepancies

| Field | Value A | Source A | Value B | Source B | Status |
| --- | --- | --- | --- | --- | --- |
| SQ58S Android version | Android 12 | `_shared/specs/pda-info-summary_202608111748/pda-info-summary.md`; `CT58S/specs/default_202601010000/CT58S(EN)-SPEC-20241204.md` (product spec lacks an SQ qualifier) | Android 14 | `_shared/certificates/gms-aer-certification-summary_202609071236/GMS+AER认证汇总.md`; `_shared/certificates/mdm-certification-summary_202608111723/MDM认证汇总.md` | Unresolved; the authored matrix reserves Android 14 for SQ58SU, while both certification workbooks label SQ58S as Android 14. The 2024-10-30 comparison lists `Android 12.0,Upgradeable to Android14`. |
| CPU speed | MT 6762, Octa-core 2.0 GHz | `_shared/comparison/urovo-spec-comparison_202609102000/Urovo_spec_comparation_241030.md` (sheet `DT50S& CT58S `, C7) | Octa-core 2.2 GHz | `CT58S/specs/default_202601010000/CT58S(EN)-SPEC-20241204.md` | Unresolved dated comparison; use product specs first for current hard-spec answers |

## Query Coverage Rule

- Treat the source table above as the complete discovery set for this product.
- Read every source of the relevant type; for a broad or exhaustive request, read every listed Markdown source.
- If routing remains uncertain, search all Markdown under `CT58S/` and linked `_shared/` sources before concluding that information is unavailable.
