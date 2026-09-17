# K388 Pro — Source Hub

This page is the exhaustive discovery entry for the product's currently synchronized local sources. Read it before answering any K388 Pro question.

## Current Source Coverage

| Type | Document key | Document | Markdown | Original |
| --- | --- | --- | --- | --- |
| brochure | `default_202601010000` | K388 Pro — Mobile Labeling Printer | `K388 Pro/brochure/default_202601010000/K388Pro(EN)-PB-20250925.md` | `K388 Pro/brochure/default_202601010000/K388Pro(EN)-PB-20250925.pdf` |
| specs | `default_202601010000` | K388 Pro — All-in-One Mobile POS Terminal Specification | `K388 Pro/specs/default_202601010000/K388 Pro(EN)-SPEC-20250925.md` | `K388 Pro/specs/default_202601010000/K388 Pro(EN)-SPEC-20250925.pdf` |
| others | `after-sales-bom-no-rfid_202609111450` | K388 Pro (ILS2) After-Sales Repair Quotation — Normal / No-RFID | `K388 Pro/others/after-sales-bom-no-rfid_202609111450/K388Pro_Normal(No-RFID)_After_Sales_Spare_Parts_BOM-20260101.md` | `K388 Pro/others/after-sales-bom-no-rfid_202609111450/K388Pro_Normal(No-RFID)_After_Sales_Spare_Parts_BOM-20260101.xlsx` |
| others | `after-sales-bom-rfid_202609111450` | K388 Pro (ILS2) After-Sales Repair Quotation — RFID | `K388 Pro/others/after-sales-bom-rfid_202609111450/K388Pro_RFID_After_Sales_Spare_Parts_BOM-20260101.md` | `K388 Pro/others/after-sales-bom-rfid_202609111450/K388Pro_RFID_After_Sales_Spare_Parts_BOM-20260101.xlsx` |

## Vault Knowledge

- [[spec/K388-Pro|K388 Pro Specification]]
- [[pb/K388-Pro|K388 Pro Brochure / Product Page]]
- [[categories/mobile-printer|Mobile Printer]]

## Shared Knowledge

- [[shared/printer-consumables-knowledge|打印机知识点（耗材）]] — thermal vs thermal-transfer and ribbon/media pairing; no named model
- [[shared/device-and-accessories-guide|Device and Accessories Guide]] — portfolio-wide device/accessory configurations, codes, material numbers, and status
- [[shared/k388-pro-series-product-spec-sheet|K388 Pro Series Product Spec Sheet]] — K388 Pro, K388 Pro 4, and K388 Pro BT positioning and specifications
- [[shared/gms-google-key-factory-programming-status|GMS Google Key Factory Programming Status]] — Google Key requirement and factory writing status by internal project
- [[shared/gms-aer-certification-summary|GMS and AER Certification Summary]] — EDLA and SMR history for the K388 Pro project
- [[shared/mdm-certification-summary|MDM Certification Summary]] — MDM validation by Android version

- [[shared/pda-info-summary|PDA Platform, Memory, and Android Summary]] — user-authored project, platform, memory, and Android mapping
- [[shared/urovo-pda-battlecard|Urovo PDA Battlecard 2025-12-05]] — dated K388 Pro/K388S comparison against Avery Dennison Pathfinder 6059 variants
- [[shared/urovo-product-price-book-2026-7-25|Urovo Product Price Book (2026-07-25)]] — dated commercial USD price list; not a live spec

- [[shared/urovo-product-brochure-europe-20260904|UROVO Product Brochure — Europe Edition (2026-09-04)]] — dated multi-product marketing claims, configurations, accessories, and UEE ecosystem
- [[shared/urovo-product-brochure-na-20260904|UROVO Product Brochure — North America Edition (2026-09-04)]] — dated NA-region portfolio brochure (Irvine / us.urovo.com); product mix differs from the Europe edition
- [[shared/urovo-rfid-product-brochure-20260904|UROVO RFID Product Brochure (2026-09-04)]] — dated RFID-focused multi-product brochure

## Active Local Source Discrepancies

| Field | Value A | Source A | Value B | Source B | Status |
| --- | --- | --- | --- | --- | --- |
| Bluetooth | BT 5.0 | `_shared/accessories/device-and-accessories-guide_202608111226/Device_and_Accessories_Guide_20260810.md` (`K388 Pro!C6`) | BT 5.3 | `K388 Pro/specs/default_202601010000/K388 Pro(EN)-SPEC-20250925.md`; `_shared/specs/k388-pro-series-product-spec-sheet_202608111352/K388Pro PRODUCT SPEC SHEET 20260617 .md` | Unresolved; both product specification sources say 5.3, while the shared device/accessory guide says 5.0 |
| Camera position/coverage | Side, 13 MP | `_shared/comparison/urovo-pda-battlecard_202608111913/Urovo PDA Battlecard_20251205.md` | Front 5 MP plus rear 13 MP with flash | `K388 Pro/specs/default_202601010000/K388 Pro(EN)-SPEC-20250925.md` | Unresolved terminology/coverage difference; 13 MP agrees |

## Query Coverage Rule

- Treat the source table above as the complete discovery set for this product.
- Read every source of the relevant type; for a broad or exhaustive request, read every listed Markdown source.
- If routing remains uncertain, search all Markdown under `K388 Pro/` and linked `_shared/` sources before concluding that information is unavailable.
