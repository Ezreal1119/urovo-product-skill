# Operation Log

## [2026-09-15] sync | K180/K200/K220 user guides + printer consumables note

Inbox had 4 real inputs. Synchronized all 4.

| Source | Decision |
| --- | --- |
| K180-Barcode-Scanner-User Manual_V1.0.2.pdf | Added first `K180/user_guide/default_202609151652`. V1.0.2 (2025/08/20). 218/218 pages. CODEK cover drawing; Limei Xincheng disclaimer. Programming-barcode manual. |
| K200-Wired-Industrial-Scanner-User-Manual.pdf | Added first `K200/user_guide/default_202609151652`. Revision through V1.0.5 (2024.03.07). 220/220 pages. Teal [User Guide] cover. Config software marked `To be release`. |
| K220-wireless-industrial-scanner-user-manual.pdf | Added first `K220/user_guide/default_202609151652`. 229/229 pages. Cover title-only; text layer Keyid not visible on cover. Disclaimer Limei Xincheng. Includes SBC220 settings. |
| 打印机耗材知识点.docx | Added `_shared/operations/printer-consumables-knowledge_202609151652`. Cover title 打印机知识点 A0 / 23.3.16. 5/5 pages, 2/2 images. Backlinked K329, K388 Pro, K389, K419, D8100 plus, D81R Series. |

No new Hub discrepancies. User guides are operation/programming sources; lead hard specs from product `specs/`.

## [2026-09-12] sync | RT40 service manual → RT40S; drop DT30 / i5000 inbox leftovers

User decision on the four leftover inbox files:

| Source | Decision |
| --- | --- |
| RT40_Service_Manual.doc | Added `RT40S/others/service-manual_202609121547`. Body is RT40 Service Manual v1.0 (2022-12-13, WuDongni). No RT40S/SQ47S strings. 16/16 pages, 46/46 images. Routed to RT40S per user. Hub discrepancies: market label RT40 vs RT40S; QC3.0 5V/3A·9V/2A·12V/1.5A vs BOM 5V/2A adapter. |
| DT30_Disassembly and assembly manual.docx | Discarded from inbox (no DT30 Hub). |
| i5000_SQ65A_Maintenance_Service_Manual.pdf | Discarded from inbox (no i5000 Hub). |
| i5000_SQ65A_Safe_Mode_Clear_Manual.pdf | Discarded from inbox (no i5000 Hub). |

## [2026-09-12] sync | After-sales service / trigger / disassembly manuals

Inbox was mostly after-sales. Synchronized 10 document identities (11 inbox files; one i9200 trigger pair was byte-identical). Left 4 because they have no Product Hub.

| Source | Decision |
| --- | --- |
| CT48_Maintenance_Service_Manual.doc | Added `CT48/others/maintenance-service-manual_202609121520`. 11/11 pages, 26/26 images. Leftover Chinese TOC lists 产品参数 / OS下载 / 写号 / 全功能测试 / FAQ that are not in this edition. Parts header prints `CT58 Main repair parts`. |
| CT58-Maintenance-Service-Manual.doc | Added `CT58/others/maintenance-service-manual_202609121520`. 12/12 pages, 35/35 images. Optional handle. |
| CT58S Service Manual.doc | Added `CT58S/others/service-manual_202609121520`. 12/12 pages, 37/37 images. HS7 and 2030S scan engines. Consumables header prints `DT58S`. |
| DT40_Disassembly_Assembly_Manual.docx | Added `DT40/others/disassembly-assembly-manual_202609121520`. 27/27 pages, 27/27 images. Bilingual teardown + assembly. Distinct from the English service-manual template. |
| DT40_Maintenance_Service_Manual.doc | Added `DT40/others/maintenance-service-manual_202609121520`. 19/19 pages, 44/44 images. Accessories + parts catalog. |
| DT50-Service-Manual.doc | Added `DT50S/others/service-manual_202609121520`. Body titled DT50; no SQ53/5G. Optional UHF handle is an accessory, not DT50P. 15/15 pages, 41/41 images. |
| DT66_Maintenance_Service_Manual_20241218.pdf | Added `DT66/others/maintenance-service-manual_202609121520`. 14/14 pages. Common-fault chapter includes scan-type code `*#1261*#`. |
| i5300(SQ65F)_Safe_Mode_Clear_Manual-20260126.doc | Added `i5300L/others/trigger-maintenance-manual_202609121520`. Body title `i5300L Trigger Maintenance Manual`. Filename i5300/SQ65F retained; routed to i5300L (SQ65F), not i5300. Hardware-trigger codes, not a generic safe-mode UI guide. 12/12 pages, 34/34 images. |
| i9200 Trigger Repair Guidebook V1.0.doc (byte-identical to `i9200(SQ68)_Safe_Mode_Clear_Manual.doc`) | Added `i9200/others/trigger-repair-guidebook_202609121520`. 7/7 pages, 12/12 images. Both inbox copies removed after one original. |
| i9200_Maintenance_Service_Manual_20251107.doc | Added `i9200/others/maintenance-service-manual_202609121520`. 20/20 pages, 57/57 images. §5.1 red trigger points to the Trigger Maintenance Guide. |
| RT40_Service_Manual.doc | Left. Title RT40; no RT40S/SQ47S; no RT40 Hub. Same ask as the previous inbox copy. |
| DT30_Disassembly and assembly manual.docx | Left. Body is DT30 拆装机. No DT30 Hub. |
| i5000_SQ65A_Maintenance_Service_Manual.pdf | Left. Title I5000 Service Manual. No i5000 Hub. |
| i5000_SQ65A_Safe_Mode_Clear_Manual.pdf | Left. Cover is SQ65A Trigger Maintenance Instruction Manual (2024.09.03). No i5000 Hub. |

No new shared Vault nodes. No new Hub discrepancies (service manuals are not live specs). Successful inbox copies removed after verification.

## [2026-09-12] sync | Replace Urovo Product Price Book 2026_7_24 → 2026_7_25

User-supplied `/Users/patrickxu/Downloads/Urovo_Product_Price_Book-2026_7_25.xls` is the next dated revision of the same commercial price book. Replaced `_shared/pricing/urovo-product-price-book_202609112225` with `_shared/pricing/urovo-product-price-book_202609121037`. SHA-256 `89824c722d9d852a…`.

Cell change: Optional Config only. Model rows, USD prices, and 77/77 pictures unchanged (media hashes identical).

| Sheet | Optional Config now |
| --- | --- |
| DT66,DT50, CT58 | HS7 +15; 8+128G +22. Removed 5500 +100 and 5800 +180. |
| DT610，DT630 | Entire Optional Config block removed. |
| P8100, P8100P，UPAD，U100 | Only 8+128G +22 (no HS7 / 5500 / 5800). |
| Other sheets | Unchanged. |

Vault node renamed to `shared/urovo-product-price-book-2026-7-25`. 28 Hub backlinks and three discrepancy provenance paths retargeted. Covered Hub set unchanged. Downloads original left in place (not an inbox file).

## [2026-09-11] sync | Service manuals + SR5600 user guide + KLD auth overview + 2026-07-24 price book

Inbox had 8 real inputs (plus README). Synchronized 6 document identities. Left 1. Dropped 1 byte-identical duplicate after a single copy.

| Source | Decision |
| --- | --- |
| K329_Maintenance_Service_Manual.pdf | Added `K329/others/maintenance-service-manual_202609112225`. 16/16 pages. Photos, mainboard USB pinout, disassembly, troubleshooting, gap-sensor / cover-sensor / self-test. Sample self-test SN `U21069300061R`, BT name `K329_41F1`. Not placed in `user_guide`. |
| P8100P_Service_Manual.doc (byte-identical to `P8100P Service Manual.doc`) | Added `P8100P 4G/others/service-manual_202609112225`. Body names P8100P only; routed to 4G not SQ83S 5G. 9/9 pages, 18/18 embedded images. Both inbox copies removed after one canonical original. |
| i9000S_Maintenance_Service_Manual.doc | Added `i9000S/others/maintenance-service-manual_202609112225`. 9/9 pages, 32/32 images. Battery label Model `iSDL900S` 3.8V 5000mAh (19Wh). |
| Urovo-SR5600-2D-Wearable-Ring-Barcode-Scanner-User-Manual.pdf | Added first `SR5600/user_guide/default_202609112225`. Cover [F.2021.07.12].2 / rev 2021.08.08. 49/49 pages. Not routed to SR5600 V2. |
| KLD_Mutual_Authentication_Overview.docx | Added `_shared/operations/kld-mutual-authentication-overview_202609112225`. Distinct from the 2025-07-07 KLD **operation** manual. 3/3 pages, 0 images. Backlinked six POS Hubs. |
| Urovo_Product_Price_Book-2026_7_24.xls | Added `_shared/pricing/urovo-product-price-book_202609112225`. 8 sheets, 77/77 pictures. Dated USD list; not a live spec. 28 Product Hub backlinks. Extra labels without Hubs: SR5600 Pro, S716, D9100, RFDT50. |
| RT40_Service_Manual.doc | Left in inbox. Title RT40 Service Manual v1.0 (2022-12-13). Zero RT40S/SQ47S. No RT40 Hub; GMS/MDM already treat RT40 as a model without a Hub. Not folded into RT40S. |

Vault: new shared nodes `kld-mutual-authentication-overview` and `urovo-product-price-book-2026-7-24`. Discrepancies recorded on DT66 (Android 13/15 vs spec 13.0), K329 (BT 2.1+4.2(BLE) vs spec 4.2/5.0 optional), P8100P 4G (10 Inch vs spec 10.1). Successful inbox copies removed after verification; RT40 remains.

## [2026-09-11] sync | After-sales BOMs + DT630 user-guide NFC revision

Inbox had 14 real inputs (13 after-sales BOMs + the previously left DT630 user guide). Synchronized 13. Left 1 BOM in `newly_added/` because filename and body disagree and there is no Hub. K388 Pro series spec sheet was already gone from inbox.

| Source | Decision |
| --- | --- |
| DT630 (EN)-User Guide_20251126(1).pdf | Replaced `DT630/user_guide/default_202608151554`. Same 84-page 20251126 guide. Only printed page 37 changes NFC: switching on → tag near antenna on the **back**. Screenshot chrome still says Visible as "DT610". |
| CT58 / CT58S / DT40 / DT50S / DT66 / P8100 / P8100P / i9100 BOMs | Added each product's `others/after-sales-bom_202609111450`. Not placed in `accessories/` (after-sales spare-part BOM, not an accessory brochure). |
| K388Pro_Normal(No-RFID)_… and K388Pro_RFID_… | Added two `K388 Pro/others/` slots (`after-sales-bom-no-rfid` / `after-sales-bom-rfid`). Same ILS2 quotation form; RFID workbook adds RFID antenna / RFID printer-control and mechanism PNs. |
| i9100S(SQ27L)_… and i9100S(SQ27M)_… | Routed to **i9000S** (body titles i9000S SQ27L / SQ27M). Filenames retained. Two `others/` keys. |
| DT30(SQ27L)_After_Sales_Spare_Parts_BOM-20260101.xlsx | Left in inbox. Filename says DT30/SQ27L; A1 is **SQ38组装售后组件BOM-海外通用**. No DT30 or SQ38 Hub. Not routed to i9000S. |

Visual protocol: DT630 84/84 pages; BOM unique `xl/media` files inspected per workbook (tiny placeholder pixels marked unreadable). Successful inbox copies removed after verification.

## [2026-09-11] sync | RT30 IP65 refresh + RT40S after-sales BOM + EU/NA/RFID brochures

Inbox had 9 real inputs. Synchronized 7. Left 2 in `newly_added/` (ambiguous revision). Visual protocol: RT30 spec 3/3; RT30 presentation 7/7; RT30 PB 2/2; RT40S BOM 26/26 drawings; EU 14/14; NA 14/14; RFID 8/8.

| Source | Decision |
| --- | --- |
| RT30(EN)-SPEC-20260908.pdf | Replaced `RT30/specs/default_202601010000` (20250927). Sealing **IP65** (was IP67). Adds WWAN bands and optional GNSS. Weight still 248 g. |
| RT30 Product Presentation-20250826.pptx | Replaced `RT30/presentation/product-presentation_202608111352`. Same 7-slide / 20250826 lineage; slide 7 badge **IP65**, subtitle still **IP67**. |
| RT30(EN)-PB-20250908.pptx | Replaced `RT30/brochure/default_202601010000` (was PDF). IP65, weight **240 g**, WWAN bands, optional GNSS. Source spelling `dustprof` retained. |
| RT40S(SQ47S-SQ47SP)——售后组件BOM-V1.00-20240725.xlsx | Added `RT40S/others/after-sales-bom_202609111045`. After-sales component BOM; not the accessories-brochure slot. |
| UROVO Product brochure - 20260904 (EU).pdf | Replaced `_shared/brochure/urovo-product-brochure-europe_202608301711`. Pages 1–7 and 10–14 match the prior edition at text-set level; pages 8–9 change SP35 (RFID dropped from first bullet; UWB optional) and U100. Page 5 RT30 panel still prints IP67. |
| UROVO Product brochure - 20260904 (NA).pdf | Added `_shared/brochure/urovo-product-brochure-na_202609111045`. Distinct NA mix (Irvine / us.urovo.com). No RT30 / CT58 family / DT50P Lite / U2S. |
| UROVO RFID product brochure_20260904.pdf | Added `_shared/brochure/urovo-rfid-product-brochure_202609111045`. 14 RFID-capable Product Hubs. |
| DT630 (EN)-User Guide_20251126(1).pdf | Left in inbox. Same printed date `20251126` as the current DT630 user-guide slot. NFC placement wording differs; filename `(1)` is not a later revision. |
| K388Pro PRODUCT SPEC SHEET.pdf | Left in inbox. 7 pages vs current 5-page shared series sheet (Update Date 2026-06-23). No later K388 Update Date; page 5 footer still `Model: DT610 / Update Date: 2026-07-17`. Media-width change is the same ambiguous class as a prior left-in-inbox K388 sheet. |

Vault: RT30 Hub paths updated; sealing/weight discrepancies recorded. RT40S Hub gained an others row. Replaced `shared/urovo-product-brochure-europe-20260826.md` with `...-20260904.md` and backlinked all 41 Hubs. Added NA and RFID shared nodes with Hub backlinks. Semantic pages that listed RT30 as IP67 now follow the current dedicated spec (IP65). Successful inbox copies removed after verification; DT630 guide and K388 sheet remain.

## [2026-09-10] sync | DT50S drop/tumble report + Urovo spec comparison workbook

Inbox had 2 real inputs. Synchronized both. Visual protocol: DT50S reliability PDF 5/5 pages; comparison workbook 84/84 drawings and 87/87 media files.

| Source | Decision |
| --- | --- |
| DT50S跌落及滚筒-可靠性测试报告20220901.pdf | Added `DT50S/others/drop-tumble-reliability-report_202609102000`. Internal sample SQ53S → DT50S Hub (not DT50 5G). Not placed in the single `specs/` slot (lab report, not a spec). Directed drop 150 cm / 20 cycles PASS; tumble IEC 68-2-32 method 2, 1000 mm × 400, 10/min, device off with battery, PASS. |
| Urovo_spec_comparation_241030.xlsx | Added `_shared/comparison/urovo-spec-comparison_202609102000`. New document identity vs the 2025-12-05 Battlecard. V1.1 / 241030 / Gawin Zhao. 9 sheets; 10 Product Hubs plus additional DT40S / DT50U / DT51U / DT51D / RFDT50. |

Vault: DT50S Hub gained an others row. Created `shared/urovo-spec-comparison.md` and backlinked DT50S, CT58S, DT66, CT48, RT40S, P8100-4G, P8100P-4G, P8100P-5G, DT50D, RFG91. New dated-comparison discrepancies recorded (DT50S Android 13 vs 11/13 optional; CT58S 2.0 vs 2.2 GHz; CT48 2.0 GHz source added; P8100 4G BT/drop/IP; P8100P 5G BT 5.0 vs 5.2; DT50D CPU/battery/Android/display/thickness; RFG91 5000 mAh source added). Successful inbox copies removed after verification.

## [2026-09-07] sync | CT58 presentation + DT50-Pro refresh + SP35 RFID drop + GMS/AER workbook

Inbox had 6 real inputs. Synchronized all 6. Visual protocol: CT58 9/9 slides, DT50-Pro spec 6/6 pages, DT50-Pro presentation 13/13 slides (slide 11 is a video placeholder), SP35 spec 5/5 pages, SP35 NPA 12/12 slides, GMS workbook 3/3 drawings.

| Source | Decision |
| --- | --- |
| CT58 PPT 20260901.pptx | Added empty `CT58/presentation/product-presentation_202609071236`. First presentation slot. Facts align with the current spec (Android 12, 2.0 GHz, 4+64, 5000 mAh / 12 h, BT 5.0, 13 MP PDAF, IP65, 1.5 m). New sales-deck coverage: 25° scan angle, 12-hour runtime, 4-battery charger. |
| DT50-Pro Edition Product Spec Sheet.pdf | Replaced `DT50-Pro/specs/default_202608111352`. Same printed Update Date 2026-06-30. Fact changes: Corning Gorilla Glass removed from the touch-panel row; Europe office Best → Breda. |
| DT50-Pro Edition(EN)Product Presentation20260901.pptx | Replaced `DT50-Pro/presentation/product-presentation_202608111352`. Same 13-slide lineage; display glass now **Rugged Cover Glass**. Tumble callout 0.5 m vs spec 1 m recorded on the Hub. |
| SP35 PRODUCT SPEC SHEET 20260902.pdf | Replaced `SP35/specs/default_202608301711`. Page 4 Update Date 2026-09-02; page 5 footer still 2026-08-21. Drops UHF RFID, 8+128 memory option, RFIDWedge, and the 17.64 Wh print. |
| SP35 New Product Announcement 20260902.pptx | Replaced `SP35/others/new-product-announcement_202608301711`. 12 slides (was 13); RFID slide and spec-table RFID row removed. Slide 2 still claims 8 GB RAM. |
| GMS+AER认证汇总.xlsx | Replaced `_shared/certificates/gms-aer-certification-summary_202608111723`. New 认证类型 column; SQ53Pro/DT50 Android 16 MADA ROW+EEA 2026.7.29; SQ66 A15 now SQ66V; SMR FP fingerprints; AER window column notes. |

Vault: CT58 Hub gained a presentation row. DT50-Pro Hub paths updated and now backlinks the GMS node. SP35 Hub RFID 1.2-vs-1.5 and operating-temp minus-sign notes resolved; new discrepancies are Battlecard-still-has-RFID, memory 6+64 vs 8 GB / older 8+128, Bluetooth Class 1+2 vs Class 2, and the dual spec-sheet dates. DT66 SQ66-vs-SQ66V intra-workbook label is resolved in the current workbook. Successful inbox copies removed after verification.

## [2026-08-21] sync | SP35 New Product Announcement; four inbox specs/PPT left unresolved

Inbox had 5 real inputs. Synchronized 1. Four left in `newly_added/` because revision order is not clearly newer, or printed date conflicts with the filename.

| Source | Decision |
| --- | --- |
| SP35-New-Product-Announcement-20260714.pptx | Added `SP35/others/new-product-announcement_202608211009`. 13/13 slides inspected. Not placed in `presentation/` (Battlecard already occupies that single slot; this is a different document). |
| DT610-Pro-PPT-20260612.pptx | Left in inbox. Same 17-slide product-presentation lineage as current `DT610 Pro-PPT-20260625.pptx` (revision 186 vs inbox 184). Filename and WPS revision are older. |
| K388Pro-PRODUCT-SPEC-SHEET-20260617.pdf | Left in inbox. Same series spec as `_shared/specs/k388-pro-series-product-spec-sheet_202608111352` (both Update Date 2026-06-23). Pages 1–3 and 5 pixel-identical; page 4 changes Media Width to 30–58 / 50–118 mm and K388 Pro 4 max print width to 104 mm (current slot 48 / 108 mm and 108 mm). Ordering ambiguous. |
| SP35-PRODUCT-SPEC-SHEET-20260817.pdf | Left in inbox. Same printed Update Date 2026-06-12 as current `SP35 Product Spec Sheet.pdf`. Product tables match; Europe office Best → Breda. Not treated as a later revision. |
| i9600-Dual-Screen-SPEC-20260819.pdf | Left in inbox. Filename 20260819 vs current `i9600 (EN)-SPEC-20260730`. Printed Update Date **2026-06-15** (older than 2026-07-30). Size 201×79×61 mm / 19.4 mm thinnest vs current 206×81×61 mm / 19.8 mm. |

SP35 Hub: recorded optional UHF RFID 1.2 m (spec) vs 1.5 m (NPA) and Bluetooth Class 1+2 vs Class 2. Existing memory 6+64 vs 4+64 discrepancy unchanged. Successful NPA inbox copy removed after verification.


## [2026-08-18] sync | ESL family (2.1 / 2.6 / 4.2 inch specs + F24A7 base station + EN overview)

New canonical product root `ESL/` (user-created empty folder). Synchronized 5 of 6 inbox inputs. `ESL-1.6inch-Specs.docx` left in `newly_added/` (not a valid DOCX/PDF/OLE; WeChat quarantine xattr; no PK/PDF signature). User directed this round to skip 1.6.

| Source | Slot | Notes |
| --- | --- | --- |
| ESL-Presentation-EN-0514.pptx | `presentation/overview-en_202608182031` | 22/22 slides inspected. Four sizes 1.54/2.13/2.66/4.2; F24A7-class base station; platforms. |
| ESL-2.1inch-Specs.docx | `others/spec-2.1inch_202608182031` | ET0213 v3.0 2026/2/2. Not placed in the single `specs/` slot (parallel size specs). 8/8 pages. |
| ESL-2.6inch-Specs.docx | `others/spec-2.6inch-t2664_202608182031` | T2664 2.66-inch. 3/3 pages. |
| ESL-4.2inch-Specs.docx | `others/spec-4.2inch_202608182031` | ET0420 v3.0 2026/2/2. 8/8 pages. |
| ESL_Base_Station_Specification_EN.pdf | `others/base-station-spec-en_202608182031` | F24A7. 7/7 pages. Running header still says 1.6英寸系列; body is the base station. |

Created Hub `products/ESL.md`, `spec/ESL.md`, `pb/ESL.md`, `categories/esl.md`. Portfolio 48→49 products, 11→12 categories. Active Hub discrepancies recorded (battery, IP, range, viewing angle, NFC vs Bluetooth, base-station Wi-Fi, drawing vs table size). Successful inbox copies removed; 1.6 remains.

## [2026-08-18] sync | KMS customer key-exchange instructions + KLD operation manual

Synchronized 2 inbox DOCX inputs under `_shared/operations/` (POS-wide, no market model named in the body text). Originals copied byte-for-byte. Companions preserve the text layer; every embedded image was visually inspected (KMS 1/1 cover logo; KLD 35/35 screenshots/photos).

| Source | Key | Classification |
| --- | --- | --- |
| KMS-Standard-Solution-Customer-Key-Exchange-and-KMS-Key-Loading-EN_V1.0.docx | `kms-standard-solution-key-exchange-en_202608181911` | Multi-product operations. V1.0 / 2026.7.13 / Zhang Weixiang. MK/SK (KEK components + TR-31 TMK) and DUKPT (BDK components, or ZMK + TR-31 BDK). |
| KLD_Operation_20250707.docx | `kld-operation-manual_202608181911` | Multi-product operations. Cover 2025.07.07. Master POS KLD UI + Sub-POS Sync Key / CA download. Routed to `operations` (operation manual), not a single-product `user_guide` slot. |

Created 2 shared Vault nodes and backlinked the 6 current POS Product Hubs plus the POS category Cross-Reference. index.md shared nodes 29 → 31. No same-context Hub discrepancy logged (KLD screenshot version strings differ across photos of SN `20241119152801` and are recorded in the companion only). Inbox copies removed after verification.

## [2026-08-15] sync | RFID Tag Reference (勤业/Qinye) — selection table + catalog

Synchronized 2 inbox inputs (both Chinese-language, third-party RFID tag vendor 勤业物联/Qinye, placed under new `_shared/rfid-tags/` category):

| Source | Key | Content |
| --- | --- | --- |
| 勤业-RFID电子标签应用选型表（热销款）.pdf | `rfid-tag-application-selection_202608152235` | 8-industry tag selection (鞋服/食品/3C/物流/医疗/新能源/汽车/金融) with DTB-* models, antenna/finished sizes, chips |
| 勤业-RFID电子标签（热销款）.pdf | `rfid-tag-catalog_202608152235` | Company intro + 6 tag form-factor catalogs (adhesive/woven+hangtag/flex/ABS/card/PCB) + UHF chip comparison table |

Both PDFs have complete text layers (markitdown extracted all DTB-* model numbers, dimensions, chips). "产品示意图" tag-photo column NOT transcribed (vision intermittent). Created 2 shared Vault nodes (portfolio-wide, applies to UHF readers FR1000/FR7000/RFG91/DT50P/DT50P Lite/DT610/DT610 Pro). index.md shared nodes 20 → 22.

## [2026-08-15] sync | PPTX Visual Transcription Redone (11 presentations/accessories)

Follow-up to the batch sync: re-transcribed the 11 unique PPTX companions with full slide-by-slide content (slide titles + body text + on-slide technical specifications). Rendered PPTX → PDF via LibreOffice → PNG, and (where vision cooperated) read slides visually.

**Key integrity finding:** the markitdown text-layer extraction for these PPTX files is complete and authoritative — all **accessory model codes** (BTY-/CRD-/ACC-/SH-/HS-/TRG-…) and on-slide **spec values** (i9600 6.745" 720×1600, Quad-core A53 2.0GHz, 5000/6200mAh, 80mm/s; i9200 18.5mm/343g, 3GB+32GB; etc.) are present in the extracted text and were NOT fabricated. The "Visual:" scene descriptions in companions are supplementary reconstructions (vision was intermittent during sync) and may be re-verified when vision is stable.

**New discrepancy recorded:** P8100P presentation slide 12 lists sealing as **IP65**, conflicting with the P8100P 4G spec sheet's **IP67** → logged in `P8100P-4G.md` Active Local Source Discrepancies (spec treated as authoritative).

**Sub-model note:** FR7000 presentation names the two series form factors **FR7600 (6 dBi)** and **FR7900 (9 dBi)**.

## [2026-08-15] sync | Batch User Guides, Presentations, Accessories + Software Manuals (P8100 / P8100P / FR1000 / FR7000 / i5x00 / i9x00 / 4 software manuals)

Synchronized 22 inbox inputs. All originals placed byte-for-byte (no duplicates). Companions generated via markitdown text-layer extraction — **vision was unavailable this round**, so PPTX slide imagery is NOT transcribed (each PPTX companion carries an explicit visual-content note; only extractable text layer preserved). No facts were fabricated.

**Single-product additions (18):**

| Product | New sources |
| --- | --- |
| P8100 4G | user_guide, quick-start (others), accessories (PPTX), presentation (PPTX) |
| P8100P 4G | user_guide, quick-start (others), accessories (PPTX), presentation (PPTX) |
| FR1000 | user_guide, presentation (PPTX) |
| FR7000 Series | presentation (PPTX) |
| i5300 | presentation (PPTX) |
| i5300L | presentation (PPTX) |
| i9100 | quick-start (user_guide), presentation (PPTX) |
| i9200 | financial presentation (presentation slot), non-financial presentation (others) |
| i9600 | presentation (PPTX) |

Routing notes: `P8100` → `P8100 4G` (SQ81A, 8-inch); `P8100P` → `P8100P 4G` (SQ83A, 10.1-inch — confirmed "supports 4G networks" in the guide text). Quick-start guides routed to `others/` where a full user guide already occupies the single `user_guide` slot. i9200 financial vs non-financial variants kept separate.

**Multi-product software manuals (4, under `_shared/operations/`):** RFID-Demo (V25), RFIDWedge (V21), Scan-Settings, and 扫描数据高级格式化说明 (v1.0.1). Created 4 shared Vault nodes (platform-wide, no per-product backlinks), added to index.md shared catalog (16 → 20 nodes).

Updated 9 Product Hubs (Current Source Coverage). No new same-context factual discrepancies surfaced. Note: FR1000 user guide internal version is `20230522v1.0` while the filename carries `20260707`; retained filename, no discrepancy logged (internal version vs file date is not a factual conflict).

## [2026-08-15] repair | Batch Rewrite of Lossy Baseline Spec Companions Round 4 (RFG91 / U2S / FR7000 Series / K180)

Fourth batch of baseline `default_202601010000` lossy spec rewrites per SYNC_PROMPT.md §3.3 (semantically lossless) + §10 (correction in place, preserve original, no new slot).

| Companion | Pages | Before | After |
| --- | --- | --- | --- |
| RFG91 spec | 4 | 38 lines | 189 lines (full 4 form factors + 8 Highlights + Physical incl 3.6V/USB/Notification/Keypad & Button/Voice & Audio/User Env incl Tumble/IP54→IP67/ESD + Wireless PAN BT 5.0+NFC pair/Sensor + RFID Performance full bands + Accessories with 5 cradle variants + Industry 5 segments) |
| U2S spec | 2 | 46 lines | 69 lines (full Performance/Basic incl F1/F2/Menu/Home/Return/Power buttons + Sensors + Audio + Interface + Charging time + NFC Forum 1-5 + Communication WLAN tri-band + Env incl storage temp/humidity/tumble/ESD) |
| FR7000 Series spec | 4 | 45 lines | 132 lines (full Models 6dBi/9dBi + RFID E710 detail + Power Supply min/typical/max table + Power Connector + RS232/DB9 + RS485 + Wiegand + 4-Output Relay + 3-Input + Cables + Physical with M5 mounting + Accessories) |
| K180 spec | 3 | 46 lines | 82 lines (full Scanning Performance + Physical incl 2500mAh battery + Wireless BT 5.2 freq 2.4GHz + 80m range + HID port + 1MByte storage + <3h charging + >20h work + Accessories charging stand + Bluetooth receiver + supported languages) |

All 4 PDFs preserved (SHA-256 verified unchanged); same `default_202601010000` slot, no new slots created. No new PDF-internal contradictions surfaced (no new discrepancy rows added to product Hubs).

## [2026-08-15] repair | Batch Rewrite of Lossy Baseline Spec Companions Round 3 (P8100P 5G / P8100P 4G / P8100 4G / DT66)

Third batch of baseline `default_202601010000` lossy spec rewrites per SYNC_PROMPT.md §3.3 (semantically lossless) + §10 (correction in place, preserve original, no new slot). Rendered each PDF via pypdfium2, read every page visually, transcribed with full spec tables and page provenance.

| Companion | Pages | Before | After |
| --- | --- | --- | --- |
| P8100P 5G spec | 4 | 46 lines | 163 lines (full Performance/Physical+Audio/Sensors/Slots/Interfaces/Network/Environment + Data Capture Camera/Scanner/RFID HF + Positioning + Wireless LAN/WAN bands ROW / PAN / Accessories) |
| P8100P 4G spec | 4 | 59 lines | 159 lines (full same structure as P8100P 5G with 4G band tables) |
| P8100 4G spec | 4 | 65 lines | 165 lines (full 8-inch tablet spec with P1–P8 keys, fingerprint, ESD, full LTE/WCDMA bands, accessories) |
| DT66 spec | 5 | 107 lines | 181 lines (full Performance/Physical/Power+Charger+Hot Swap/Network/Data Capture Camera+Scanner+RFID HF/Wireless LAN/WAN Europe&Asia + North America bands/PAN/Accessories Standard+Optional) |

All 4 PDFs preserved (SHA-256 verified unchanged); same `default_202601010000` slot, no new slots created. No new PDF-internal contradictions surfaced (no new discrepancy rows added to product Hubs).

## [2026-08-15] repair | Batch Rewrite of Lossy Baseline Spec Companions Round 2 (K389/DT610 Pro/K388 Pro/S710/i5300L/i5300)

Second batch of baseline `default_202601010000` lossy spec rewrites per SYNC_PROMPT.md §3.3 (semantically lossless) + §10 (correction in place, preserve original, no new slot). Rendered each PDF via pypdfium2, read every page visually, transcribed with full spec tables and page provenance.

| Companion | Pages | Before | After |
| --- | --- | --- | --- |
| K389 spec | 5 | 38 lines | 213 lines (full Performance/Physical/Printer/Barcode/Programming/Fonts/WLAN/PAN/Sensor/Media/User Environment/Other/Accessories/Industry) |
| DT610 Pro spec | 6 | 83 lines | 305 lines (full 14 Highlights + Performance/Physical/WWAN World+NA bands/WLAN full data rates/PAN/Data Capture/User Environment/Software/Accessories/Industry) |
| K388 Pro spec | 4 | 64 lines | 159 lines (full Performance/Physical/Network incl NFC+UHF/Printing/Data Capture Camera+Scan Engine+RFID HF+RFID UHF/Positioning/WLAN/Accessories) |
| S710 spec | 2 | 39 lines | 70 lines (full Basic characteristics incl OS/Processor/Camera/Viewing/Decode/Reading Distance/Power/Interfaces/Environmental) |
| i5300L spec | 3 | 55 lines | 122 lines (full OS/Processor/Memory/Display/Button/Network/Camera/Scanning/Payment/Thermal Printer/Audio/Positioning/Slot/Interface/Notification LED/Battery/Adaptor/Environment/Physical/Certification) |
| i5300 spec | 2 | 55 lines | 119 lines (full, same structure as i5300L with 3.5" display, 16-key keyboard, top camera w/ flash, 5V/1A adapter, certification inline) |

All 6 PDFs preserved (SHA-256 verified unchanged); same `default_202601010000` slot, no new slots created. No new PDF-internal contradictions surfaced (no new discrepancy rows added to product Hubs).

## [2026-08-15] repair | Batch Rewrite of Lossy Baseline Spec Companions (UPad/RT40S/RT30/K220)

Following the audit that confirmed 7 lossy baseline companions (all `default_202601010000` slots), rewrote the 4 confirmed-lossy **spec sheets** in place per SYNC_PROMPT.md §3.3 (semantically lossless) + §10 (correction to existing companion, preserve original, no new slot):

| Companion | Pages | Before | After |
| --- | --- | --- | --- |
| UPad spec | 5 | 41 lines | 277 lines, full Performance/Physical/WWAN/WLAN/WPAN/Data Capture/User Environment/Software/Accessories/Contact |
| RT40S spec | 5 | 47 lines | 156 lines, full Performance/Basic (incl. keyboard detail, PTT)/Communication/Environment + Data Capture (Camera, 2 scan engines, HF RFID)/Data Transfer (GNSS detail, WLAN with channels, WWAN bands)/PAN/Accessories |
| RT30 spec | 2 | 48 lines | 70 lines, full Performance/Basic (incl. button detail, Audio, Card Slot)/NFC/Communication/Environment |
| K220 spec | 4 | 53 lines | 105 lines, full Scanning Performance/Decode/Depth of Field/Physical/Environmental/Wireless (incl. BT5.0/BLE, 3200mA battery, <4h charging)/Accessories (SBC220 cradle, 5V2A adapter) |

All 4 PDFs preserved (SHA-256 verified unchanged); same `default_202601010000` slot, no new slots created. Audit findings + repair logged in workspace memory.

## [2026-08-15] repair | DT630 Spec Sheet Companion → Semantically Lossless

The historical-baseline companion `DT630/specs/default_202601010000/DT630 Product Spec Sheet.md` was a lossy paraphrase (omitted dimensions, 8 GB RAM / 128 GB ROM, front 8 MP camera, full cellular band tables, Wi-Fi/Bluetooth detail, NFC, voltage, accessories, environment specs, industry list) and silently chose one side of two PDF-internal contradictions (Android 19 vs 20, RFID 1.2 m vs 1.5 m). Per SYNC_PROMPT.md "semantically lossless" rule and the "no silent winner" discrepancy rule, rewrote the companion in place to cover all 6 PDF pages faithfully. Original PDF preserved (bytes unchanged); same `default_202601010000` slot, no new slot created. Surfaced two intra-source contradictions in DT630 Hub Active Local Source Discrepancies (Android upgrade target, RFID read range).

### Added
- Synchronized two new multi-product `operations` sources under `_shared/operations/` with byte-preserved originals and same-stem companions:
  - `urovo-oemconfig-manual_202608151815/Urovo-OEMConfig-Manual.pdf` (SHA-256 `4cdd9b7dae…`) — Urovo OEMConfig 1.0 user manual (2023-03-17) documenting all configuration groups, actions, and items (Clock, Display, NFC, FOTA, General UI, KeyRemap, Power, Wireless General, WLAN, WlanAdvanced, Scanner, Device Management).
  - `soti-oemconfig-guide_202608151815/SOTI-OEMConfig-guide.docx` (SHA-256 `3e15779b1a…`) — Chinese step-by-step SOTI MobiControl + Urovo OEMConfig deployment guide (4 steps, 7 embedded screenshots preserved in the original).
- Added two shared Vault nodes (`shared/urovo-oemconfig-manual.md`, `shared/soti-oemconfig-guide.md`) and registered both in `index.md` Shared Knowledge Sources (16 shared nodes, 180 total pages).
- Cross-linked both nodes from the MDM certification summary node.

### Classification and Routing Decisions
- Both documents are platform-wide operational references (the UrovoOEMConfig app applies to the UROVO Android portfolio as a whole), not product-specific. They therefore link no individual Product Hub; scope is documented as portfolio-wide with cross-references to the MDM certification summary and between the two OEMConfig sources.
- The OEMConfig manual's EA630/PA760 programmable-key names are illustrative examples, not claims about current product coverage, and were recorded as such.

### Conflict Review
- No new same-context contradiction was identified. The SOTI guide's OEMConfig version 1.3.42 is time-of-writing evidence, not a current-version claim.

### Validation
- Original and synchronized SHA-256 hashes match for both sources.
- Shared nodes, index.md catalog entries, and MDM cross-references resolve.

## [2026-08-15] sync | GMS Certification Reuse (套用) Statistics

### Added
- Synchronized `GMS认证套用统计.xlsx` as a new multi-product `certificates` source under `_shared/certificates/gms-certification-reuse-statistics_202608151804/`, preserving the original workbook byte-for-byte (SHA-256 `89c3eb760275f013b91da7d666662bee2fd2b18b033dc8cd35246f660689b0e1`).
- Generated a same-stem, coordinate-preserving Markdown companion: 1 sheet (工作表2), 29 non-empty cells, 10 merged ranges, no formulas/comments/hyperlinks/drawings. Merged-cell values (认证型号 ro.product.device and 内部型号) are propagated to every row for unambiguous retrieval.
- Added the `GMS Certification Reuse Statistics` shared Vault node (`shared/gms-certification-reuse-statistics.md`) and backlinks from 15 covered Product Hubs (CT48, CT48C, CT58, CT58C, CT58S, DT40, i9000S, i9100, i5300, i5300L, i9200, i9600, P8100 4G, P8100P 4G, RT30).
- Added the shared source to the `index.md` Shared Knowledge Sources table and bumped the shared-node count to 14 (178 total pages).

### Classification and Routing Decisions
- The workbook records which internal models reuse (套用) the GMS certification of a base certified model, keyed by `ro.product.device`, with the internal model and application time. Five reuse groups: SQ57 (→ SQ29M/MB/MR, SQ27M, SQ65B/F, SQ45C, SQ53X, SQ52M), i9100/SQ29MB (→ SQ68 series, SQ69PC/D/DM/KB), DT50_5G/SQ53B (→ SQ48C, SQ58C, SQ48, SQ58 A12), P8100/SQ81 (→ SQ83), and CT58S/SQ58S (→ SQ310 A14, SQ48CU A14, SQ58CU A14).
- Routed SQ48 → CT48, SQ48C → CT48C, SQ58 A12 → CT58, SQ58C → CT58C, SQ58S → CT58S, SQ45C → DT40, SQ27M → i9000S, SQ29M/MB/MR → i9100, SQ65B → i5300, SQ65F → i5300L, SQ68 → i9200, SQ69PC/D/DM/KB → i9600, SQ81 → P8100 4G, SQ83 → P8100P 4G, SQ310 → RT30. SQ57, SQ53X, SQ52M, DT50 5G/SQ53B, SQ48CU A14, and SQ58CU A14 have no canonical Hub and are recorded as additional models.

### Conflict Review
- No new same-context contradiction with the existing GMS+AER certification summary was found; the reuse relationships are consistent with that workbook's project-level records. The "A12"/"A14" suffixes on reusing models denote the Android version of each project and are treated as contextual qualifiers rather than universal claims.

### Validation
- Original and synchronized workbook SHA-256 hashes match.
- Shared node, 15 Hub backlinks, and the index.md catalog entry all resolve.
- No single-product source slot was changed; this is an additive shared source only.

## [2026-08-15] repair | Full-Text and Visual Companion Recovery

### Repaired
- Rebuilt eight lossy long-form user-guide companions as complete page-by-page transcriptions covering all **642** source pages: CT58, DT50-Pro, DT50D, DT50P, DT66, RFG91, RT30, and RT40S.
- Preserved the complete native PDF text layer in source-page order and rendered every page for OCR inspection. Added reviewed visual labels only where image-dominant pages contained useful text not present in the native layer.
- Restored the exact CT58 SD/SIM installation steps and ESD warning that had previously been replaced by a generic procedure summary.
- Added the visually rendered **≈390 g** RFG91 weight and **498 g** DT50P Lite weight to their presentation companions.
- Replaced the DT66 Dust Plugs placeholder with a description of the pictured tethered/lanyard-style plug.
- Removed `see original`, `standard procedure`, and `standard settings` omission shortcuts from the repaired scope.

### Source Integrity and Validation
- Original PDF and PPTX files were not modified. The repair workflow asserted unchanged PDF SHA-256 values before and after each companion rewrite.
- All eight rebuilt guides have a consecutive `### Page N` section and one native-text block for every source page; normalized native-text coverage is **100%** for each guide.
- The three targeted presentation/accessories omissions were rechecked against their rendered sources.
- Product Hub paths and single-slot routing were unchanged.

## [2026-08-15] sync | DT50D / DT50P / DT50P Lite / RFG91 Guides, Accessories, and Presentations

### Added
- Synchronized ten new single-product sources as `default_202608151705` (or `quick-start-guide_202608151705`) slots, each preserving the original bytes with a same-stem structured Markdown companion:
  - `DT50D/user_guide/` — DT50D Mobile Computer User Guide (2023-07-25; older template; battery 5000 mAh; UHF RFID app).
  - `DT50D/others/quick-start-guide_…` — DT50D Quick Start Guide (v3.01.200.10054).
  - `DT50P/user_guide/` — DT50P Mobile Computer User Guide (2023-07-25; battery 9000 mAh).
  - `DT50P/others/quick-start-guide_…` — DT50P Quick Start Guide (image-only, 2 pages, no text layer; companion records metadata).
  - `DT50P Lite/user_guide/` — DT50P Lite Quick Start Guide (v3.01.200.12492; cover labeled DT50U Lite / DT50P Lite; handle + RFID reader antenna).
  - `DT50P Lite/presentation/` — DT50P Lite Product Presentation (Impinj E710, 15 m+, 1300+ tags/sec, 6500 mAh).
  - `RFG91/user_guide/` — RFG91 UHF RFID Sled User Manual (V2.1, 2025-12-15; Bluetooth + Pogo versions; holds a DT610).
  - `RFG91/others/quick-start-guide_…` — RFG91 Quick Start Guide (v3.01.200.12482; source text layer has doubled characters, de-duplicated in the companion).
  - `RFG91/accessories/` — RFG91 Accessories Guide (standard 4900 mAh / extended 6700 mAh; cradles; mounts; wrist strip).
  - `RFG91/presentation/` — RFG91 Product Introduction Presentation (2025-02-21; Impinj E710 + Gen2X, 1300+ tags/sec, 15 m+).
- Added the new sources to the DT50D, DT50P, DT50P Lite, and RFG91 Product Hub coverage tables.

### Classification and Routing Decisions
- DT50D/DT50P full user guides hold the single `user_guide` slot; their quick-start guides sit under `others/quick-start-guide_…`. DT50P Lite's quick-start guide is its only user-guide-type source, so it holds the `user_guide` slot.
- RFG91 is a UHF RFID sled that mounts a DT610/DT610 Pro; all RFG91 sources are single-product (the sled) and were routed under `RFG91/`.

### Conflict Review
- Updated the existing RFG91 standard-battery discrepancy: the new presentation corroborates 5000 mAh while the new accessories guide corroborates 4900 mAh / 18 Wh; both new source paths were added to the discrepancy row. The optional 6700 mAh value agrees across sources.
- No new discrepancy elsewhere: DT50D (5000 mAh), DT50P (9000 mAh), and DT50P Lite (6500 mAh) guide/presentation facts agree with their spec pages.

### Validation
- Single-slot layout verified for all four products.
- All twenty synchronized original/Markdown pairs resolve.
- No wiki pages were renamed, so existing wiki links remain valid.

## [2026-08-15] sync | Batch User Guides and Accessories (CT58/DT40/DT50-Pro/DT66/RT30/RT40S)

### Added
- Synchronized ten new single-product sources as `default_202608151629` slots, each preserving the original bytes with a same-stem structured Markdown companion:
  - `CT58/user_guide/` — CT58 Mobile Computer User Guide (2023-10-19; older template with a Technical Specifications section: Android 12, octa-core 2.0 GHz, 265 g, IP65, 5000 mAh, BT5.0, 4G).
  - `CT58/accessories/` — CT58 Accessories Brochure (2023-12-01).
  - `DT40/user_guide/` — DT40 Quick Start Guide (v3.01.200.10028; keypad + NFC).
  - `DT40/accessories/` — DT40 Accessories Brochure (2025-08-06 PPTX; battery 4500 mAh, BTY-DT40-45-* models).
  - `DT50-Pro/user_guide/` — DT50 Pro Mobile Computer User Guide (source body labeled DT50/DT50Pro; battery HB50DT50; 4G; NFC; gloves mode).
  - `DT66/accessories/` — DT66 Accessories Guide (2025-09-15; CRD-DT66-* cradle models, BTY-DT66-02 battery, vehicle mount CAK-DT66-01).
  - `DT66/user_guide/` — DT66 Mobile Computer User Guide (2025-01-16; battery HB50DT66, 5G, hot-swap 60 s, NFC, gloves mode).
  - `RT30/user_guide/` — RT30 Handheld Intelligent Terminal User Guide (2025-08-01; battery NB49RT30, hot-swap, NFC, gloves mode).
  - `RT40S/user_guide/` — RT40S Mobile Computer User Guide (2024-02-05; older template with 29/38/51-key keypad variants, SHIFT/Orange/Blue function keys; 4G).
  - `RT40S/accessories/` — RT40S Accessories Brochure (2025-08-06; battery 5200 mAh, BTY-RT40S-52-* models).
- Added the new sources to the CT58, DT40, DT50-Pro, DT66, RT30, and RT40S Product Hub coverage tables.

### Duplicates Removed (inbox only)
- `DT50-Pro_Accessories_Guide.pdf` and `DT50S_Accessories_Guide.pdf` were both byte-identical (md5 `f0dd44ae…`) to the existing shared `_shared/accessories/dt50-series-accessories-guide_202608111352/DT50 Series Accessories Guide.pdf`. Removed without creating redundant single-product accessories slots.

### Classification and Routing Decisions
- Routed the DT50-Pro user guide to `DT50-Pro/user_guide/` per its filename and internal "DT50Pro" references; it is 4G (SQ53Pro) and distinct from DT50S (SQ53S/SQ53ST) and the separate "DT50 5G" (SQ53B/SQ53BV) lineage.
- The CT58 files reference only the base CT58 model (zero CT58C/CT58S mentions), so they are single-product CT58 sources.

### Conflict Review
- Recorded a new RT30 network-generation discrepancy: the 2025 guide's status-icon reference table lists a "5G network" icon, while the RT30 specification and internal SQ310 mapping both list 4G/3G/2G only. Treated the guide icon as a generic template; the spec remains authoritative for hard-spec answers.
- No other new discrepancy: CT58 (Android 12, 2.0 GHz, 265 g, IP65, 5000 mAh), DT40 (4500 mAh), DT50-Pro (HB50DT50), DT66 (HB50DT66, 5G), and RT40S (4G) guide facts all agree with their spec pages.
- Enriched the DT50-Pro, DT66, and RT30 spec pages with the newly sourced battery model numbers (HB50DT50, HB50DT66, NB49RT30).

### Validation
- Single-slot layout verified for all six products (each single-slot parent holds at most one document directory).
- All twenty synchronized original/Markdown pairs resolve.
- No wiki pages were renamed, so existing wiki links remain valid.

## [2026-08-15] sync | Batch User Guides and Inbox Dedup

### Added
- Synchronized five new single-product user guides as `default_202608151554` (or `quick-start-guide_202608151554`) sources, each preserving the original PDF byte-for-byte with a same-stem structured Markdown companion:
  - `CT58S/user_guide/default_202608151554/` — CT58S Mobile Computer User Guide (2024-11-19, 60 pages).
  - `DT50S/user_guide/default_202608151554/` — DT50 Mobile Computer User Guide (2023-04-20), routed to the canonical DT50S 4G lineage (source labeled DT50; confirms 4G WWAN, 5000 mAh battery, UHF gun-grip accessory).
  - `DT50S/others/quick-start-guide_202608151554/` — DT50S Quick Start Guide (cover labeled DT50, version 3.01.200.10070 V1.1). Placed under `others/` because the `user_guide` single slot is held by the full DT50 user guide.
  - `DT610/user_guide/default_202608151554/` — DT610 (STD) Mobile Computer User Guide (2025-09-19, 87 pages; battery HB40DT610, hot-swap 60 s, RFID 1.5 m/50 tags/sec).
  - `DT630/user_guide/default_202608151554/` — DT630 Mobile Computer User Guide (2025-11-26, 80 pages; battery HB45DT630, 5G, RFID 1.2 m/50 tags/sec, NFC, gloves mode).
- Added the new sources to the CT58S, DT50S, DT610, and DT630 Product Hub coverage tables.

### Duplicates Removed (inbox only)
- `SP35_Battlecard.pptx`, `DT630_Accessories_Guide.pdf`, `DT610_Accessories_Guide.pdf`, and `DT610-Pro_Accessories_Guide.pdf` were byte-identical to existing synchronized originals; removed without altering any slot.

### Classification and Routing Decisions
- Normalized a non-breaking space in the DT610 filename `DT610(STD)-User<NBSP>Guide_20250919.pdf` to a regular space for the canonical copy; content bytes are unchanged.
- Routed the retained DT50 guide to DT50S per the canonical identity override; kept the source-specific DT50 label as provenance.
- The DT50S Quick Start Guide is a secondary `user_guide`-type document; the full DT50 user guide remains the primary `user_guide` slot and the quick start sits under `others/`.

### Conflict Review
- No new same-context discrepancy was found. Guide facts are consistent with existing specifications: DT630 RFID 1.2 m/50 tags/sec, DT610 RFID 1.5 m/50 tags/sec, and DT50S 5000 mAh battery all match the spec pages.
- Enriched the DT610, DT630, and DT50S spec pages with the newly sourced battery model numbers (HB40DT610, HB45DT630) and the DT50S UHF gun-grip accessory specs (up to 8 m, >200 labels/sec, 3000 mAh battery).

### Unresolved Inbox
- `CT58C(EN)-User Guide-20241119 copy.pdf` remains in `newly_added/`. It is byte-identical to the CT58S user guide and its content mentions CT58S 33 times with zero CT58C references, so it is a mislabeled copy, not a genuine CT58C document. Left in the inbox pending a correct CT58C original.

### Validation
- Single-slot layout verified (each `brochure/specs/user_guide/presentation/accessories` parent holds at most one document directory; `others` holds two for DT50S as allowed).
- All ten synchronized original/Markdown pairs resolve; original PDFs preserved with SHA-256 hashes `5bf370c0…` (CT58S), `d36c07db…` (DT50), `4a0223d1…` (DT50S QS), `783afc35…` (DT610), `5c27554b…` (DT630).
- No wiki pages were renamed, so existing wiki links remain valid.

## [2026-08-15] sync | SR5750 Companion Repair and U2S User Guide

### Corrected
- Detected that the inbox `SR5750 Product Spec Sheet.pdf` is byte-identical to the retained canonical PDF, so the original source and its existing `default_202601010000` slot were preserved rather than creating a false revision.
- Rebuilt the same-stem SR5750 Markdown companion in place because the previous companion omitted most source content and incorrectly stated a 2.06-inch display; the retained PDF specifies a 2.1-inch 410×502 AMOLED display.
- Restored the complete SR5750 narrative and specifications, including wireless protocols/security, scanner options, NFC, environmental tests, software, accessories, applications, and contact details.
- Updated the SR5750 spec/PB/category/connectivity/durability/synthesis knowledge. Corrected its battery grouping to 1150 mAh non-removable and added its Wi-Fi 6 and 1.8 m drop facts.

### Added
- Synchronized the 75-page `U2S (EN)-User Guide_20250703.pdf` as the new single-product `U2S/user_guide/default_202608151537/` source without changing its bytes.
- Generated a structured same-stem Markdown companion covering device controls, HBLU2 battery safety and 60-second hot swap, Android operation/settings, enterprise features, wrist strap, camera, application catalog, U Stage, maintenance, troubleshooting, factory reset, warranty, and support information.
- Added the guide to the U2S Product Hub and added operational facts to the U2S specification page.

### Conflict Review
- Kept the existing U2S battery, sealing, camera, and scan-engine warnings active.
- Expanded the camera warning because the 2025 guide's Camera UI instructs front/rear switching, while the 2026 product specification says top 13 MP, the brochure says rear 13 MP, and the dated Battlecard says side 13 MP.
- Treated the guide's Battery Management screenshot values, including 5430 mAh present capacity, as sample UI rather than a product specification because the guide explicitly says screens and available features may vary by model and operating-system version.

### Validation
- Preserved original SHA-256 hashes `f20476498b29970ddc52fc415d6bd678a9283c1f15c125985bb586ecc4e538c3` (SR5750) and `02db5cfd900aeed76dc90e9e94079a33cb79302422cbe57adab8308ea4776081` (U2S user guide).
- Rendered and reviewed all 75 U2S guide pages; affected original/Markdown pairs, single-slot layout, hard-fact coverage, and Product Hub coverage passed.
- Skill package validation passed; the Vault audit checked 1,168 Wiki links with zero broken targets.

## [2026-06-02] build | Product Knowledge Vault — Construction Complete

### Final Deliverables
- **112 wiki pages** (~6,100+ lines) across 10 directories
- **44 spec pages** — one per product with structured specifications
- **46 brochure pages** — marketing content, features, and positioning per product
- **7 category overviews** — handheld terminals, enterprise smartphones, POS, barcode scanners, mobile printers, desktop printers & fixed RFID, other devices
- **3 comparison pages** — CT series, DT series, Enterprise Smartphone comparison
- **3 feature pages** — Connectivity evolution, Durability tiers, RFID capabilities
- **2 entity pages** — Impinj E710, Qualcomm Q-6690
- **2 technology pages** — Wi-Fi 7, UHF RFID technology
- **5 core pages** — index.md, overview.md, synthesis.md, CLAUDE.md, log.md
- **1 matrix** — Performance comparison across 25 products
- **All directories populated**: comparisons/, entity/, features/, matrices/, pb/, spec/, technology/, categories/

### Compliance Check
- CLAUDE.md schema fully implemented
- Wiki interlinks verified across entity→spec→pb→comparison chains
- index.md serves as navigable catalog listing all 112 pages
- Sources remain immutable (46 original product folders untouched)

## [2026-06-02] review | Quality Audit Pass
- Found & fixed: SR5600 missing PB page → created
- Found & fixed: features/ directory empty → added connectivity, durability, RFID pages  
- Found & fixed: DT610 Pro spec missing Overview/Key Differentiators → added
- Found & fixed: index.md outdated counts → refreshed to 112 pages

## [2026-06-03] structure | Official Web Source Layer Added

### Changes
- Added `web-source.md` with 46 product rows and verified official UROVO web URLs where available.
- Added official-web conflict workflow files: `sync/web_conflicts.json`, root-level `WEB_VS_LOCAL_CONFLICTS.md`, and root-level `USER_JUDGMENT_NEEDED.md`.
- Updated `SCHEMA.md` and `SYNC_INSTRUCTION.md` with web-source, conflict, user-judgment, and wiki-link audit rules.
- Fixed deterministic broken wiki links caused by renamed schema/category/spec targets.

### Verification
- Wiki link scan: 566 links, 0 broken.
- Official web source table: 46 products, 36 filled URLs, 10 blank URLs with no verified official page found.
- Vault count updated to 114 markdown pages.

## [2026-08-11] structure | Timestamped Sources and Simple Inbox Sync

### Changes
- Moved 82 historical original documents and their 82 same-stem Markdown companions into 82 product-level document slots using the baseline timestamp `202601010000`.
- Preserved the financial/non-financial variants for i9200 and separated the R70/R71 ring-scanner brochure that had been misfiled under K329 into the `R7` product directory.
- Added `newly_added/` as a non-authoritative document inbox and `SYNC_PROMPT.md` as the only explicit maintenance workflow.
- Retired the source-manifest checker workflow; routine sync now inspects inbox files and current product directories directly.
- Updated source discovery, provenance, and Vault maintenance rules for timestamped paths.

### Invariants
- Normal Q&A remains read-only and ignores `newly_added/`.
- Every synchronized source slot contains one unchanged original plus one same-stem Markdown companion.
- The baseline timestamp records this directory migration and is not a source publication date.

## [2026-08-11] cleanup | Source Special Cases and Extracted Images

### Changes
- Removed 1,066 extracted JPG/PNG artifacts (58,079,591 bytes) and all resulting empty product-level `images/` directories. Original PDF/PPTX documents remain available for visual verification.
- Updated sync guidance so future conversions do not extract or store page images.
- Aligned all i9200 references with the `financial` and `non_financial` slot names.
- Added the R7 (R70/R71) brochure page and barcode-scanner index entry without inferring specifications absent from the source.
- Aligned the reclassified R7 source pair and Vault provenance with the current `R7-PB.pdf` / `R7-PB.md` filenames.
- Removed legacy WorkBuddy state, ignored historical output artifacts, macOS `.DS_Store` files, and the empty root-level human conflict/judgment files. `sync/web_conflicts.json` remains the only optional structured conflict record.
- Removed a partial duplicate brochure index, moved i5300/i5300L into the POS specification section, documented overlapping SR5750 categories, and corrected the barcode-scanner count to eight.
- Removed the obsolete `outputs` ignore rule so future misplaced Skill-local deliverables are visible in Git status.
- Retired the Web-vs-local layer completely: removed `web-source.md`, `sync/web_conflicts.json`, and the empty `sync/` directory. Product answers and maintenance now use only synchronized local source documents and their Vault summaries.

## [2026-08-11] structure | Canonical Types and Exhaustive Product Hubs

### Changes
- Migrated all 82 source slots to `<product>/<canonical-type>/<document-key>_<timestamp>/` without changing the 164 source/Markdown file contents.
- Restricted product roots to `brochure`, `specs`, `user_guide`, `presentation`, `accessories`, and `others`; the first five allow one current document while `others` allows multiple.
- Kept i9200 financial sources as the primary specs/brochure and moved its additional non-financial sources under `others`.
- Added `_shared/` for all multi-product originals and `shared/` Vault nodes for graph integration.
- Added 47 exhaustive product Hubs covering all 82 current sources, plus backlinks from all 44 spec and 47 PB pages.
- Changed Query routing to complete discovery through product Hubs followed by selective source loading; broad requests read every listed source.
- Added sync-time local discrepancy detection and product-Hub warnings so Query surfaces conflicting local values.

### Invariants
- Every source document directory has exactly one original and one same-stem Markdown.
- Every current product source appears exactly once in its product Hub.
- Multi-product sources must have a shared Vault node and backlinks from every covered product Hub.

## [2026-08-11] sync | First Multi-Product Shared Sources

### Added
- Synchronized `i9000S_i9100_internal_projects_main_diff-20250509.xlsx` as `_shared/comparison/i9000s-i9100-internal-project-differences_202608111226/`.
- Synchronized `Device_and_Accessories_Guide_20260810.xlsx` as `_shared/accessories/device-and-accessories-guide_202608111226/`.
- Preserved both original workbooks byte-for-byte and generated same-stem, coordinate-preserving Markdown companions.
- Added two shared Vault nodes and backlinks from 34 affected Product Hubs; i9000S and i9100 link both sources.
- Added the shared source catalog to `index.md`.

### Conflict Review
- Recorded unresolved CT58 CPU difference: 2.2 GHz in the shared guide versus 2.0 GHz in the product specification.
- Recorded unresolved K388 Pro Bluetooth difference: BT 5.0 in the shared guide versus BT 5.3 in the product specification.
- Recorded unresolved RFG91 standard battery difference: 5000 mAh in the shared guide versus 4900 mAh / 18 Wh in the product specification.
- Treated project, market, lifecycle, option, and adapter-form differences as contextual rather than silently merging them.

### Validation
- 39 sheets and 4,292 non-empty cells transcribed; no formulas or comments were present.
- The device/accessory workbook's 279 drawing anchors and external printer hyperlink were preserved as Markdown metadata while all visual assets remain in the unchanged original.
- Original and synchronized workbook SHA-256 hashes match.

## [2026-08-11] sync | Batch PDF and PowerPoint Refresh

### Source Changes
- Synchronized 21 current documents: 6 single-product replacements, 12 new single-product sources, and 3 new multi-product shared sources.
- Replaced CT48C specs, DT50-Pro specs, FR1000 specs, FR2000 brochure, i5300L brochure, and i9600 specs after confirming substantive content changes.
- Added product presentations for CT48C, DT50-Pro, DT610, DT610 Pro, RT30, and i5300L; added DT610 / DT610 Pro / DT630 accessory guides; added the DT610 Pro user guide; and created SP35 specs plus battlecard sources.
- Added shared nodes for the DT50 Series Accessories Guide, DT610 Std/Pro Product Spec Sheet, and K388 Pro Series Product Spec Sheet.
- Preserved every synchronized PDF/PPTX byte-for-byte and created a same-stem Markdown companion. The 90-page DT610 Pro user guide and every slide in each synchronized deck were extracted and visually sampled or reviewed.

### Same-Batch Version Selection
- Selected `DT50-Pro Edition(EN)Product Presentation20260630.pptx` over the same-lineage 2026-05-13 deck based on the explicit later date and changed Android, memory, NFC, and accessory content.
- Detected that all three DT610 Pro 2026-06-25 PPTX inputs were byte-identical and synchronized only one copy.
- Removed exact duplicate inbox copies for the existing RT30 brochure/specs and i5300 brochure/specs without altering their current slots.
- Clarified `SYNC_PROMPT.md` so every sync groups same-lineage inbox candidates before choosing the newest revision.

### Conflict Review
- Recorded CT48C weight as unresolved: 268 g with standard battery in specs/brochure versus an unqualified 252 g in the presentation.
- Recorded DT610 Pro battery capacity as unresolved: 5500 mAh in product-specific specs/accessories versus 5200 mAh in the newer shared DT610 series sheet.
- Kept the K388 Pro Bluetooth discrepancy active; the new series spec corroborates BT 5.3 while the device/accessory guide states BT 5.0.

### Validation
- Canonical source/Hubs test: 2 passed.
- Wiki-link audit: 951 links, 0 broken.
- Vault inventory: 169 Markdown pages, 48 Product Hubs, 5 shared nodes, 45 spec pages, and 48 brochure/product pages.

## [2026-08-11] sync | POS Certification Status Workbook

### Added
- Synchronized `pos-certificates.xlsx` as `_shared/certificates/pos-certificates_202608111641/` without changing the original workbook bytes.
- Generated a same-stem, coordinate-preserving Markdown companion covering all 18 worksheets and normalized true Excel date values to ISO 8601 for unambiguous retrieval.
- Added the `POS Certificates and Firmware Validity` shared Vault node and backlinks from i5300, i5300L, i9000S, i9100, i9200, and i9600 Product Hubs.
- Linked the POS category page to the dated certification source and clarified that model-level certification families do not establish current validity for every project or firmware.

### Classification and Conflict Review
- Classified the workbook as a new multi-product `certificates` source; no same-lineage shared document existed, so no current source was replaced.
- Retained i2000, i5000, Q1000, Q1500, Q2000, Q3000, Q5000, T5000, i9101, i9200K, and i9600K in the shared source without creating unsupported canonical Product Hubs.
- Identified no unresolved same-context contradiction with product-specific sources. Project, OS, security-chip, historical, and expiry differences remain explicitly qualified.
- Added query guidance that `已通过` records must still be checked against their applicable expiry date and that PCI hardware and firmware expiry are separate fields.

### Validation
- Transcribed 3,419 non-empty cells and 452 merged ranges; the workbook contains no formulas, comments, hyperlinks, or embedded drawings.
- Reviewed rendered output for all 18 worksheets and preserved the original workbook SHA-256 `c2e6ae8d6fb67347b0fac062c772f88832e551c1bbdc2516ea1c68c11486d164`.

## [2026-08-11] sync | GMS, MDM, Google Key, and POS Kernel Workbooks

### Added
- Synchronized four new multi-product workbooks under `_shared/`: Google Key factory programming status, GMS/AER certification status, MDM certification status, and POS financial certification kernel versions.
- Preserved each original workbook byte-for-byte and generated a same-stem, coordinate-preserving Markdown companion with ISO-normalized true Excel dates.
- Added four shared Vault nodes and backlinks from 25 affected Product Hubs; models without canonical Hubs remain discoverable in each shared node's `Additional Models` or `Additional Projects` section.
- Linked the POS category page to both dated certification evidence and the separate payment-kernel version matrix.

### Classification and Conflict Review
- Classified all four workbooks as new multi-product sources. No same-lineage current document existed, so no synchronized source was replaced.
- Kept project-, Android-, region-, customer-brand-, MDM-vendor-, certification-, and component-layer qualifiers separate; no unresolved same-context contradiction was identified.
- Treated Google Key writing status as factory provisioning evidence rather than GMS certification, and treated kernel-version rows as complementary to—not proof of—dated certificate validity.
- Left the standalone `pda-info-summary.md` in `newly_added/` because it is an unpaired new Markdown source rather than a correction supported by an existing retained original.

### Validation
- Transcribed 12 worksheets and 1,925 non-empty cells across the four workbooks, including 72 merged ranges, 6 hyperlinks, and 3 embedded drawings; no formulas or comments were present.
- Preserved workbook SHA-256 hashes `5a385f0883955ca1467983bd4080e12dadf16a3837f5cfb28bc9f53a0896d393`, `b552eec1996d19189e37f9ee33baac63273c8deab55b5179ada4126e605364b4`, `ae35eca6eea839560140408564dc1e252b475262c8441fe365a7991b2678599a`, and `8f6fd7fec417e111867207e189b7bf932eefed169f06b28b79abe50313d94caa`.

## [2026-08-11] sync | User-Authored Canonical Markdown and PDA Matrix

### Rule Change
- Added an explicit one-file source form for standalone Markdown that the user identifies as personally authored or approves as canonical knowledge.
- Such Markdown is preserved unchanged and serves as both canonical source and retrieval form; no duplicate companion or Office/PDF original is required.
- Unconfirmed orphan conversions, temporary notes, and AI-generated summaries remain ineligible until the user supplies an original or explicitly adopts the Markdown as canonical.

### Added
- Synchronized `pda-info-summary.md` as `_shared/specs/pda-info-summary_202608111748/pda-info-summary.md` with unchanged SHA-256 `36e23b22eeaecf4d1abc5439173b7a447d06d4f915311e13673a8db9d1ec75b2`.
- Added the `PDA Platform, Memory, and Android Summary` shared node and backlinks from 22 affected Product Hubs.
- Preserved all 36 data rows, including duplicate CT58C/CT58S rows and non-canonical models, without rewriting user-authored content.

### Conflict Review
- Recorded the CT58S/SQ58S Android 12-versus-14 difference, the SP35 6+64-versus-4+64 memory-option difference, and the SQ53Pro DT50-versus-DT50 Pro market-label difference.
- Recorded the SQ66 Android 13/15 project-label ambiguity because the GMS/AER table uses SQ66 while its maintenance note refers to the Android 15 project as SQ66V.

## [2026-08-11] sync | SQ53 and Portfolio Battlecards

### Added
- Synchronized `SQ53PRO VS SQ53ST Battle Card.pptx` and `Urovo PDA Battlecard_20251205.pptx` as two new multi-product comparison sources under `_shared/comparison/`.
- Preserved both PPTX files byte-for-byte and generated same-stem Markdown companions covering all 16 slides, 14 tables, slide text, labels, qualifiers, source footers, and speaker-note state.
- Added two shared Vault nodes and backlinks from 11 affected Product Hubs. DT50 5G, DT510, and K388S remain discoverable through the shared node without creating unsupported canonical Hubs.

### Routing and Conflict Review
- Routed SQ53PRO to DT50-Pro, SQ53ST to DT50, and SQ630 to DT630 while retaining the source-specific market labels and exact internal project identifiers.
- Added active discrepancies for SQ53 model labels and the DT50-Pro Android ceiling; DT66 sealing; DT610 weight, extended battery, and biometrics; CT48 CPU; U2S battery, sealing, and camera position; SR5600 battery and connectivity; DT630 weight, battery, and Android ceiling; RT30 weight and display option direction; and K388 Pro camera terminology/coverage.
- Treated the DT66 FHD display as a valid optional configuration because the product specification explicitly lists it as optional. Competitor values remain dated Battlecard evidence rather than current authoritative specifications.

### Validation
- Source and synchronized original SHA-256 hashes match: `266bec4454c3f46757dd3b265595e765c7bad523a1e4a6bedb7ac4fcce5c0e1c` and `593cec178aebbe9b0e131b2e32777bbf44f2d2010d8db583238992443cf12f3c`.
- Visually reviewed all 16 rendered slides. The converted Markdown contains 14 tables with the same row/column dimensions as the source layouts.

## [2026-08-12] sync | Internal-to-Market Model Mappings and DT50S Canonicalization

### Added
- Synchronized 27 user-authored Markdown files as unchanged one-file canonical sources under each affected product's `others/internal-model-mapping_202608121411/` slot.
- Added the new source to every affected Product Hub so internal project identifiers, market names, Android variants, memory configurations, lifecycle notes, scanners, and accessories remain directly discoverable.
- Cleared every successfully processed inbox input; only `newly_added/README.md` remains.

### Canonical Identity
- Renamed the legacy `DT50` product root, Product Hub, specification page, and brochure page to `DT50S`.
- Routed `SQ53S` and `SQ53ST` through the canonical `DT50S` Hub while preserving retained source filenames and source-specific `DT50` labels as provenance.
- Kept `DT50 5G` (`SQ53B` / `SQ53BV`) separate from the DT50S 4G lineage and corrected shared navigation that had treated DT50S as unhubbed.

### Conflict Review
- Added or corroborated active source differences for CT48 CPU speed, CT48C AnTuTu score, CT58 CPU speed, DT50P battery/configuration, DT66 Android project labeling, SP35 memory options, and U2S battery and scan-engine configuration.
- Treated model variants, optional configurations, lifecycle status, and source-specific market labels as qualified context rather than silently merging them into universal product facts.

### Validation
- Product structure and exhaustive Hub coverage test passed.
- Skill package validation and Wiki/provenance link audits passed.

## [2026-08-14] sync | DT66 Internal Model Correction and FR2000 User Manual

### Replaced
- Replaced the DT66 authored internal-model mapping with the corrected canonical Markdown under `DT66/others/internal-model-mapping_202608142020/`.
- The current mapping now assigns Android 13 to SQ66 and Android 15 to SQ66V instead of combining both operating-system versions under SQ66.
- Updated the DT66 Product Hub to use the corrected path and to route current Android 15 answers through SQ66V while preserving the earlier SQ66-labelled certification row as historical provenance.

### Added
- Synchronized `User_Manual_for_FR2000_Desktop_RFID.docx` under `FR2000/user_guide/default_202608142020/` without changing the original bytes.
- Generated a same-stem Markdown companion covering the manual's body text, operational steps, tables, screenshot-only interface values, sample identifiers, safety guidance, development-material folders, and appendix specifications.
- Added the user guide to the exhaustive FR2000 Product Hub.

### Conflict Review
- Recorded the manual's 0–27 dBm setup limit against its own 30 dBm Android screenshot and appendix, as well as the 30 dBm maximum in the current specification and brochure.
- Recorded the manual appendix's Bluetooth 5.0/RJ45 optional qualifier against the supported-connectivity language elsewhere in the manual, specification, and brochure.
- Treated the corrected user-authored DT66 mapping and the certification maintenance note as the current routing authority for SQ66V, without deleting the contradictory historical workbook row.

### Validation
- Rendered and reviewed all 25 pages of the FR2000 DOCX and structurally inspected 168 paragraphs, five Word tables, headers, footers, and 30 embedded media items.
- Preserved original SHA-256 hashes `806329a518ed0cba45021a3d6f21350b7ff93a25e7a2d1b4eeea131ffb887896` (DT66 Markdown) and `509d26f885604f9919e8d9cd3c7134155212691b4fee80b9df3174fd86e79750` (FR2000 DOCX).
- Affected product layout, one-original/one-Markdown pairing, and exhaustive Product Hub coverage checks passed.
- Skill package validation passed; the Vault audit checked 1,165 wiki links with zero broken targets.

## [2026-08-16] sync | 6 Scan Engine Specifications (Honeywell EX30 / N570X / N6803, UROVO SE2030S, Zebra SE55 / SE58)

### Added
- Created new shared semantic-type `_shared/scan-engines/` for third-party (Honeywell, Zebra) and UROVO's own scan engine specifications. These are component specs referenced by multiple UROVO barcode-scanning products; following the `_shared/rfid-tags/` precedent (third-party RFID tag specs).
- Synchronized 6 sources into timestamped document directories `*_202608161732/`:
  - `Honeywell-Scanner-EX30-Specs.pdf` → `_shared/scan-engines/honeywell-ex30-scan-engine_202608161732/` (Honeywell Extended FlexRange EX30, 10 cm–20 m auto-focus 2D scan engine, MIPI/parallel, N670X/N660X/N360X compatible)
  - `Honeywell-Scanner-HS7-Specs.pdf` → `_shared/scan-engines/honeywell-n570x-scan-engine_202608161732/` (Honeywell N570X Series — N5703SR / N5701HD compact 2D scan engines, 8.1×21.6×10.4 mm)
  - `Honeywell-Scanner-N6803FR-Specs.pdf` → `_shared/scan-engines/honeywell-n6803-scan-engine_202608161732/` (Honeywell FlexRange N6803 — MR/FR/LR ultra-slim 2D scan engines, 6 m / 10 m / 25 m)
  - `Urovo-Scanner-SE2030S-Specs.pdf` → `_shared/scan-engines/urovo-se2030s-scan-engine_202608161732/` (UROVO 自研 SE2030S 2D scan engine, 1280×1080, 红色十字激光)
  - `Zebra-SE55(00)-Specs.pdf` → `_shared/scan-engines/zebra-se55-scan-engine_202608161732/` (Zebra SE55 Advanced Range, IntelliFocus, 2.2 in–40 ft, 4 MP, PL5000A/PL5000C/SDL options)
  - `Zebra-SE58(00)-Specs.pdf` → `_shared/scan-engines/zebra-se58-scan-engine_202608161732/` (Zebra SE58 Extended Range, IntelliFocus, <2 in–105 ft, dual 1+2 MP, 10.6 g)
- Created 6 same-stem Markdown companions covering overview, features, technical specifications (mechanical / electrical / performance / environmental / decode ranges / symbologies / warranty), regulatory, and laser safety.
- Created 6 portfolio-wide shared Vault nodes under `product-knowledge-vault/shared/` (honeywell-ex30-scan-engine, honeywell-n570x-scan-engine, honeywell-n6803-scan-engine, urovo-se2030s-scan-engine, zebra-se55-scan-engine, zebra-se58-scan-engine) with scope, affected products, query guidance, and cross-references.
- Updated `product-knowledge-vault/index.md` to list 6 new shared nodes; shared source nodes count 22 → 28, total 186 → 192.

### Classification
- All 6 inputs are **scan engine component specs** (third-party Honeywell/Zebra OEM scan engines + UROVO's own SE2030S), not standalone UROVO end products. Routed to new `_shared/scan-engines/` semantic-type because they are referenced by multiple UROVO barcode-scanning products.
- Source filenames preserved byte-identical (e.g., `Honeywell-Scanner-HS7-Specs.pdf` → routed to N570X series content; `Honeywell-Scanner-N6803FR-Specs.pdf` → routed to N6803 series content covering MR/FR/LR). Document-key is descriptive of the actual content series, not the filename.

### Validation
- All 6 PDF copies SHA-256 verified identical to inbox originals; bytes unchanged.
- Visual verification performed on N6803FR pages 2–3 (electrical, performance, environmental, read ranges tables), SE55 page 3 (full spec table + decode ranges), SE58 page 3 (full spec table + decode ranges), SE2030S page 1 (Chinese spec sheet). Markitdown text layer was complete for EX30 and N570X; visual verification confirmed accurate table reconstruction where markitdown column ordering was scrambled.
- All 6 companions include exact model numbers, mechanical dimensions, electrical specs, performance characteristics, environmental limits, full decode range tables (mm/inch), symbology lists, and warranty terms. No facts invented from memory; no silent corrections.
- Removed all 6 inputs from `newly_added/` after successful sync.

### Discrepancies
- None recorded at the source-vs-companion level. The 6 specs are from independent vendors (Honeywell, Zebra, UROVO) and have no cross-vendor factual alignment to verify.

## [2026-08-17] sync | Scanner 默认配置说明 (Default Profile, user-authored Markdown)

### Added
- Synchronized user-authored canonical Markdown `Scanner默认配置说明.md` as a **one-file source slot** under `_shared/operations/scanner-default-config_202608170900/` (no companion, file unchanged).
- The Markdown documents the UROVO scanner `Default` profile (from `Default_scanner_property.xml`): grouped by function — configuration basics, symbology (1D/2D/composite/postal) default enable states, output config (keyboard wedge / Intent / clipboard / TCP-IP / cache), data post-processing (append enter, prefix/suffix, regex matcher, encoding, UDI parser, advanced formatting), trigger & power saving, decode behavior, imaging/exposure/illumination, image preprocessing, OCR, and engine/other options.
- Created shared Vault node `product-knowledge-vault/shared/scanner-default-config.md` with scope, query guidance, and cross-references to Scan Settings User Manual / Scan Data Advanced Formatting / Scan Engine Specifications.
- Updated `product-knowledge-vault/index.md`: shared source nodes 28 → 29, total 192 → 193.

### Classification
- Standalone Markdown, user explicitly confirmed as authoritative/canonical knowledge (option "作为权威知识直接同步"). Per SYNC_PROMPT rule 10, synchronized unchanged as a one-file source slot; no duplicate companion created.
- Routed to `_shared/operations/` (platform-level scanner configuration reference), consistent with existing `scan-settings-user-manual` and `scan-data-advanced-formatting` nodes.

### Validation
- SHA-256 verified byte-identical (`945add04396211cd32dc3b71ca3512af21d61341f8699a41e0683e4547f0df7a`).
- Removed the inbox input after successful sync.

### Discrepancies
- None recorded.

## [2026-08-28] sync | U100 Refresh, UPad Printer Dock, T500 Reference, and Heating App

### Replaced
- Replaced `U100/specs/default_202601010000/` with the newer 2026-08-25 U100 price-checker specification under `U100/specs/default_202608281943/`; the previous source pair was removed only after the new original/Markdown pair and Hub coverage passed validation.
- Refreshed the U100 semantic specification, product page, category summary, and Skill overview from the current source.

### Added
- Added `U100/accessories/default_202608281943/` for the standard power adapter and quick-hitch bracket plus the optional height-adjustable 360-degree desk clamp stand.
- Added `UPad/accessories/dual-screen-printer-dock_202608281943/` for the UPad host, multifunction dock, and 203 dpi / 250 mm/s thermal printer system.
- Added `_shared/specs/xydcode-t500-fixed-mount-scanner_202608281943/` and `shared/xydcode-t500-fixed-mount-scanner.md` as an external/vendor reference. The source identifies Shenzhen XYDcode Technology Co., Ltd. and does not identify T500 as a UROVO product, so no UROVO Product Hub or portfolio-count entry was created.
- Added `_shared/operations/heating-app-instructions_202608281943/` and `shared/heating-app-instructions.md`. The source names no compatible hardware model, so no Product Hub backlink was inferred.
- Added both new shared nodes to the Vault index and added the external T500 reference to the barcode-scanner category without changing the canonical UROVO product count.

### Active Discrepancies
- U100's source prints operating temperature as both `0°C to 50°C` and `14°F to 131°F`; these are not equivalent conversions. Both ranges are preserved and flagged in the U100 Hub and semantic specification.
- UPad sources disagree between an “under 7 mm” marketing claim and an 11 mm specification value, and between 1 TB and 2 TB maximum MicroSD capacity. Both differences are preserved and flagged in the UPad Hub, specification, product page, and category summary.
- Heating App narrative states a 35°C overtemperature default while two screenshots display 25°C. The companion preserves 35°C as the documented default and treats 25°C as the shown configured/example state.

### Validation
- Visually inspected every page: T500 3/3, U100 accessories 2/2, U100 specification 2/2, UPad printer dock 3/3, and the converted Heating App document 10/10.
- Verified original SHA-256 hashes after copying: `b64ac391cc43565652c908397d3ad8a891abde8ea15c46a6b2f7e39785f609fb` (T500), `e332d596e2f22dba3fcf3ad71e782e80ee5a53607d25f043413977d3fcfb5020` (U100 accessories), `58f409c23bf146b1878c72bf20e0fe4df8f5d5536e166ff7f4b00ea70c8417b8` (U100 specification), `4818e062e66041bb32a576f655c11cfb61e1988c750e2d505fe3d736a5a85a78` (UPad printer dock), and `7fc30d94258537c799b4c9e6d200994b06e2f7e84106da803acea3f9f58e41e5` (Heating App).
- All five synchronized slots passed exact same-stem source/Markdown pairing; all first-five product source types passed the single-slot rule; U100 and UPad Hubs cover every current non-hidden source file.
- Skill package validation and `git diff --check` passed. The Vault audit checked 1,320 Wiki links with zero broken targets; a pre-existing aggregate `shared/scan-engines` link was replaced with links to the six existing engine nodes.
- Removed all five successfully synchronized inputs from `newly_added/`; only the inbox README and ignored hidden metadata remain.

## [2026-08-30] sync | SP35 Refresh and Europe Product Brochure

### Replaced
- Replaced `SP35/specs/default_202608111352/` with the newer `SP35/specs/default_202608301711/` source pair. The synchronized 2026-08-21 specification covers the complete five-page source, including hardware, wireless, data capture, environment, software, accessories, and regional contacts.
- Replaced `SP35/others/new-product-announcement_202608211009/` with `SP35/others/new-product-announcement_202608301711/`. The synchronized announcement preserves all 13 slides, their product imagery and diagrams, configurations, use cases, optional UHF module, accessories, and slide-specific claims.
- Updated the SP35 Source Hub, specification page, product page, and handheld-terminal category summary to route current queries through the new sources.

### Added
- Added `_shared/brochure/urovo-product-brochure-europe_202608301711/` as a distinct dated multi-product brochure; it does not replace any product-specific brochure slot.
- Created the portfolio shared node `shared/urovo-product-brochure-europe-20260826.md` and linked it bidirectionally with all 41 affected Product Hubs.
- Added the shared node to the Vault index, increasing shared source nodes from 33 to 34 and total pages from 201 to 202.

### Active Discrepancies
- SP35: current specification/NPA support 6+64 standard and 8+128 optional, while internal/shared configuration sources retain 8+128 with 4+64 optional; UHF range is stated as both 1.2 m and 1.5 m; Bluetooth class is stated as configurable Class 1/2 and Class 2. The specification's operating-temperature text layer and Fahrenheit value indicate -10°C, while the rendered Celsius row visually lacks the minus sign.
- DT50S: the Europe brochure's source-labelled `DT50` panel states Android 16 and 16 MP in body copy, while its own icon and the dedicated source state 13 MP; the dedicated source states Android 11 with Android 13 optional.
- DT610 Pro: the Europe brochure and shared series sheet state 5200 mAh, versus 5500 mAh in product-specific sources; the dedicated specification itself contains Bluetooth 6.0 marketing copy and a Bluetooth 5.0 wireless-PAN table.
- SR5750: the same brochure panel states 1200 mAh in body copy and 1150 mAh in its icon; the dedicated specification states 1150 mAh.
- RFG91, U2S, UPad, DT66, and P8100P 4G: the new brochure was added as corroborating provenance to their already active battery, thickness, or sealing differences.

### Validation
- Preserved exact original bytes. SHA-256: `9408a6b61cd96471e24fda59082e5fbb3a070ef268007760bf3cb289940c8396` (SP35 specification), `a6a42c2d3c44b2cf47ff66bab779dc6c78bace2770408e544d4fafc4ff2a9e18` (SP35 announcement), and `2f55dea194c185716ab53a01573f1fce4c6be7b3b1619a5d49d089b5c2030274` (Europe brochure).
- Visually inspected every source page/slide: SP35 specification 5/5, SP35 announcement 13/13, and Europe brochure 14/14. Same-stem original/Markdown pairing passed for all three synchronized slots.
- Confirmed 41 unique brochure-covered Product Hubs, 41 Hub backlinks, and complete SP35 Hub coverage. The Vault audit checked 1,406 Wiki links with zero broken targets; all checked provenance paths resolved.
- Skill package validation passed.
