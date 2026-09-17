# RT40S — Source Hub

This page is the exhaustive discovery entry for the product's currently synchronized local sources. Read it before answering any RT40S question.

## Current Source Coverage

| Type | Document key | Document | Markdown | Original |
| --- | --- | --- | --- | --- |
| brochure | `default_202601010000` | RT40S — Premium Handheld Terminal | `RT40S/brochure/default_202601010000/RT40S(EN)_PB-20241121.md` | `RT40S/brochure/default_202601010000/RT40S(EN)_PB-20241121.pdf` |
| specs | `default_202601010000` | RT40S — Handheld Intelligent Terminal Specification | `RT40S/specs/default_202601010000/RT40S(EN)-SPEC-20241118.md` | `RT40S/specs/default_202601010000/RT40S(EN)-SPEC-20241118.pdf` |
| user_guide | `default_202608151629` | RT40S — Mobile Computer User Guide | `RT40S/user_guide/default_202608151629/RT40S(EN)_User_Guide_20240205.md` | `RT40S/user_guide/default_202608151629/RT40S(EN)_User_Guide_20240205.pdf` |
| accessories | `default_202608151629` | RT40S Accessories Brochure | `RT40S/accessories/default_202608151629/RT40S_Accessories_brochure_20250806.md` | `RT40S/accessories/default_202608151629/RT40S_Accessories_brochure_20250806.pdf` |
| others | `internal-model-mapping_202608121411` | RT40S / SQ47 Series Internal Model Mapping | `RT40S/others/internal-model-mapping_202608121411/RT40S_internal_models.md` | Authored Markdown (canonical source) |
| others | `after-sales-bom_202609111045` | RT40S (SQ47S–SQ47SP) After-sales Component BOM V1.00 (2024-07-25) | `RT40S/others/after-sales-bom_202609111045/RT40S(SQ47S-SQ47SP)——售后组件BOM-V1.00-20240725.md` | `RT40S/others/after-sales-bom_202609111045/RT40S(SQ47S-SQ47SP)——售后组件BOM-V1.00-20240725.xlsx` |
| others | `service-manual_202609121547` | RT40 Service Manual v1.0 (2022-12-13; source labeled RT40; routed to RT40S) | `RT40S/others/service-manual_202609121547/RT40_Service_Manual.md` | `RT40S/others/service-manual_202609121547/RT40_Service_Manual.doc` |

## Vault Knowledge

- [[spec/RT40S|RT40S Specification]]
- [[pb/RT40S|RT40S Brochure / Product Page]]
- [[categories/handheld-terminal|Handheld Terminal]]

## Shared Knowledge

- [[shared/device-and-accessories-guide|Device and Accessories Guide]] — portfolio-wide device/accessory configurations, codes, material numbers, and status
- [[shared/gms-google-key-factory-programming-status|GMS Google Key Factory Programming Status]] — Google Key requirement and factory writing status by internal project
- [[shared/gms-aer-certification-summary|GMS and AER Certification Summary]] — certification regions, windows, and maintenance history by project
- [[shared/mdm-certification-summary|MDM Certification Summary]] — MDM validation by project and Android version

- [[shared/pda-info-summary|PDA Platform, Memory, and Android Summary]] — user-authored project, platform, memory, and Android mapping
- [[shared/urovo-pda-battlecard|Urovo PDA Battlecard 2025-12-05]] — dated RT40S comparison against Zebra, Honeywell, Newland, and Seuic devices
- [[shared/urovo-spec-comparison|Urovo Spec Comparison 241030]] — dated 2024-10-30 competitive sheet (RT40S column); not a live competitor-spec feed
- [[shared/urovo-product-price-book-2026-7-25|Urovo Product Price Book (2026-07-25)]] — dated commercial USD price list; not a live spec

- [[shared/urovo-product-brochure-europe-20260904|UROVO Product Brochure — Europe Edition (2026-09-04)]] — dated multi-product marketing claims, configurations, accessories, and UEE ecosystem
- [[shared/urovo-product-brochure-na-20260904|UROVO Product Brochure — North America Edition (2026-09-04)]] — dated NA-region portfolio brochure (Irvine / us.urovo.com); product mix differs from the Europe edition

## Active Local Source Discrepancies

| Field | Value A | Source A | Value B | Source B | Status |
| --- | --- | --- | --- | --- | --- |
| Market-model label | RT40 | `RT40S/others/service-manual_202609121547/RT40_Service_Manual.md` (title, revision note, parts headers) | RT40S | `RT40S/others/internal-model-mapping_202608121411/RT40S_internal_models.md`; `RT40S/specs/default_202601010000/RT40S(EN)-SPEC-20241118.md` | Canonical Hub is RT40S per user routing; retain and surface the source-specific RT40 label |
| Power adapter | QC3.0; Input 100-240V~50/60Hz 0.6AMAX; Output 5V/3A, 9V/2A, 12V/1.5A | `RT40S/others/service-manual_202609121547/RT40_Service_Manual.md` (Accessories) | 中规 YHPC052000A0 5V,2A USB | `RT40S/others/after-sales-bom_202609111045/RT40S(SQ47S-SQ47SP)——售后组件BOM-V1.00-20240725.md` (adapter row) | Unresolved dated accessory difference; do not silently pick a winner |

## Query Coverage Rule

- Treat the source table above as the complete discovery set for this product.
- Read every source of the relevant type; for a broad or exhaustive request, read every listed Markdown source.
- If routing remains uncertain, search all Markdown under `RT40S/` and linked `_shared/` sources before concluding that information is unavailable.
