# DT50S — Source Hub

This page is the exhaustive discovery entry for the product's currently synchronized local sources. Read it before answering any DT50S question. Older product-specific documents use the DT50 label; treat them as retained source filenames for the DT50S lineage.

## Current Source Coverage

| Type | Document key | Document | Markdown | Original |
| --- | --- | --- | --- | --- |
| brochure | `default_202601010000` | DT50S — Enterprise Mobile Computer (source labeled DT50) | `DT50S/brochure/default_202601010000/DT50(EN)-PB-S20241120.md` | `DT50S/brochure/default_202601010000/DT50(EN)-PB-S20241120.pdf` |
| specs | `default_202601010000` | DT50S — Rugged Mobile Computer Specification (source labeled DT50) | `DT50S/specs/default_202601010000/DT50(EN)-SPEC-S20241118.md` | `DT50S/specs/default_202601010000/DT50(EN)-SPEC-S20241118.pdf` |
| user_guide | `default_202608151554` | DT50S — Mobile Computer User Guide (source labeled DT50) | `DT50S/user_guide/default_202608151554/DT50(EN)_User_Guide_20230420.md` | `DT50S/user_guide/default_202608151554/DT50(EN)_User_Guide_20230420.pdf` |
| others | `internal-model-mapping_202608121411` | DT50S / SQ53S / SQ53ST Internal Model Mapping | `DT50S/others/internal-model-mapping_202608121411/DT50S_internal_models.md` | Authored Markdown (canonical source) |
| others | `quick-start-guide_202608151554` | DT50S — Quick Start Guide (source cover labeled DT50) | `DT50S/others/quick-start-guide_202608151554/DT50S-Quick-Start-Guide.md` | `DT50S/others/quick-start-guide_202608151554/DT50S-Quick-Start-Guide.pdf` |
| others | `drop-tumble-reliability-report_202609102000` | DT50S — Drop and Tumble Reliability Test Report (sample SQ53S; report date 2022.09.01) | `DT50S/others/drop-tumble-reliability-report_202609102000/DT50S跌落及滚筒-可靠性测试报告20220901.md` | `DT50S/others/drop-tumble-reliability-report_202609102000/DT50S跌落及滚筒-可靠性测试报告20220901.pdf` |
| others | `after-sales-bom_202609111450` | DT50S (SQ53S) After-Sales Spare Parts BOM (filename date 20260101; Sheet3 is SQ53X) | `DT50S/others/after-sales-bom_202609111450/DT50S(SQ53S)_After_Sales_Spare_Parts_BOM-20260101.md` | `DT50S/others/after-sales-bom_202609111450/DT50S(SQ53S)_After_Sales_Spare_Parts_BOM-20260101.xlsx` |
| others | `service-manual_202609121520` | DT50 Service Manual (source labeled DT50; after-sales teardown; optional UHF handle is an accessory, not DT50P) | `DT50S/others/service-manual_202609121520/DT50-Service-Manual.md` | `DT50S/others/service-manual_202609121520/DT50-Service-Manual.doc` |

## Vault Knowledge

- [[spec/DT50S|DT50S Specification]]
- [[pb/DT50S|DT50S Brochure / Product Page]]
- [[categories/handheld-terminal|Handheld Terminal]]

## Shared Knowledge

- [[shared/device-and-accessories-guide|Device and Accessories Guide]] — portfolio-wide device/accessory configurations, codes, material numbers, and status
- [[shared/dt50-series-accessories-guide|DT50 Series Accessories Guide]] — current DT50S / DT50-Pro batteries, cradles, protection, carrying, and trigger accessories
- [[shared/gms-google-key-factory-programming-status|GMS Google Key Factory Programming Status]] — Google Key requirement and factory writing status by internal project
- [[shared/gms-aer-certification-summary|GMS and AER Certification Summary]] — certification regions, windows, and maintenance history by project
- [[shared/mdm-certification-summary|MDM Certification Summary]] — MDM validation by project and Android version

- [[shared/pda-info-summary|PDA Platform, Memory, and Android Summary]] — user-authored project, platform, memory, and Android mapping
- [[shared/sq53pro-vs-sq53st-battlecard|SQ53PRO vs SQ53ST Battle Card]] — direct DT50S/SQ53ST versus DT50PRO/SQ53PRO comparison; the deck itself uses DT50 for SQ53ST
- [[shared/urovo-pda-battlecard|Urovo PDA Battlecard 2025-12-05]] — DT50S lineage 4G and separate DT50 5G competitive comparison tables
- [[shared/urovo-spec-comparison|Urovo Spec Comparison 241030]] — dated 2024-10-30 competitive sheet; not a live competitor-spec feed
- [[shared/urovo-product-price-book-2026-7-25|Urovo Product Price Book (2026-07-25)]] — dated commercial USD price list; not a live spec

- [[shared/urovo-product-brochure-europe-20260904|UROVO Product Brochure — Europe Edition (2026-09-04)]] — dated multi-product marketing claims, configurations, accessories, and UEE ecosystem
- [[shared/urovo-product-brochure-na-20260904|UROVO Product Brochure — North America Edition (2026-09-04)]] — dated NA-region portfolio brochure (Irvine / us.urovo.com); product mix differs from the Europe edition

## Active Local Source Discrepancies

| Field | Value A | Source A | Value B | Source B | Status |
| --- | --- | --- | --- | --- | --- |
| SQ53ST market-model label | DT50 | `_shared/comparison/sq53pro-vs-sq53st-battlecard_202608111913/SQ53PRO VS SQ53ST Battle Card.md`; retained product brochure/spec filenames | DT50S | `DT50S/others/internal-model-mapping_202608121411/DT50S_internal_models.md`; `_shared/specs/pda-info-summary_202608111748/pda-info-summary.md`; `_shared/accessories/device-and-accessories-guide_202608111226/Device_and_Accessories_Guide_20260810.md` | Canonical Hub is DT50S; retain and surface source-specific DT50 labeling when relevant |
| Android version | Android 16 | `_shared/brochure/urovo-product-brochure-europe_202609111045/UROVO Product brochure - 20260904 (EU).md` (page 4, source panel labeled `DT50`); `_shared/brochure/urovo-product-brochure-na_202609111045/UROVO Product brochure - 20260904 (NA).md` (page 4, source panel labeled `DT50`) | Android 11; Android 13 optional | `DT50S/specs/default_202601010000/DT50(EN)-SPEC-S20241118.md` | Unresolved dated/lineage difference; qualify the source and do not silently treat Android 16 as the current dedicated-spec value |
| Android version | Android 13 | `_shared/comparison/urovo-spec-comparison_202609102000/Urovo_spec_comparation_241030.md` (sheet `DT50S& CT58S `, B6) | Android 11; Android 13 optional | `DT50S/specs/default_202601010000/DT50(EN)-SPEC-S20241118.md` | Unresolved dated comparison; do not drop the optional-11 framing |
| Rear camera | 16 MP PDAF in body copy | `_shared/brochure/urovo-product-brochure-europe_202609111045/UROVO Product brochure - 20260904 (EU).md` (page 4); `_shared/brochure/urovo-product-brochure-na_202609111045/UROVO Product brochure - 20260904 (NA).md` (page 4) | 13 MP in the same panel's icon and in the dedicated specification | Same brochure page; `DT50S/specs/default_202601010000/DT50(EN)-SPEC-S20241118.md` | Unresolved intra-brochure and cross-source difference |

## Query Coverage Rule

- Treat the source table above as the complete discovery set for this product.
- Read every source of the relevant type; for a broad or exhaustive request, read every listed Markdown source.
- If routing remains uncertain, search all Markdown under `DT50S/` and linked `_shared/` sources before concluding that information is unavailable.
