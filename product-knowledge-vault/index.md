# Product Knowledge Vault — Index

Master catalog of all pages in the UROVO Product Knowledge Base.

## Core Pages

| Page | Summary |
| --- | --- |
| [[overview|Overview]] | High-level product portfolio view with category breakdowns and technology landscape |
| [[synthesis|Synthesis & Key Insights]] | Cross-product patterns, strategic observations, and gap analysis |
| [[SCHEMA|SCHEMA.md]] | Wiki schema, conventions, source hierarchy, and LLM workflows |
| [[log|log.md]] | Chronological operation history |

## Product Source Hubs

Read the relevant Hub before answering a product query. Each Hub exhaustively lists that product's current local source documents and linked shared knowledge.

| Category | Product Hubs |
| --- | --- |
| Handheld Terminals | [[products/CT48|CT48]], [[products/CT48C|CT48C]], [[products/CT58|CT58]], [[products/CT58C|CT58C]], [[products/CT58S|CT58S]], [[products/DT40|DT40]], [[products/DT50S|DT50S]], [[products/DT50D|DT50D]], [[products/DT50P|DT50P]], [[products/DT50P-Lite|DT50P Lite]], [[products/RT30|RT30]], [[products/RT40S|RT40S]], [[products/SP35|SP35]] |
| Enterprise Smartphones | [[products/DT50-Pro|DT50-Pro]], [[products/DT66|DT66]], [[products/DT610|DT610]], [[products/DT610-Pro|DT610 Pro]], [[products/DT630|DT630]] |
| POS Terminals | [[products/i5300|i5300]], [[products/i5300L|i5300L]], [[products/i9000S|i9000S]], [[products/i9100|i9100]], [[products/i9200|i9200]], [[products/i9600|i9600]], [[products/i9600-Mini|i9600 Mini]] |
| Barcode Scanners | [[products/R7|R7]], [[products/K180|K180]], [[products/K200|K200]], [[products/K220|K220]], [[products/SR5600|SR5600]], [[products/SR5600-V2|SR5600 V2]], [[products/SR5750|SR5750]], [[products/S710|S710]] |
| Mobile Printers | [[products/K329|K329]], [[products/K388-Pro|K388 Pro]], [[products/K389|K389]], [[products/K419|K419]] |
| Desktop Printers | [[products/D8100-plus|D8100 Plus]], [[products/D81R-Series|D81R Series]], [[products/T1120|T1120]] |
| Fixed RFID Readers | [[products/FR1000|FR1000]], [[products/FR2000|FR2000]], [[products/FR7000-Series|FR7000 Series]] |
| RFID Sled & Tablets | [[products/RFG91|RFG91]], [[products/P8100-4G|P8100 4G]], [[products/P8100P-4G|P8100P 4G]], [[products/P8100P-5G|P8100P 5G]], [[products/UPad|UPad]] |
| Wearables & Others | [[products/U2S|U2S]], [[products/U100|U100]] |
| Electronic Shelf Labels | [[products/ESL|ESL]] |

## Shared Knowledge Sources

Multi-product documents are synchronized under `_shared/`. Read the corresponding Vault node for scope, affected products, query guidance, and active discrepancies.

| Page | Scope |
| --- | --- |
| [[shared/i9000s-i9100-internal-project-differences|i9000S / i9100 Internal Project Differences]] | SQ27/SQ29 project, market, lifecycle, and configuration differences |
| [[shared/pos-certificates|POS Certificates and Firmware Validity]] | Dated payment/security certification status, report and certificate numbers, expiry dates, and PCI firmware validity across POS models and projects |
| [[shared/pos-financial-certification-kernel-versions|POS Financial Certification Kernel Versions]] | ICCR/PCD and payment-application kernel versions by POS model and SQ project |
| [[shared/gms-aer-certification-summary|GMS and AER Certification Summary]] | GMS/MADA, EDLA, and AER status, regions, certification windows, and SMR/MR history |
| [[shared/gms-certification-reuse-statistics|GMS Certification Reuse Statistics]] | Which internal models reuse (套用) another model's GMS certification, keyed by ro.product.device with application time |
| [[shared/mdm-certification-summary|MDM Certification Summary]] | SOTI, AirWatch, Springdel, Ivanti, and TeamViewer validation by model, project, and Android version |
| [[shared/gms-google-key-factory-programming-status|GMS Google Key Factory Programming Status]] | Google Key requirement, programming method, property import, and factory-test provisioning by internal project |
| [[shared/urovo-oemconfig-manual|Urovo OEMConfig User Manual]] | OEMConfig 1.0 configuration groups, actions, and items exposed to EMM solutions across the UROVO Android portfolio |
| [[shared/u-stage-operation-manual|U Stage Operation Manual V1.1]] | Platform-wide UEE staging tool: export/import via UMS, QR, or local file; synchronizable scanner/system/RFID/UBrowser settings |
| [[shared/soti-oemconfig-guide|SOTI-OEMConfig Guide]] | Step-by-step SOTI (MobiControl) + Urovo OEMConfig deployment procedure |
| [[shared/rfid-demo-user-manual|RFID-Demo User Manual]] | Built-in RFID tag read/write demo application (UHF EPC C1G2 / HF ISO 15693-14443), platform-wide |
| [[shared/rfid-wedge-user-manual|RFIDWedge User Manual]] | No-code RFID input tool (keyboard-wedge style) for delivering tag data into apps without integration |
| [[shared/scan-settings-user-manual|Scan Settings User Manual]] | Built-in barcode scan configuration app (symbology, output mode, prefix/suffix, trigger) |
| [[shared/scan-data-advanced-formatting|Scan Data Advanced Formatting]] | Chinese reference for advanced scan-data output formatting and control interface |
| [[shared/rfid-tag-application-selection|RFID Tag Application Selection (勤业/Qinye)]] | UHF RFID tag selection by 8 industries (apparel/food/3C/logistics/medical/energy/auto/finance), with DTB-* model, size, and chip |
| [[shared/rfid-tag-catalog|RFID Tag Catalog (勤业/Qinye)]] | UHF RFID tag catalog by form factor (adhesive/woven/flex/ABS/card/PCB) + UHF chip comparison table |
| [[shared/pda-info-summary|PDA Platform, Memory, and Android Summary]] | User-authored market model, internal project, platform, memory, and Android mapping across PDA-related products |
| [[shared/device-and-accessories-guide|Device and Accessories Guide]] | Portfolio device configurations, accessory compatibility/codes/status, and printer matrix |
| [[shared/dt50-series-accessories-guide|DT50 Series Accessories Guide]] | DT50S / DT50-Pro batteries, charging, protection, carrying, and trigger accessories |
| [[shared/dt610-series-product-spec-sheet|DT610 Series Product Spec Sheet]] | Side-by-side DT610 Std and DT610 Pro specifications |
| [[shared/k388-pro-series-product-spec-sheet|K388 Pro Series Product Spec Sheet]] | K388 Pro 2’’, K388 Pro 4’’, and K388 Pro BT (7-page 2026-09-16 edition) |
| [[shared/sq53pro-vs-sq53st-battlecard|SQ53PRO vs SQ53ST Battle Card]] | Direct DT50PRO/SQ53PRO versus DT50S/SQ53ST comparison; the deck itself uses the DT50 label for SQ53ST |
| [[shared/urovo-pda-battlecard|Urovo PDA Battlecard 2025-12-05]] | Dated UROVO-versus-competitor tables covering ten canonical Product Hubs plus DT50 5G, DT510, and K388S |
| [[shared/urovo-spec-comparison|Urovo Spec Comparison 241030]] | Dated 2024-10-30 Excel competitive sheet covering ten Product Hubs plus DT40S, DT50U, DT51U, DT51D, and RFDT50; not a live competitor-spec feed |
| [[shared/honeywell-ex30-scan-engine|Honeywell Extended FlexRange EX30 2D Scan Engine]] | Honeywell EX30 undecoded auto-focus 2D scan engine, 10 cm–20 m read range, MIPI/parallel |
| [[shared/honeywell-n570x-scan-engine|Honeywell N570X Series 2D Scan Engines]] | Honeywell N5703SR (Standard Range) + N5701HD (High Density) compact 2D scan engines, 8.1×21.6×10.4 mm |
| [[shared/honeywell-n6803-scan-engine|Honeywell FlexRange N6803 Series 2D Scan Engines]] | Honeywell N6803MR (6 m) / N6803FR (10 m) / N6803LR (25 m) ultra-slim 2D scan engines |
| [[shared/urovo-se2030s-scan-engine|UROVO SE2030S 2D Scan Engine]] | UROVO 自研 SE2030S 扫描引擎规格参数（1280×1080 / 红色十字激光 / 60 fps） |
| [[shared/zebra-se55-scan-engine|Zebra SE55 Advanced Range Scan Engine]] | Zebra SE55 IntelliFocus 2D scan engine, 2.2 in–40 ft, 4 MP, PL5000A/PL5000C/SDL options |
| [[shared/zebra-se58-scan-engine|Zebra SE58 Extended Range Scan Engine]] | Zebra SE58 IntelliFocus 2D scan engine, <2 in–105 ft, dual 1+2 MP, 10.6 g ultra-light |
| [[shared/scanner-default-config|Scanner 默认配置说明 (Default Profile)]] | UROVO 扫描器 Default profile 全参数默认值（码制/输出/后处理/触发/成像/OCR），源自 Default_scanner_property.xml |
| [[shared/kms-standard-solution-key-exchange-en|KMS Standard Solution — Customer Key Exchange and KMS Key Loading]] | V1.0 English process for MK/SK (KEK + TR-31 TMK) and DUKPT (BDK or ZMK + TR-31 BDK) customer key exchange into UROVO KMS |
| [[shared/kld-operation-manual|KLD Operation Manual]] | Master POS KLD app: administrator/operator login, BDK/KEK/TMK import, CA download, Load Key to Sub-POS, lockout/activation |
| [[shared/kld-mutual-authentication-overview|KLD Mutual Authentication Overview]] | POS-wide certificate Check Binding (CAKRD/CredKRD, CAKDH/CredKDH, CRL) before TR-34-style key injection; not the KLD app UI manual |
| [[shared/urovo-product-price-book-2026-7-25|Urovo Product Price Book (2026-07-25)]] | Dated commercial USD price list covering 28 Product Hubs plus additional labels without Hubs; not a live spec |
| [[shared/heating-app-instructions|Heating App Instructions v1.2]] | Cross-product operating guide for fast temperature rise, rapid cooling, one-touch heating, global-button control, and stop conditions; no compatible hardware model is named in the source |
| [[shared/printer-consumables-knowledge|打印机知识点（耗材）]] | Thermal vs thermal-transfer printing and ribbon/media pairing; no named model; backlinked to six printer Hubs |
| [[shared/xydcode-t500-fixed-mount-scanner|XYDcode T500 Fixed-Mount Barcode Scanner]] | External/vendor fixed-mount 1D/2D scanner reference; the source does not identify T500 as a UROVO product |
| [[shared/urovo-product-brochure-europe-20260904|UROVO Product Brochure — Europe Edition (2026-09-04)]] | Dated 14-page portfolio brochure covering 41 Product Hubs, accessories, company positioning, applications, and the UEE software ecosystem |
| [[shared/urovo-product-brochure-na-20260904|UROVO Product Brochure — North America Edition (2026-09-04)]] | Dated 14-page NA-region portfolio brochure (Irvine / us.urovo.com); product mix differs from the Europe edition |
| [[shared/urovo-rfid-product-brochure-20260904|UROVO RFID Product Brochure (2026-09-04)]] | Dated 8-page RFID introduction covering 14 Product Hubs |

## Entity Pages (Key Components)

| Page | Summary |
| --- | --- |
| [[entity/impinj-e710|Impinj E710]] | Flagship UHF RFID chipset — 1,300+ tags/sec across 8 products |
| [[entity/qualcomm-q6690|Qualcomm Q-6690]] | Next-gen enterprise processor — 6 TOPS AI, integrated RFID |

## Technology Pages

| Page | Summary |
| --- | --- |
| [[technology/wi-fi-7|Wi-Fi 7 (802.11be)]] | 5,764.7 Mbps, 320 MHz — deployed on DT610 series |
| [[technology/uhf-rfid|UHF RFID Technology]] | Full UHF RFID ecosystem: 10 products, 4 form factors, 3 range tiers |

## Comparison Pages

| Page | Summary |
| --- | --- |
| [[comparisons/ct-series-comparison|CT Series Comparison]] | CT48/48C vs CT58/58C/58S — form factor, IP, SIM decisions |
| [[comparisons/dt-series-comparison|DT Series Comparison]] | DT40→DT50P Lite — entry to UHF pistol grip |
| [[comparisons/enterprise-smartphone-comparison|Enterprise Smartphone Comparison]] | DT610→DT630 — flagship 5G smartphone specs |

## Category Overviews

| Page | Products | Summary |
| --- | --- | --- |
| [[categories/handheld-terminal|Handheld Terminals]] | 13 | CT48–CT58S, DT40–DT50P Lite, RT30, RT40S, SP35 |
| [[categories/enterprise-smartphone|Enterprise Smartphones]] | 5 | DT50-Pro, DT66, DT610–DT630 |
| [[categories/pos-terminal|POS Terminals]] | 7 | i5300/i5300L, i9000S, i9100, i9200, i9600, i9600 Mini |
| [[categories/barcode-scanner|Barcode Scanners]] | 8 | R7 (R70/R71), K180, K200, K220, SR5600, SR5600 V2, SR5750, S710 |
| [[categories/mobile-printer|Mobile Printers]] | 4 | K329, K388 Pro, K389, K419 |
| [[categories/desktop-printer|Desktop Printers & Fixed RFID]] | 6 | D8100 Plus, D81R, T1120, FR1000, FR2000, FR7000 |
| [[categories/other-devices|RFID Sled, Tablets, Wearables & More]] | 8 | RFG91, P8100 Series, UPad, U2S, U100 |
| [[categories/esl|Electronic Shelf Labels]] | 1 | ESL (ET0213 / T2664 / ET0420 tags + F24A7 base station) |

Category membership can overlap: SR5750 is both a barcode-scanning device and a wearable computer. The 51-product total counts each product once.

## Product Specification Pages

### Handheld Terminals
| Page | Product |
| --- | --- |
| [[spec/CT48|CT48]] | Compact keypad handheld, Android 12, IP67 |
| [[spec/CT48C|CT48C]] | CT48 with 2W speaker, 80% faster Antutu |
| [[spec/CT58|CT58]] | 5.5" handheld, IP65, PDAF camera |
| [[spec/CT58C|CT58C]] | 5.5" handheld, IP67, dual SIM, WPA3 |
| [[spec/CT58S|CT58S]] | 5.5" handheld, IP67, 2.2 GHz |
| [[spec/DT40|DT40]] | Entry-level, 4" Gorilla Glass, BT4.2 |
| [[spec/DT50S|DT50S]] | Premium 5.7", Wi-Fi 6 Ready, up to 8GB |
| [[spec/DT50D|DT50D]] | DT50S-series handheld with UHF RFID (1.5m) |
| [[spec/DT50P|DT50P]] | Pistol grip, Impinj E710, 20m UHF, 9000mAh |
| [[spec/DT50P-Lite|DT50P Lite]] | Lightweight 498g, dual HF+UHF RFID |
| [[spec/RT30|RT30]] | Compact 3.5", Android 14, hot-swap |
| [[spec/RT40S|RT40S]] | 4" with cold chain -30°C option |
| [[spec/SP35|SP35]] | Personal shopper, Q-6690, UWB, optional UHF RFID |

### Enterprise Smartphones
| Page | Product |
| --- | --- |
| [[spec/DT50-Pro|DT50-Pro]] | Android 16, Wi-Fi 6E, AnTuTu 418K |
| [[spec/DT66|DT66]] | 5G, Wi-Fi 6E, 6.5", iToF, IP68 |
| [[spec/DT610|DT610]] | Qualcomm Q-6690, Wi-Fi 7, 5G, 222g |
| [[spec/DT610-Pro|DT610 Pro]] | Q-6690, 50MP, 3D sensing, IP68 |
| [[spec/DT630|DT630]] | 4nm NPU, 6.6", 10.4mm, IP68 |

### POS Terminals
| Page | Product |
| --- | --- |
| [[spec/i5300|i5300]] | Compact smart POS, 3.5" display |
| [[spec/i5300L|i5300L]] | Smart POS, 5" display |
| [[spec/i9000S|i9000S]] | 5.0", Octa-core, PCI/EMV |
| [[spec/i9100|i9100]] | 5.5", Quad-core, value POS |
| [[spec/i9200|i9200]] | 5.5", Octa/Quad option |
| [[spec/i9600|i9600]] | Dual screen, 58mm 80mm/s printer |
| [[spec/i9600-Mini|i9600 Mini]] | MiniPOS, 6.745", 17 mm / 298 g, no printer |

### Barcode Scanners
| Page | Product |
| --- | --- |
| [[spec/K180|K180]] | Wireless ring scanner, BT5.2 |
| [[spec/K200|K200]] | Wired handheld, DPM reading |
| [[spec/K220|K220]] | Wireless handheld with base |
| [[spec/SR5600-V2|SR5600 V2]] | Wearable ring, BT5.3, IP65 |
| [[spec/SR5750|SR5750]] | Android wearable computer |
| [[spec/S710|S710]] | Desktop barcode reader |

### Mobile Printers
| Page | Product |
| --- | --- |
| [[spec/K329|K329]] | Thermal mobile, 120mm/s, NFC |
| [[spec/K388-Pro|K388 Pro]] | 4-in-1 labeling, Android 14 (upgradable to 20) |
| [[spec/K389|K389]] | Rugged mobile, 2m drop, 390g |

### Desktop Printers
| Page | Product |
| --- | --- |
| [[spec/D8100-plus|D8100 Plus]] | Thermal transfer, 203/300 DPI |
| [[spec/D81R-Series|D81R Series]] | RFID thermal transfer |
| [[spec/T1120|T1120]] | 4-inch industrial, 203 mm/s, 104 mm |

### Fixed RFID Readers
| Page | Product |
| --- | --- |
| [[spec/FR1000|FR1000]] | Box reader, 8× SMA antenna |
| [[spec/FR2000|FR2000]] | Desktop RFID pad |
| [[spec/FR7000-Series|FR7000 Series]] | Antenna reader, 6/9dBi |

### RFID Sled & Tablets
| Page | Product |
| --- | --- |
| [[spec/RFG91|RFG91]] | UHF RFID sled, multi-platform |
| [[spec/P8100-4G|P8100 4G]] | 8" tablet, Wi-Fi 6 Ready |
| [[spec/P8100P-4G|P8100P 4G]] | 10.1" tablet, 10000mAh |
| [[spec/P8100P-5G|P8100P 5G]] | 10.1" 5G tablet, Wi-Fi 6E |
| [[spec/UPad|UPad]] | 11" commercial tablet, SoftPOS |

### Wearables & Others
| Page | Product |
| --- | --- |
| [[spec/U2S|U2S]] | Wearable computer, dual scanners |
| [[spec/U100|U100]] | Price checker, 10.1" |
| [[spec/ESL|ESL]] | Electronic shelf labels + F24A7 base station |

## Comparison & Analysis

| Page | Summary |
| --- | --- |
| [[matrices/performance-matrix|Performance Comparison Matrix]] | Full spec comparison across 26 products |
| [[overview|Technology Landscape]] | OS, processor, wireless, RFID evolution |

## Feature Dimension Pages

| Page | Summary |
| --- | --- |
| [[features/connectivity|Connectivity Evolution]] | Wi-Fi, Bluetooth, and Cellular generational tracking |
| [[features/durability|Durability Tiers]] | IP ratings, drop resistance, temperature ranges |
| [[features/rfid-capabilities|RFID Capabilities]] | HF vs UHF, chipset distribution, range tiers |

## Product Brochure Pages (51 products)

| Category | Pages |
| --- | --- |
| Handheld Terminals | [[pb/CT48|CT48]], [[pb/CT48C|CT48C]], [[pb/CT58|CT58]], [[pb/CT58C|CT58C]], [[pb/DT40|DT40]], [[pb/DT50S|DT50S]], [[pb/DT50D|DT50D]], [[pb/DT50P|DT50P]], [[pb/DT50P-Lite|DT50P Lite]], [[pb/RT30|RT30]], [[pb/RT40S|RT40S]], [[pb/SP35|SP35]] |
| Enterprise Smartphones | [[pb/DT50-Pro|DT50-Pro]], [[pb/DT66|DT66]], [[pb/DT610|DT610]], [[pb/DT610-Pro|DT610 Pro]], [[pb/DT630|DT630]] |
| POS Terminals | [[pb/i5300|i5300]], [[pb/i5300L|i5300L]], [[pb/i9000S|i9000S]], [[pb/i9100|i9100]], [[pb/i9200|i9200]], [[pb/i9600|i9600]], [[pb/i9600-Mini|i9600 Mini]] |
| Barcode Scanners | [[pb/R7|R7 Series]], [[pb/K180|K180]], [[pb/K200|K200]], [[pb/K220|K220]], [[pb/SR5600|SR5600]], [[pb/SR5600-V2|SR5600 V2]], [[pb/SR5750|SR5750]], [[pb/S710|S710]] |
| Mobile Printers | [[pb/K329|K329]], [[pb/K388-Pro|K388 Pro]], [[pb/K389|K389]], [[pb/K419|K419]] |
| Desktop Printers | [[pb/D8100-plus|D8100 Plus]], [[pb/D81R-Series|D81R Series]], [[pb/T1120|T1120]] |
| Fixed RFID Readers | [[pb/FR1000|FR1000]], [[pb/FR2000|FR2000]], [[pb/FR7000-Series|FR7000 Series]] |
| RFID Sled & Tablets | [[pb/RFG91|RFG91]], [[pb/P8100-4G|P8100 4G]], [[pb/P8100P-4G|P8100P 4G]], [[pb/P8100P-5G|P8100P 5G]], [[pb/UPad|UPad]] |
| Wearables & Others | [[pb/U2S|U2S]], [[pb/U100|U100]] |
| Electronic Shelf Labels | [[pb/ESL|ESL]] |

---

*Last updated: 2026-09-18 | 51 products | 51 product hubs | 37 shared source nodes | 48 spec pages | 51 brochure/product pages | 8 category pages | 3 comparison pages | 3 feature pages | 1 matrix page | 2 technology pages | 2 entity pages | 5 core pages | 211 total*
