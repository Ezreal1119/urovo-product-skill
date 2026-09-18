# K388 Pro — Source Hub

This page is the exhaustive discovery entry for the product's currently synchronized local sources. Read it before answering any K388 Pro question.

## Current Source Coverage

| Type | Document key | Document | Markdown | Original |
| --- | --- | --- | --- | --- |
| brochure | `default_202601010000` | K388 Pro — Mobile Labeling Printer | `K388 Pro/brochure/default_202601010000/K388Pro(EN)-PB-20250925.md` | `K388 Pro/brochure/default_202601010000/K388Pro(EN)-PB-20250925.pdf` |
| specs | `default_202609181554` | K388 Pro 2-inch dedicated specification (filename K388 Pro 2; Model UROVO K388 Pro) | `K388 Pro/specs/default_202609181554/K388 Pro 2_(EN)-SPEC-20260914.md` | `K388 Pro/specs/default_202609181554/K388 Pro 2_(EN)-SPEC-20260914.pdf` |
| others | `specs-4inch_202609181554` | K388 Pro 4 dedicated specification (185 × 144 × 137 mm, 992 g, 104 mm print). Not the 2-inch Hub spec. No K388 Pro 4 Hub. | `K388 Pro/others/specs-4inch_202609181554/K388 Pro 4_(EN)-SPEC-20260914.md` | `K388 Pro/others/specs-4inch_202609181554/K388 Pro 4_(EN)-SPEC-20260914.pdf` |
| others | `specs-bt_202609181554` | K388 Pro BT dedicated specification (ESP32, 700 g, BT v4.2). Not the Android Hub spec. No K388 Pro BT Hub. | `K388 Pro/others/specs-bt_202609181554/K388 Pro BT(EN)-SPEC-20260910.md` | `K388 Pro/others/specs-bt_202609181554/K388 Pro BT(EN)-SPEC-20260910.pdf` |
| others | `after-sales-bom-no-rfid_202609111450` | K388 Pro (ILS2) After-Sales Repair Quotation — Normal / No-RFID | `K388 Pro/others/after-sales-bom-no-rfid_202609111450/K388Pro_Normal(No-RFID)_After_Sales_Spare_Parts_BOM-20260101.md` | `K388 Pro/others/after-sales-bom-no-rfid_202609111450/K388Pro_Normal(No-RFID)_After_Sales_Spare_Parts_BOM-20260101.xlsx` |
| others | `after-sales-bom-rfid_202609111450` | K388 Pro (ILS2) After-Sales Repair Quotation — RFID | `K388 Pro/others/after-sales-bom-rfid_202609111450/K388Pro_RFID_After_Sales_Spare_Parts_BOM-20260101.md` | `K388 Pro/others/after-sales-bom-rfid_202609111450/K388Pro_RFID_After_Sales_Spare_Parts_BOM-20260101.xlsx` |

## Vault Knowledge

- [[spec/K388-Pro|K388 Pro Specification]]
- [[pb/K388-Pro|K388 Pro Brochure / Product Page]]
- [[categories/mobile-printer|Mobile Printer]]

## Shared Knowledge

- [[shared/printer-consumables-knowledge|打印机知识点（耗材）]] — thermal vs thermal-transfer and ribbon/media pairing; no named model
- [[shared/device-and-accessories-guide|Device and Accessories Guide]] — portfolio-wide device/accessory configurations, codes, material numbers, and status
- [[shared/k388-pro-series-product-spec-sheet|K388 Pro Series Product Spec Sheet]] — K388 Pro 2’’, K388 Pro 4’’, and K388 Pro BT positioning and specifications (7-page 2026-09-16 edition)
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
| Bluetooth version | BT 5.0 | `_shared/accessories/device-and-accessories-guide_202608111226/Device_and_Accessories_Guide_20260810.md` (`K388 Pro!C6`) | BT 5.3 | `K388 Pro/specs/default_202609181554/K388 Pro 2_(EN)-SPEC-20260914.md`; `_shared/specs/k388-pro-series-product-spec-sheet_202609181554/K388Pro PRODUCT SPEC SHEET .md` | Unresolved; both current product specification sources say 5.3, while the shared device/accessory guide says 5.0 |
| Bluetooth class (Android 2’’ / 4’’) | Class 2, Bluetooth v5.3 and secondary BLE | `K388 Pro/specs/default_202609181554/K388 Pro 2_(EN)-SPEC-20260914.md`; series sheet page 4 | Configurable Class 1 and 2, Bluetooth v5.3; Classic BR/EDR and Bluetooth LE | `_shared/specs/k388-pro-series-product-spec-sheet_202609181554/K388Pro PRODUCT SPEC SHEET .md` page 6 WIRELESS PAN | Unresolved intra-series plus dedicated-spec vs series page 6; same Android K388 Pro wireless-PAN context |
| Camera position/coverage | Side, 13 MP | `_shared/comparison/urovo-pda-battlecard_202608111913/Urovo PDA Battlecard_20251205.md` | Front 5 MP plus rear 13 MP with flash | `K388 Pro/specs/default_202609181554/K388 Pro 2_(EN)-SPEC-20260914.md` | Unresolved terminology/coverage difference; 13 MP agrees |
| Operating system wording | Android 14 | `K388 Pro/brochure/default_202601010000/K388Pro(EN)-PB-20250925.md`; series sheet page 2 marketing block | Android 14, Upgradable to Android 20 | `K388 Pro/specs/default_202609181554/K388 Pro 2_(EN)-SPEC-20260914.md`; series sheet page 4 | Unresolved; brochure/page-2 marketing omit the upgrade ceiling that the specification tables print |
| Cellular / 4G | 4G | `K388 Pro/brochure/default_202601010000/K388Pro(EN)-PB-20250925.md` (Connectivity) | Not listed | `K388 Pro/specs/default_202609181554/K388 Pro 2_(EN)-SPEC-20260914.md` | Unresolved; brochure lists 4G, dedicated specification has no cellular/WWAN row |
| K388 Pro 4 drop specification | Multiple 5 ft. / 1.5 m drop to concrete at room temperature | `K388 Pro/others/specs-4inch_202609181554/K388 Pro 4_(EN)-SPEC-20260914.md` | Multiple 4 ft. / 1.2 m drop to concrete at room temperature | `_shared/specs/k388-pro-series-product-spec-sheet_202609181554/K388Pro PRODUCT SPEC SHEET .md` page 5 (K388 Pro 4’’ column) | Unresolved; 4-inch variant only — do not apply to the 2-inch Hub product |
| K388 Pro 4 optional UHF | Not listed | `K388 Pro/others/specs-4inch_202609181554/K388 Pro 4_(EN)-SPEC-20260914.md` | UHF RFID Tag Encoding (optional) spanning the 2’’ and 4’’ columns | `_shared/specs/k388-pro-series-product-spec-sheet_202609181554/K388Pro PRODUCT SPEC SHEET .md` page 6 | Unresolved; 4-inch variant only |

K388 Pro BT (ESP32, BT v4.2, 700 g, 0.9 inch OLED) is a different series SKU documented under `others/specs-bt_` and the series sheet BT column. Do not flatten BT values into Android K388 Pro answers.

## Query Coverage Rule

- Treat the source table above as the complete discovery set for this product.
- Lead hard specs for the Hub product from `K388 Pro/specs/` (2-inch dedicated spec). Use `others/specs-4inch_` and `others/specs-bt_` only when the question is about those variants.
- Read every source of the relevant type; for a broad or exhaustive request, read every listed Markdown source.
- If routing remains uncertain, search all Markdown under `K388 Pro/` and linked `_shared/` sources before concluding that information is unavailable.
