# Urovo Product Price Book (filename date 2026_7_25)

> Canonical original: `_shared/pricing/urovo-product-price-book_202609121037/Urovo_Product_Price_Book-2026_7_25.xls` (bytes and `.xls` filename unchanged). LibreOffice `.xlsx` conversion was inspection-only.
> SHA-256: `89824c722d9d852a239e8e2082f45499ca3913fc85dae60d74fc16e36e8d0d76`
> Replaces `_shared/pricing/urovo-product-price-book_202609112225/Urovo_Product_Price_Book-2026_7_24.xls` (same document identity; filename date 2026_7_24 → 2026_7_25).
> Dated commercial / marketing price list. **Not a live spec.** Lead hard specs from each product `specs/` slot. Preserve USD prices, MOQ, accessory SKUs, and source labels (`SQ47S`, `SQ46S`, `DT50S`, `UPAD`, `SR5600 Pro`, `D812R`, `i9200 EMV`, `i9600 mini`).
> Sheets: 8. Formulas: 0. Picture-column cells that stored Excel `#NAME?` are recorded as that literal (broken picture formula), not as prices.
> Visual protocol: **77/77** unique `xl/media` files; **85** drawing anchors. All 77 media files and all 85 anchors are byte-identical to the 2026_7_24 workbook. Tiny crops whose product identity cannot be read remain marked unreadable.

Company header repeated on every sheet:

- UROVO TECHNOLOGY CO., LTD.
- 36F, High-Tech Zone Union Tower, No.63,Xuefu Road, Nanshan district, Shenzhen, Guangdong, China
- Fax :  +86-755-23636919       Tel:  +86-755-23636919      Web: en.urovo.com
- PRICE LIST

Commercial footer repeated on every sheet (source spelling retained, including `shippment`):

| Field | Value |
| --- | --- |
| Warranty | 1 year factory warranty for main device; 6 months for accessories |
| Lead Time | Sample:2-10 working days;  Bulk order:20-40 working days |
| Payment Terms | Sample: 100% T/T; Bulk order: T/T 30% in advance upon order,rest 70% before shippment. |
| Trade Term | EXW SHENZHEN |

### Change vs 2026_7_24 (cell-level)

Product model rows, prices, and pictures are unchanged. Optional-config blocks changed:

| Sheet | 2026_7_24 Optional Config | 2026_7_25 Optional Config |
| --- | --- | --- |
| `DT66,DT50, CT58` | HS7; 5500 +100USD; 5800 +180USD; 8+128G +22USD | HS7:+15USD/pcs; 8+128G:+22USD/pcs (5500/5800 rows removed; footer shifted up) |
| `DT610，DT630` | HS7; 5500; 5800; 8+128G | **removed entire Optional Config block**; footer now starts at A8 |
| `P8100, P8100P，UPAD，U100` | HS7; 5500; 5800; 8+128G | only `8+128G:+22USD/pcs` in D17 (no Optional Config label in A17) |
| `RT40,CT48C` / `POS` / `U2S…` / `Printers` / `FIXED RFID READER` | unchanged | unchanged (RT40 and FIXED RFID still list HS7 / 5500 / 5800 / 8+128G) |

---

### DT66,DT50, CT58

`nonempty=140 formulas=0 merged=48 images=23`

`merged_ranges=A41:C41;A38:C39;A25:A37;E7:H7;A1:H1;E32:H32;D40:H40;E37:H37;E22:H22;A42:C42;E18:H18;E12:H12;E21:H21;D41:H41;E33:H33;A43:C43;A6:A15;E14:H14;A3:H3;E17:H17;E23:H23;E8:H8;A16:A23;D43:H43;A2:H2;E35:H35;E20:H20;A40:C40;E29:H29;B7:B15;E19:H19;E10:H10;E28:H28;E13:H13;A4:H4;D39:H39;E9:H9;E31:H31;E34:H34;D42:H42;B17:B23;E30:H30;E15:H15;D38:H38;E11:H11;E27:H27;B27:B37;E36:H36`

| Cell | Value |
| --- | --- |
| A1 | UROVO TECHNOLOGY CO., LTD. |
| A2 |  36F, High-Tech Zone Union Tower, No.63,Xuefu Road, Nanshan district, Shenzhen, Guangdong, China |
| A3 |  Fax :  +86-755-23636919       Tel:  +86-755-23636919      Web: en.urovo.com |
| A4 | PRICE LIST |
| A5 | Series |
| B5 | Picture |
| C5 | Model |
| D5 | Configuration |
| E5 | Remark |
| F5 | Sample Price（USD） |
| G5 | Unit Price(USD)        (MOQ 50pcs) |
| H5 | Unit Price(USD)        (MOQ 500pcs) |
| A6 | DT66 |
| C6 | DT66 |
| D6 | Qualcomm Octa-Core 2.4 GHz, \nAndroid 13/15 OS, 6.5 Inch Display, \nRAM: 4GB ROM: 64GB /Optional 8+128G\nBattery: 5000mAh, Support Hot Swap, Support smart battery\nCamera:  Front 5MP, Rear 13MP \n1D/2D Barcode Scanner; Backside and In-Display NFC\nWi-Fi:  Wi-Fi 6E, 2.4GHz/5GHz, support 2x2 MU-MIMO\nBT:  BT5.2;  5G/4G/3G/2G;\nStandard Accessories: Power Adapter*1, USB Cable*1 |
| E6 | UROVO SE2030 |
| F6 | 315 |
| G6 | 300 |
| H6 | 284 |
| B7 | Optional Accessories |
| C7 | BTY-DT66-01 |
| D7 | Spare Battery |
| E7 | 14 |
| C8 | SPF-DT66-01 |
| D8 | Screen Protector Film |
| E8 | 4 |
| C9 | BC-DT66-01 |
| D9 | Boot Case（TPU） |
| E9 | 8 |
| C10 | SH-DT66-01 |
| D10 | Nylon Holster |
| E10 | 12 |
| C11 | TRG-DT66-02 |
| D11 | Trigger Handle |
| E11 | 18 |
| C12 | CRD-DT66-02 |
| D12 | Single Charging Cradle |
| E12 | 32 |
| C13 | CRD-DT66-05 |
| D13 | 4-Slot Battery Charging Cradle |
| E13 | 60 |
| C14 | CRD-DT66-08 |
| D14 | 5-Slot Charging Cradle (5 devices) |
| E14 | 95 |
| C15 | CRD-DT66-11 |
| D15 | 5-Slot Charging Cradle (4 devices+4 batteries) |
| E15 | 135 |
| A16 | CT58C |
| C16 | CT58C |
| D16 | MTK Octa-Core 2.0 GHz, \nAndroid 12/14 OS, 5.5 Inch Display, \nRAM: 4GB ROM: 64GB; 5000mAh Battery; \nCamera:  Front 5MP, Rear 13MP \n1D/2D Barcode Scanner, NFC \nWi-Fi:  2.4GHz/5GHz, BT:  BT5.0\nStandard Accessories: Power Adapter*1, USB Cable*1 |
| E16 | SE2030 |
| F16 | 150 |
| G16 | 145 |
| H16 | 140 |
| B17 | Optional Accessories |
| C17 | BTY-CT58S-02 |
| D17 | Spare Battery |
| E17 | 14 |
| C18 | SPF-CT58-02 |
| D18 | Screen Protector Film |
| E18 | 4 |
| C19 | BC-CT58S-01 |
| D19 | Boot Case |
| E19 | 8 |
| C20 | HS-CT58S-01 |
| D20 | Hand Strap |
| E20 | 8 |
| C21 | CRD-CT58S-04 |
| D21 | Single Charging Cradle |
| E21 | 32 |
| C22 | TRG-CT58S-02 |
| D22 | Trigger Handle |
| E22 | 18 |
| C23 | CRD-CT58-03 |
| D23 | 4-Slot Battery Charging Cradle |
| E23 | 95 |
| C24 | DT50 Pro |
| D24 | Qualcomm Octa-Core 2.4 GHz, \nAndroid 16 OS, 5.7 Inch Display, \nRAM：4GB ROM：64GB / Optional 6+64G\n5000mAh Battery\nCamera: Front 5MP, Rear 13MP \n1D/2D Barcode Scanner, NFC \nWifi 6E, BT: BT5.3\nStandard Accessores:  Power Adapter*1, USB Cable*1 |
| E24 | SE2030 |
| F24 | 279 |
| G24 | 261 |
| H24 | 251 |
| A25 | DT50 |
| C25 | DT50S |
| D25 | Qualcomm Octa-Core 2.45 GHz, \nAndroid 11/13 OS, 5.7 Inch Display, \nRAM：4GB ROM：64GB /Optional 8+128G\n5000mAh Battery\nCamera: Front 5MP, Rear 13MP \n1D/2D Barcode Scanner, NFC \nWifi: 2.4GHz/5GHz, BT: BT5.0\nStandard Accessores:  Power Adapter*1, USB Cable*1 |
| E25 | SE2030 |
| F25 | 273 |
| G25 | 260 |
| H25 | 246 |
| C26 | DT50P |
| D26 | Qualcomm 4290 Octa-Core 2.45 GHz, \nAndroid 11/13 OS, 5.7 Inch Display, \nRAM：4GB ROM：64GB,   9000mAh Battery\nCamera: Front 5MP, Rear 13MP \n1D/2D Barcode Scanner, NFC \nWifi: 2.4GHz/5GHz, BT: BT5.0\nUHF(15-20M)                                                                         \n Accessories: Power Adapter*1, USB Cable*1 |
| E26 | SE2030 |
| F26 | 380 |
| G26 | 361 |
| H26 | 342 |
| B27 | Optional Accessories |
| C27 | TRG-DT50-06 |
| D27 | RFID Gun（UHF）- RFDT50 |
| E27 | 290 |
| C28 | BC-DT50-01 |
| D28 | Boot Case |
| E28 | 8 |
| C29 | CRD-DT50 |
| D29 | Single-Slot Cradle(one device+one battery) |
| E29 | 32 |
| C30 | CRD-DT50-07 |
| D30 | Quad-Slot Battery Cradle |
| E30 | 60 |
| C31 | CRD-DT50-05 |
| D31 | Five-Slot Device Cradle |
| E31 | 95 |
| C32 | CRD-DT50-06 |
| D32 | Five-Slot Device Cradle with Ethernet interface |
| E32 | 105 |
| C33 | CRD-DT50-08 |
| D33 | Quad-Slot Battery Cradle+Quad-slot battery cradle |
| E33 | 135 |
| C34 | TRG-DT50-01 |
| D34 | Scan Trigger |
| E34 | 18 |
| C35 | FPM-DT50 |
| D35 | Optical Fingerprint Module |
| E35 | 50 |
| C36 | SPF-DT50-01 |
| D36 | Screen Protector Film |
| E36 | 4 |
| C37 | HS-DT50-03 |
| D37 | Hand Strap |
| E37 | 8 |
| A38 | Optional Config |
| D38 | HS7:+15USD/pcs |
| D39 | 8+128G:+22USD/pcs |
| A40 | Warranty |
| D40 | 1 year factory warranty for main device; 6 months for accessories |
| A41 | Lead Time |
| D41 | Sample:2-10 working days;  Bulk order:20-40 working days |
| A42 | Payment Terms |
| D42 | Sample: 100% T/T; Bulk order: T/T 30% in advance upon order,rest 70% before shippment. |
| A43 | Trade Term |
| D43 | EXW SHENZHEN |

Drawing anchors (from cell → media):

| From cell | Media | Drawing name |
| --- | --- | --- |
| B25 | image1.png | 图片 6 |
| B26 | image2.png | 图片 1 |
| D27 | image3.png | ID_42E224D13E36471CB54EC12B0DDC505B |
| D29 | image4.png | ID_3C67F1E2806440C598FD50FF7CC30CB6 |
| D30 | image5.png | ID_ABC98C8F7EEA4EC8BA4C28D45E03B602 |
| D31 | image6.png | ID_C23B11E0126B4CD7BEB3E15007232A65 |
| D34 | image7.png | ID_D6E3F8F44F7A4397B7C89A59F483A6FF |
| D35 | image8.png | ID_D70E3D49176B4C2598C6924D8564BBFA |
| D36 | image9.png | 图片 7 |
| D37 | image10.png | ID_298BEF999912481B9C4B1D35B1642D37 |
| B6 | image11.png | 图片 1 |
| B16 | image12.png | 图片 2 |
| D11 | image7.png | ID_D6E3F8F44F7A4397B7C89A59F483A6FF |
| D10 | image13.png | 图片 3 |
| D11 | image14.png | 图片 4 |
| D13 | image15.png | 图片 5 |
| D14 | image16.png | 图片 6 |
| D15 | image17.png | 图片 7 |
| D20 | image14.png | 图片 8 |
| D22 | image18.png | 图片 9 |
| D23 | image19.png | 图片 10 |
| D9 | image20.png | 图片 3 |
| B24 | image21.png | 图片 4 |

### DT610，DT630

`nonempty=34 formulas=0 merged=12 images=3`

`merged_ranges=A10:C10;A4:H4;A3:H3;D8:H8;A11:C11;D10:H10;A8:C8;A2:H2;D11:H11;A9:C9;A1:H1;D9:H9`

| Cell | Value |
| --- | --- |
| A1 | UROVO TECHNOLOGY CO., LTD. |
| A2 |  36F, High-Tech Zone Union Tower, No.63,Xuefu Road, Nanshan district, Shenzhen, Guangdong, China |
| A3 |  Fax :  +86-755-23636919       Tel:  +86-755-23636919      Web: en.urovo.com |
| A4 | PRICE LIST |
| A5 | Series |
| B5 | Picture |
| C5 | Model |
| D5 | Configuration |
| E5 | Remark |
| F5 | Sample Price（USD） |
| G5 | Unit Price(USD)        (MOQ 50pcs) |
| H5 | Unit Price(USD)(MOQ 500pcs) |
| A6 | DT610 |
| C6 | DT610 |
| D6 | Octa-core, 2.0Ghz/2.9 GHz, \nAndroid 15 OS, 6-inch FHD+ screen, \nRAM: 8GB ROM: 128GB /Optional 12+256G\nBattery: 4000mAh, Support Hot Swap, Support smart battery\nCamera:  Front 8MP, Rear 16MP \n1D/2D Barcode Scanner; \nsupports UWB for device locating\nStandard Accessories: Power Adapter*1, USB Cable*1 |
| E6 | UROVO SE2030 S1-SR620W |
| F6 | 451 |
| G6 | 429 |
| H6 | 406 |
| A7 | DT630 |
| C7 | DT630 |
| D7 | Octa-core, 2.5 GHz, \nAndroid 15 OS, 6.58 Inch Display, \nRAM：8GB ROM：128GB ,  4500mAh Battery\nCamera: Rear 50MP autofocus; flash LED, PDAF; Torch mode;Front : 8MP Fixed, FF;  \n1D/2D Barcode Scanner, NFC \nWifi 6E, BT: BT5.4\nStandard Accessores:  Power Adapter*1, USB Cable*1 |
| E7 | SE630 |
| F7 | 378 |
| G7 | 360 |
| H7 | 340 |
| A8 | Warranty |
| D8 | 1 year factory warranty for main device; 6 months for accessories |
| A9 | Lead Time |
| D9 | Sample:2-10 working days;  Bulk order:20-40 working days |
| A10 | Payment Terms |
| D10 | Sample: 100% T/T; Bulk order: T/T 30% in advance upon order,rest 70% before shippment. |
| A11 | Trade Term |
| D11 | EXW SHENZHEN |

Drawing anchors (from cell → media):

| From cell | Media | Drawing name |
| --- | --- | --- |
| B6 | image22.png | 图片 26 |
| B7 | image23.png | 图片 27 |
| B7 | image24.png | 图片 28 |

### P8100, P8100P，UPAD，U100

`nonempty=70 formulas=0 merged=25 images=9`

`merged_ranges=D20:H20;D19:H19;E16:H16;A18:C18;E7:H7;A21:C21;A1:H1;A11:A16;D21:H21;A6:A9;A17:C17;B7:B9;A20:C20;D17:H17;E14:H14;B13:B16;A3:H3;A19:C19;E8:H8;A2:H2;D18:H18;E13:H13;A4:H4;E9:H9;E15:H15`

| Cell | Value |
| --- | --- |
| A1 | UROVO TECHNOLOGY CO., LTD. |
| A2 |  36F, High-Tech Zone Union Tower, No.63,Xuefu Road, Nanshan district, Shenzhen, Guangdong, China |
| A3 |  Fax :  +86-755-23636919       Tel:  +86-755-23636919      Web: en.urovo.com |
| A4 | PRICE LIST |
| A5 | Series |
| B5 | Picture |
| C5 | Model |
| D5 | Configuration |
| E5 | Remark |
| F5 | Sample Price |
| G5 | Unit Price(USD)        (MOQ 100pcs) |
| H5 | Unit Price(USD)        (MOQ 500pcs) |
| A6 | UPAD |
| B6 | #NAME? |
| C6 | UPAD |
| D6 | Octa-core, 2.2 GHz\nAndroid 16 OS, 11 Inch Display, \nRAM: 4GB ROM: 64GB / Optional 8+128G   \n8000mAh Battery\nCamera:  Front 8MP, Rear 16MP \n1D/2D Barcode Scanner, NFC \nStandard Accessories: Power Adapter*1, USB Cable*1 |
| E6 | SE2030 S1-SR620W |
| F6 | 290 |
| G6 | 276 |
| H6 | 261 |
| B7 | Optional Accessories |
| C7 | BC-UPad-01 |
| D7 | Protective Case |
| C8 | ACC-UPad-01 |
| D8 | Shoulder Strap |
| C9 | SPF-UPad-01 |
| D9 | Explosion-proof Film |
| A10 | U100 |
| B10 | #NAME? |
| C10 | U100 |
| D10 | Quad-core A53 2.0GHz\nAndroid 13\nRAM: 3GB  ROM: 32GB\n10.1 Inch Display\nSpeaker(3W), MIC\nWIFI 2.4GHz/5GHz，BT5.0\n8MP AF Camera（Optional UHF）\nBuilt-in ScannerSupporting 1D/2D Barcode Reading |
| E10 | / |
| F10 | 200 |
| G10 | 190 |
| H10 | 180 |
| A11 | P8100P Series |
| C11 | P8100P 4G |
| D11 | Qualcomm Octa-Core 2.45 GHz, \nAndroid 13.0 OS, 10 Inch Display, \nRAM: 4GB ROM: 64GB / RAM: 8GB ROM: 128GB,   \n10000mAh Battery\nCamera:  Front 5MP, Rear 13MP \n1D/2D Barcode Scanner, NFC \nWi-Fi:  2.4GHz/5GHz, Wi-Fi 6 Ready, BT:  BT5.0 \nStandard Accessories: Power Adapter*1, USB Cable*1 |
| E11 | SE2030 |
| F11 | 333 |
| G11 | 317 |
| H11 | 300 |
| C12 | P8100P 5G |
| D12 | Qualcomm Octa-Core 2.4GHz, \nAndroid 13.0 OS, 10 Inch Display, \nRAM: 4GB ROM: 64GB / RAM: 8GB ROM: 128GB,   \n10000mAh Battery\nCamera:  Front 5MP, Rear 13MP \n1D/2D Barcode Scanner, NFC \nWi-Fi:  Wi-Fi 6E, 2.4GHz/5GHz, \nBT:  BT5.2;  5G/4G/3G/2G;\nStandard Accessories: Power Adapter*1, USB Cable*1 |
| E12 | SE2030 |
| F12 | 380 |
| G12 | 361 |
| H12 | 342 |
| B13 | Optional Accessories |
| C13 | CRD-P8100P |
| D13 | cradle |
| E13 | 28 |
| C14 | HS-P8100P |
| D14 | Hand strap |
| E14 | 8 |
| C15 | CP-P8100P-01 |
| D15 | Carrying Pouch（Without shoulder strap） |
| E15 | 12 |
| C16 | CP-P8100P-02 |
| D16 | Carrying Pouch（With shoulder strap） |
| E16 | 14.5 |
| D17 | 8+128G:+22USD/pcs |
| A18 | Warranty |
| D18 | 1 year factory warranty for main device; 6 months for accessories |
| A19 | Lead Time |
| D19 | Sample:2-10 working days;  Bulk order:20-40 working days |
| A20 | Payment Terms |
| D20 | Sample: 100% T/T; Bulk order: T/T 30% in advance upon order,rest 70% before shippment. |
| A21 | Trade Term |
| D21 | EXW SHENZHEN |

Drawing anchors (from cell → media):

| From cell | Media | Drawing name |
| --- | --- | --- |
| A1 | image25.png | Picture 1292 |
| D15 | image26.png | 图片 1 |
| D16 | image27.png | 图片 2 |
| D14 | image28.png | ID_87B2373DF28D4E3E91273B2A94F1D6F7 |
| D13 | image29.png | ID_4A101E51A09242C287A3A6D8D9A07AA4 |
| A11 | image30.png | 图片 1 |
| B12 | image30.png | 图片 2 |
| D6 | image31.png | 图片 2 |
| D7 | image32.png | 图片 3 |

### RT40,CT48C

`nonempty=95 formulas=0 merged=47 images=16`

`merged_ranges=B19:B25;H6:H7;B17:D17;I14:I16;E25:H25;A1:H1;A14:A16;D31:H31;E22:H22;A33:C33;E18:H18;A32:C32;E12:H12;B8:B13;E21:H21;G6:G7;D27:H27;E6:E7;D32:H32;A6:A13;B6:B7;E24:H24;A3:H3;E17:H17;E23:H23;E8:H8;D6:D7;A2:H2;A31:C31;E20:H20;C14:C16;D28:H28;A30:C30;E19:H19;E10:H10;E13:H13;A4:H4;D30:H30;E9:H9;D33:H33;D29:H29;B18:D18;A26:C29;C6:C7;E11:H11;F6:F7;D26:H26`

| Cell | Value |
| --- | --- |
| A1 | UROVO TECHNOLOGY CO., LTD. |
| A2 |  36F, High-Tech Zone Union Tower, No.63,Xuefu Road, Nanshan district, Shenzhen, Guangdong, China |
| A3 |  Fax :  +86-755-23636919       Tel:  +86-755-23636919      Web: en.urovo.com |
| A4 | PRICE LIST |
| A5 | Series |
| B5 | Picture |
| C5 | Model |
| D5 | Configuration |
| E5 | Remark |
| F5 | Sample Price |
| G5 | Unit Price(USD)        (MOQ 100pcs) |
| H5 | Unit Price(USD)        (MOQ 500pcs) |
| A6 | CT48C |
| C6 | CT48C |
| D6 | MTK Octa-Core 2.0GHz, \nAndroid 12/14 OS, 4.0 inch Display, \n RAM: 4GB ROM: 64GB,    5000mAh Battery, gyroscope（optional）\nCamera:  Front 2MP, Rear 13MP \n1D/2D Barcode Scanner, NFC (optional)\nWi-Fi:  2.4GHz/5GHz, BT:  BT5.0\n4G/3G/2G\nStandard Accessories: Power Adapter*1, USB Cable*1 |
| E6 | SE2030 |
| F6 | 140 |
| G6 | 130 |
| H6 | 115 |
| B8 | Optional \nAccessories |
| C8 | BTY-CT48-50-03 |
| D8 | Spare Battery |
| E8 | 14 |
| C9 | SPF-CT48-02 |
| D9 | Screen Protector Film |
| E9 | 4 |
| C10 | BC-CT48-01 |
| D10 | Boot case |
| E10 | 8 |
| C11 | HS-CT48-01 |
| D11 | Hand Strap |
| E11 | 8 |
| C12 | CRD-CT48-07 |
| D12 | Single Charging Cradle |
| E12 | 32 |
| C13 | CRD-CT48-05 |
| D13 | 4-Slot Battery Charging Cradle |
| E13 | 95 |
| A14 | RT40S  |
| C14 | SQ47S |
| D14 | Qualcomm Octa-Core 2.45GHz, \nAndroid 13.0 OS\nRAM: 4GB ROM: 64GB,   5200mAh Battery\nCamera: 13MP Rear\n1D/2D Barcode Scanner, NFC \nWi-Fi:  2.4GHz/5GHz, BT:  5.0\nSupport Wi-Fi 6, 2x2 MU-MIMO\n29keys\nStandard Accessories: Power Adapter*1, USB Cable*1 |
| E14 | SE2030 |
| F14 | 273 |
| G14 | 260 |
| H14 | 246 |
| I14 | 38keys and 51keys RT40S is available in both room temperature and Cold chain version |
| D15 | Qualcomm Octa-Core 2.45GHz, \nAndroid 13.0 OS\nRAM: 4GB ROM: 64GB,   5200mAh Battery\nCamera: 13MP Rear\n1D/2D Barcode Scanner, NFC \nWi-Fi:  2.4GHz/5GHz, BT:  5.0\nSupport Wi-Fi 6, 2x2 MU-MIMO\n38keys,\nStandard Accessories: Power Adapter*1, USB Cable*1 |
| E15 | SE2030 |
| F15 | 278 |
| G15 | 265 |
| H15 | 251 |
| D16 | Qualcomm Octa-Core 2.45GHz, \nAndroid 13.0 OS; RAM: 4GB ROM: 64GB,   \nBattery: 5200mAh, \nCamera: 13MP Rear\n1D/2D Barcode Scanner, NFC \nWi-Fi:  2.4GHz/5GHz, BT:  5.0\nSupport Wi-Fi 6, 2x2 MU-MIMO\n51keys\nStandard Accessories: Power Adapter*1, USB Cable*1 |
| E16 | SE2030 |
| F16 | 283 |
| G16 | 270 |
| H16 | 256 |
| B17 | Add Heating Functions(Cold chain) |
| E17 | 10 |
| B18 | Add handle |
| E18 | 10 |
| B19 | Optional Accessories |
| C19 | CP-RT40-01 |
| D19 | Carrying Pouch |
| E19 | 15 |
| C20 | HS-RT40-01 |
| D20 | Hand strap |
| E20 | 6 |
| C21 | CRD-RT40 |
| D21 | Single-Slot Cradle(one device+one battery) |
| E21 | 28 |
| C22 | CRD-RT40-04 |
| D22 | Quad-Slot Battery Cradle |
| E22 | 55 |
| C23 | CRD-RT40-05 |
| D23 | Five-Slot Device Cradle |
| E23 | 95 |
| C24 | CRD-RT40-08 |
| D24 | Quad-Slot Battery Cradle+\nQuad-slot device cradle |
| E24 | 135 |
| C25 | BC-RT40-01 |
| D25 | Boot case |
| E25 | 10 |
| A26 | Optional Config |
| D26 | HS7:+15USD/pcs |
| D27 |  5500(Mid-to Long distance scanner):+100USD/pcs |
| D28 |  5800(Long distance scanner):+180USD/pcs |
| D29 | 8+128G:+22USD/pcs |
| A30 | Warranty |
| D30 | 1 year factory warranty for main device; 6 months for accessories |
| A31 | Lead Time |
| D31 | Sample:2-10 working days;  Bulk order:20-40 working days |
| A32 | Payment Terms |
| D32 | Sample: 100% T/T; Bulk order: T/T 30% in advance upon order,rest 70% before shippment. |
| A33 | Trade Term |
| D33 | EXW SHENZHEN |

Drawing anchors (from cell → media):

| From cell | Media | Drawing name |
| --- | --- | --- |
| A1 | image25.png | Picture 1292 |
| D19 | image33.png | 图片 1 |
| D19 | image34.png | 图片 2 |
| B6 | image35.png | 图片 2 |
| B6 | image36.png | 图片 3 |
| B14 | image37.png | ID_2DCD343A39154627B521F03882104B10 |
| D20 | image38.png | ID_9177901D34EF4ECBB775347D83EACA68 |
| D21 | image39.png | ID_23DE85FD07604C63AF3E2714DD28768C |
| D22 | image40.png | ID_3D27C435AD5A425997D21B50392DF615 |
| D23 | image41.png | ID_2F669C925E9545B3996ED7088C85BC36 |
| D24 | image42.png | ID_677D5177D2C84A4698E8F59DD2B5E6C0 |
| D25 | image43.png | ID_023FC6721414486E9E53B27D63BD2465 |
| B15 | image44.png | 图片 2 |
| D12 | image45.png | 图片 1 |
| D13 | image19.png | 图片 2 |
| B16 | image46.png | 图片 1 |

### POS

`nonempty=62 formulas=0 merged=15 images=3`

`merged_ranges=A13:C13;A1:G1;A9:A10;A3:G3;A14:C14;D16:G16;A4:G4;A7:A8;A2:G2;D15:G15;D13:G13;A15:C15;A11:A12;A16:C16;D14:G14`

| Cell | Value |
| --- | --- |
| A1 | UROVO TECHNOLOGY CO., LTD. |
| A2 |  36F, High-Tech Zone Union Tower, No.63,Xuefu Road, Nanshan district, Shenzhen, Guangdong, China |
| A3 |  Fax :  +86-755-23636919       Tel:  +86-755-23636919      Web: en.urovo.com |
| A4 | PRICE LIST |
| A5 | Series |
| B5 | Picture |
| C5 | Model |
| D5 | Configuration |
| E5 | Sample Price（USD） |
| F5 | Unit Price(USD)        (MOQ 50pcs) |
| G5 | Unit Price(USD)        (MOQ 500pcs) |
| A6 | i9100 |
| C6 | i9100 |
| D6 | Quad-core 2.0 GHz, \nAndroid 13 OS, 5.5 Inch Display, \nRAM: 2GB ROM: 16GB\nCamera:  Standard No Front, Rear 2MP\n         Optional: 2MP front camera\n         Optional: 5MP or 16MP rear camera\nOptional ESIM.MIC and Finger Module\nStandard Accessories: Power Adapter*1, USB Cable*1 |
| E6 | 110 |
| F6 | 105 |
| G6 | 98 |
| A7 | i9200 |
| C7 | i9200 EMV |
| D7 | Quad-core 2.0 GHz, Optional Octa-core 2.0GHz\nAndroid 13 OS, 5.5 Inch Display, \nRAM: 2GB ROM: 16GB /Optional 3+32G\nCamera:  Standard No Front, Rear 5MP\n         Optional: 2MP front camera\n         Optional: 16MP rear camera\nOptional ESIM.MIC and Finger Module\nStandard Accessories: Power Adapter*1, USB Cable*1 |
| E7 | 110 |
| F7 | 105 |
| G7 | 98 |
| C8 | i9200  |
| D8 | Quad-core 2.0 GHz, Optional Octa-core 2.0GHz\nAndroid 13 OS, \n5.5 Inch Display, \nRAM: 3GB ROM: 32GB\nCamera:  Standard No Front, Rear 5MP\n         Optional: 2MP front camera\n         Optional: 16MP rear camera\nStandard Receipt Printing,Optional Label Printing\nStandard Accessories: Power Adapter*1, USB Cable*1 |
| E8 | 100 |
| F8 | 95 |
| G8 | 88 |
| A9 | i9600 |
| B9 | #NAME? |
| C9 | i9600 |
| D9 | Quad-core A53 2.0GHz Optional Octa-core 2.0GHz\nAndroid 13 OS, \n6.745 Inch Display, \nRAM: 2GB ROM: 16GB/Optional 3+32G\nOptional Customer Display;\nCamera:  Standard No Front, Rear 5MP\nOptional Top  Camera 0.3MP\n         Optional: 2MP front camera(cannot support top and front camera at the same time)\n         Optional: 16MP rear camera\nStandard Accessories: Power Adapter*1, USB Cable*1 |
| E9 | 134 |
| F9 | 128 |
| G9 | 120 |
| B10 | #NAME? |
| C10 | i9600 mini |
| D10 | Quad-core 2.0GHz Optional Octa-core 2.0GHz\nAndroid 13 OS, \n6.745 Inch Display, \nRAM: 2GB ROM: 16GB/Optional 3+32G\nCamera:  Standard No Front, Rear 5MP\n         Optional: 2MP front camera\nStandard Accessories: Power Adapter*1, USB Cable*1 |
| E10 | 128 |
| F10 | 122 |
| G10 | 115 |
| A11 | i5300 |
| B11 | #NAME? |
| C11 | i5300 |
| D11 | Quad-core 2.0GHz\nAndroid 13 OS, \n3.5 Inch Display, \nRAM: 2GB ROM: 16GB\nCamera:  Standard No Front Camera, No Rear Camera,with 0.3MP Top Camera\n         Optional: 0.3MP front camera\nOptional:5MP Rear Camera(cannot support top and front camera at the same time)\nStandard Accessories: Power Adapter*1, USB Cable*1 |
| E11 | 90 |
| F11 | 85 |
| G11 | 80 |
| B12 | #NAME? |
| C12 | i5300L |
| D12 | Quad-core 2.0GHz\nAndroid 13 OS, \n5.5 Inch Display, \nRAM: 2GB ROM: 16GB、Optional 3+32G\nCamera:  Standard No Front Camera, No Rear Camera,with 0.3MP Top Camera\n         Optional: 0.3MP front camera\nOptional:5MP Rear Camera(cannot support top and front camera at the same time)\nStandard Accessories: Power Adapter*1, USB Cable*1 |
| E12 | 95 |
| F12 | 90 |
| G12 | 85 |
| A13 | Warranty |
| D13 | 1 year factory warranty for main device; 6 months for accessories |
| A14 | Lead Time |
| D14 | Sample:2-10 working days;  Bulk order:20-40 working days |
| A15 | Payment Terms |
| D15 | Sample: 100% T/T; Bulk order: T/T 30% in advance upon order,rest 70% before shippment. |
| A16 | Trade Term |
| D16 | EXW SHENZHEN |

Drawing anchors (from cell → media):

| From cell | Media | Drawing name |
| --- | --- | --- |
| B6 | image47.png | 图片 24 |
| B7 | image48.png | 图片 25 |
| B8 | image49.png | 图片 26 |

### U2S, SR5600Pro，SR5750，S716

`nonempty=90 formulas=0 merged=44 images=19`

`merged_ranges=E26:H26;A4:G4;E16:H16;A27:C27;A14:A16;G17:H17;E22:H22;E18:H18;G7:H7;A25:A26;E12:H12;C25:C26;B8:B13;E21:H21;I21:I22;D27:H27;G6:H6;A29:C29;A6:A13;E24:H24;B15:B16;A28:C28;E23:H23;A1:G1;E8:H8;A17:A20;E20:H20;G5:H5;D28:H28;G14:H14;A30:C30;E19:H19;E10:H10;E13:H13;D30:H30;E9:H9;B18:B24;A3:G3;G25:H25;D29:H29;B25:B26;A2:G2;E15:H15;E11:H11`

| Cell | Value |
| --- | --- |
| A1 | UROVO TECHNOLOGY CO., LTD. |
| A2 |  36F, High-Tech Zone Union Tower, No.63,Xuefu Road, Nanshan district, Shenzhen, Guangdong, China |
| A3 |  Fax :  +86-755-23636919       Tel:  +86-755-23636919      Web: en.urovo.com |
| A4 | PRICE LIST |
| A5 | Series |
| B5 | Picture |
| C5 | Model |
| D5 | Configuration |
| E5 | Sample Price |
| F5 | Unit Price(USD)        (MOQ 100pcs) |
| G5 | Unit Price(USD)        (MOQ 500pcs) |
| A6 | U2S |
| C6 | SQ46S |
| D6 | 1. Qualcomm Quad Core 2.4GHz, \n2. Android 14 OS,\n3. 4GB RAM/64GB ROM,\n4. 4 inch display\n5. Standard Accessories: Power Adapter*1, Main Battery*1, USB-Magnetic pogo pin data Cable*1 |
| E6 | 267 |
| F6 | 254 |
| G6 | 240 |
| C7 | R70 |
| D7 | 1. Bluetooth4.0 (Compatible Android OS, iOS, Windows) , 2.4Ghz Wireless\n2. 1D/ 2D Barcode Engine( Zebra 2D)\n3. 1000mAh Battery \n4. Standard Accessories:  Power Adapter*1, USB Cable*1, Wireless Receiver*1 |
| E7 | 90 |
| F7 | 80 |
| G7 | 70 |
| B8 | Optional Accessories |
| C8 | CRD-U2 |
| D8 | Dual Charging Dock |
| C9 | CRD-U2S-04 |
| D9 | U2S Battery 20-unit Charger |
| C10 | SW-U2 |
| D10 | Extra Spare Wristband |
| E10 | 15 |
| C11 | BA-U2 |
| D11 | Extra Battery |
| E11 | 20 |
| C12 | PA-U2 |
| D12 | Extra Power Adapter |
| E12 | 10 |
| C13 | CRD-U2-10 |
| D13 | U2+R7 Charging Dock |
| E13 | 45 |
| A14 | SR5750 |
| C14 | SR5750 |
| D14 | 1. Qualcomm Quad Core 2.0GHz, \n2. Android 13 OS,\n3. 4GB RAM/64GB ROM,\n4. 2.1 inch display\n5.WIFI 6 and BT5.3\n6. Standard Accessories: Power Adapter*1, Main Battery*1, USB-Magnetic pogo pin data Cable*1 |
| E14 | 217 |
| F14 | 207 |
| G14 | 195 |
| B15 | Optional Accessories |
| C15 | HS-SR5750-01 |
| D15 | Watch Band |
| C16 | ACC-PDA-04 |
| D16 | Neck Strap |
| A17 | SR5600 Pro |
| C17 | SR5600 Pro |
| D17 | 2D ring sanner, cable, adaptor\nBluetooth 5.0（Compatible Android OS, IOS, Windows）\n1D/2D Barcode Engine , NFC(tap to pair)\n3.8V 950mAh Battery\nStandard Accessories: Power Adapter*1, USB Cable*1 |
| E17 | 85 |
| F17 | 75 |
| G17 | 65 |
| B18 | Optional Accessories |
| C18 | CRD-SR5600-04 |
| D18 | FOUR-Slot Device Cradle |
| E18 | 56 |
| C19 | CRD-SR5600-06 |
| D19 | SIX-Slot Battery Cradle |
| E19 | 70 |
| C20 | CRD-SR5600-14 |
| D20 | 20-Slot Host Charging Dock |
| C21 | CRD-SR5600-15 |
| D21 | 30-Slot Host Charging Dock |
| C22 | BUT-SR5600-05 |
| D22 | Ring |
| C23 | ACC-SR5600-03 |
| D23 | Lanyard |
| E23 | 8 |
| C24 | CRD-SR5600-06 |
| D24 | Direct Charger |
| A25 | S716 |
| C25 | S716 |
| D25 | wireless barcode scanner                                                                                                       \n1. Processor 32-bit CPU\n2. Support standard 1D and 2D\nbarcodes Camera: 640X480 CMOS, 30fps 3.\nStandard Accessores: Power Adapter*1, USB\nCable*1 |
| E25 | 22 |
| F25 | 20 |
| G25 | 18 |
| D26 | Base charger for S716 |
| E26 | 5 |
| A27 | Warranty |
| D27 | 1 year factory warranty for main device; 6 months for accessories |
| A28 | Lead Time |
| D28 | Sample:2-10 working days;  Bulk order:20-40 working days |
| A29 | Payment Terms |
| D29 | Sample: 100% T/T; Bulk order: T/T 30% in advance upon order,rest 70% before shippment. |
| A30 | Trade Term |
| D30 | EXW SHENZHEN |

Drawing anchors (from cell → media):

| From cell | Media | Drawing name |
| --- | --- | --- |
| A1 | image25.png | Picture 1292 |
| B25 | image50.png | 图片 1 |
| D10 | image51.png | 图片 6 |
| B17 | image52.jpeg | 图片 2 |
| D18 | image53.png | ID_55ECA2768F55440497E3D01275D4A83F |
| D19 | image54.png | ID_C8D4125F0E7D4B5DBADABD26AD89C80C |
| B6 | image55.png | 图片 1 |
| D8 | image56.png | 图片 2 |
| D9 | image57.png | 图片 3 |
| B14 | image58.png | 图片 4 |
| D15 | image59.png | 图片 5 |
| D16 | image60.png | 图片 7 |
| B7 | image61.png | ID_ECFDBA155B3748C2954837508B4F8D38 |
| D13 | image62.png | 图片 10 |
| D20 | image63.png | 图片 12 |
| D21 | image64.png | 图片 13 |
| D22 | image65.png | 图片 14 |
| D23 | image66.png | 图片 15 |
| D24 | image67.png | 图片 16 |

### Printers

`nonempty=86 formulas=0 merged=36 images=9`

`merged_ranges=A25:C25;E13:G13;C20:C21;A4:G4;B8:B9;A27:C27;A14:A18;E15:G15;A26:C26;C22:C23;E11:G11;A6:A9;D27:H27;B6:B7;E16:G16;A1:G1;E22:G22;A22:A23;E12:G12;B11:B13;B15:B18;E18:G18;A20:A21;B20:B21;E21:G21;A24:C24;A10:A13;D25:H25;A3:G3;B22:B23;E23:G23;D24:H24;E17:G17;A2:G2;E20:G20;D26:H26`

| Cell | Value |
| --- | --- |
| A1 | UROVO TECHNOLOGY CO., LTD. |
| A2 |  36F, High-Tech Zone Union Tower, No.63,Xuefu Road, Nanshan district, Shenzhen, Guangdong, China |
| A3 |  Fax :  +86-755-23636919       Tel:  +86-755-23636919      Web: en.urovo.com |
| A4 | PRICE LIST |
| A5 | Series |
| B5 | Pictures |
| C5 | Model |
| D5 | Configuration |
| E5 | Sample Price |
| F5 | Unit Price(USD)       (MOQ:100pcs) |
| G5 | Unit Price (USD)      (MOQ:500pcs) |
| A6 | K388Pro |
| C6 | K388 Pro |
| D6 | Octa-core 2.4GHz\nAndroid 14\n4+64G\n5.5-inch screen / 3000mAh battery (10.8V)\nPaper Width 30-58mm，PaperRoll≤60mm\nSupports 4G (domestic bands only) / Wi-Fi 6E / Bluetooth 5.0\nStandard Accessries：Adapter,Battery，Data cable |
| E6 | 772 |
| F6 | 734 |
| G6 | 695 |
| C7 | K388 Pro（RFID） |
| D7 | Octa-core 2.4GHz\nAndroid 14\n4+64G\n5.5-inch screen / 3000mAh battery (10.8V)\nPaper Width 30-58mm，PaperRoll≤60mm\nSupports 4G (domestic bands only) / Wi-Fi 6E / Bluetooth 5.0\nStandard Accessries：Adapter,Battery，Data cable |
| E7 | 1010 |
| F7 | 960 |
| G7 | 909 |
| B8 | Optional Accessories |
| C8 | BTY-K388 Pro-30-01 |
| D8 | Spare Battery |
| C9 | CRD-K388 Pro-02 |
| D9 | Four-Battery Charger/12V 5A |
| A10 | K329 |
| C10 | K329 |
| D10 | Print Mode: Direct thermal \nMaximum Print Width:3"/72mm \nMaximum Print Speed:120mm per second \nResolution:203dpi ,8dots/mm \nPower:2600mAh/7.4V Rechargeable lithium polymer battery \nBluetooth: 2.1+4.2(BLE)\nCompatible with Android OS, IOS, Windows \nStandard Accessories: Power Adapter*1, Main Battery*1,USB Cable*1 |
| E10 | 70 |
| F10 | 60 |
| G10 | 55 |
| B11 | Optional Accessories |
| C11 | CH-K329 |
| D11 | Carrying Case / Holster |
| E11 | 10 |
| C12 | PA-K329 |
| D12 | Extra Power Adapter |
| E12 | 10 |
| C13 | BA-K329 |
| D13 | Extra Battery |
| E13 | 18 |
| A14 | K419 |
| C14 | K419 |
| D14 | Print Mode: Direct thermal \nMaximum Print Width:4"/104mm \nMaximum Print Speed:55mm per second\nResolution:203dpi ,8dots/mm \nPower:2600mAh/7.4V Rechargeable lithium polymer battery \nBluetooth :2.1+4.2(BLE)\nCompatible with Android OS, IOS, Windows \nStandard Accessories: Power Adapter*1, Main Battery*1,USB Cable*1 |
| E14 | 110 |
| F14 | 100 |
| G14 | 90 |
| B15 | Optional Accessories |
| C15 | CH-K419 |
| D15 | Carrying Case / Holster |
| E15 | 12 |
| C16 | PA-K419 |
| D16 | Extra Power Adapter |
| E16 | 10 |
| C17 | BA-K419 |
| D17 | Extra Battery |
| E17 | 18 |
| C18 | UC-K419 |
| D18 | Extra USB Cable |
| E18 | 5 |
| A19 | D81R Series |
| C19 | D812R |
| D19 | Desktop UHF RFID printer |
| E19 | 540 |
| F19 | 510 |
| G19 | 480 |
| A20 | D8100 Plus |
| D20 | D8120plus\nPrint Mode: Thermal Transfer or Direct Thermal\nMaximum Print Width:4.09"/104mm \nMaximum Print length:25,400mm\nMaximum Print Speed:203mm/s\nResolution:203dpi ,8dots/mm  \nCompatible with Android OS, IOS, Windows \nStandard Accessories: Power Adapter*1 |
| E20 | $125                                                                                                              +  Bluetooth      +$25                                                                            +  WiFi      + $45 |
| D21 | D8130plus/D813iplus\nPrint Mode: Thermal Transfer or Direct Thermal\nMaximum Print Width:4.27"/108.4mm \nMaximum Print length:11,430mm\nMaximum Print Speed:152mm/s\nResolution:300dpi ,12dots/mm  \nCompatible with Android OS, IOS, Windows \nStandard Accessories: Power Adapter*1 |
| E21 | $135                                                                                                              +  Bluetooth      +$25                                                                            +  WiFi      + $45 |
| A22 | D9100 |
| D22 | D9120plus\nPrint Mode: Thermal Transfer or Direct Thermal\nMaximum Print Width:4.09"/104mm \nMaximum Print length:2286mm\nMaximum Print Speed:203mm/s\nResolution:203dpi ,8dots/mm  \nCompatible with Android OS, IOS, Windows \nStandard Accessories: Power Adapter*1 |
| E22 | $350                                                                                                           +  Bluetooth      +$35                                                                            +  WiFi      + $45 |
| D23 | D9130plus/D9130iplus\nPrint Mode: Thermal Transfer or Direct Thermal\nMaximum Print Width:4.27"/108.4mm \nMaximum Print length:1016mm\nMaximum Print Speed:152mm/s\nResolution:300dpi ,12dots/mm  \nCompatible with Android OS, IOS, Windows \nStandard Accessories: Power Adapter*1 |
| E23 | $380                                                                                                           +  Bluetooth      +$35                                                                            +  WiFi      + $45 |
| A24 | Warranty |
| D24 | 1 year factory warranty for main device; 6 months for accessories |
| A25 | Lead Time |
| D25 | Sample:2-10 working days;  Bulk order:20-40 working days |
| A26 | Payment Terms |
| D26 | Sample: 100% T/T; Bulk order: T/T 30% in advance upon order,rest 70% before shippment. |
| A27 | Trade Term |
| D27 | EXW SHENZHEN |

Drawing anchors (from cell → media):

| From cell | Media | Drawing name |
| --- | --- | --- |
| A1 | image25.png | Picture 1292 |
| B10 | image68.png | 图片 8 |
| B14 | image69.png | 图片 9 |
| B20 | image70.png | 图片 2 |
| B19 | image71.png | 图片 4 |
| B22 | image72.png | 图片 5 |
| B6 | image73.png | 图片 1 |
| D8 | image74.png | 图片 2 |
| D9 | image75.png | 图片 3 |

### FIXED RFID READER

`nonempty=42 formulas=0 merged=28 images=3`

`merged_ranges=D20:H20;A13:C16;D19:H19;A4:G4;A18:C18;E7:H7;C7:C11;E12:H12;D13:H13;A17:C17;A6:A11;A20:C20;D17:H17;A19:C19;A1:G1;E8:H8;D16:H16;G5:H5;E10:H10;D18:H18;E9:H9;D15:H15;A3:G3;B6:B11;E6:H6;A2:G2;D14:H14;E11:H11`

| Cell | Value |
| --- | --- |
| A1 | UROVO TECHNOLOGY CO., LTD. |
| A2 |  36F, High-Tech Zone Union Tower, No.63,Xuefu Road, Nanshan district, Shenzhen, Guangdong, China |
| A3 |  Fax :  +86-755-23636919       Tel:  +86-755-23636919      Web: en.urovo.com |
| A4 | PRICE LIST |
| A5 | Series |
| B5 | Picture |
| C5 | Model |
| D5 | Configuration |
| E5 | Sample Price |
| F5 | Unit Price(USD)        (MOQ 100pcs) |
| G5 | Unit Price(USD)        (MOQ 500pcs) |
| A6 | FR1000 |
| C6 | FR1000 |
| D6 | AP：IMPINJ E710 Octa-Core 1.6 GHz, \nAndroid 10 OS, \nRAM: 2GB ROM: 16GB, \nWifi: 2.4GHz/5GHz, BT: BT5.0\nUHF: ISO18000-6C,ISO18000-6B, 840～960MHz\nStandard Accessories:  Power Adapter*1, GPS Active Antenna*1 |
| E6 | 350 |
| D7 | 4 dbi antenna |
| E7 | 25 |
| D8 | 6 dbi antenna |
| E8 | 35 |
| D9 | 8 dbi antenna |
| E9 | 30 |
| D10 | 9 dbi antenna |
| E10 | 38 |
| D11 | 10 dbi antenna |
| E11 | 90 |
| A12 | FR2000 |
| C12 | FR2000 |
| D12 | Desktop RFID reader                                                                                                     Based on Impinj E710 design, fully support 18000-6C (EPC \nCLASS1 G2) protocol tags                                                                                        840~960MHz frequency band (frequency customization \noptional)                                                                                                                                        FHSS or Fix Frequency transmission, support RSSI                                                      RF output power up to 30dbm (adjustable)                                                                    Built-in antenna, typical reading effective distance ＜50cm |
| E12 | 300 |
| A13 | Optional Config |
| D13 | HS7:+15USD/pcs |
| D14 |  5500(Mid-to Long distance scanner):+100USD/pcs |
| D15 |  5800(Long distance scanner):+180USD/pcs |
| D16 | 8+128G:+22USD/pcs |
| A17 | Warranty |
| D17 | 1 year factory warranty for main device; 6 months for accessories |
| A18 | Lead Time |
| D18 | Sample:2-10 working days;  Bulk order:20-40 working days |
| A19 | Payment Terms |
| D19 | Sample: 100% T/T; Bulk order: T/T 30% in advance upon order,rest 70% before shippment. |
| A20 | Trade Term |
| D20 | EXW SHENZHEN |

Drawing anchors (from cell → media):

| From cell | Media | Drawing name |
| --- | --- | --- |
| A1 | image25.png | Picture 1292 |
| B12 | image76.png | 图片 4 |
| B6 | image77.png | 图片 4 |

## Embedded pictures (77 unique media)

Coverage: 77/77 `xl/media` files. Reused files are listed once.

| Media | Visible evidence |
| --- | --- |
| image1.png | Collage of black DT50-family accessories (cradles, holster, trigger, chargers) on white. |
| image2.png | Tall smartphone front, Android home with Google search, time 08:01, Play Store; used at DT50P row. |
| image3.png | Black/orange UHF RFID pistol grip / gun accessory (RFDT50 class) on black background. |
| image4.png | Black pistol-grip trigger handle, orange accents, light background. |
| image5.png | Black UROVO single-slot charging cradle, gold pogo pins. |
| image6.png | Black 4-bay battery charging dock. |
| image7.png | Pistol-grip scan trigger, grey/orange, three-quarter view. |
| image8.png | Black 5-slot device charging cradle. |
| image9.png | Curved screen-protector film, two pieces. |
| image10.png | Black nylon holster / belt pouch, empty. |
| image11.png | CT58C-class PDA, front 08:11 Android launcher and rear camera/scanner housing, UROVO. |
| image12.png | Similar PDA pair (front 08:11 / rear), slightly different rear texture — DT50S-class. |
| image13.png | Tiny 71×94 px icon-like crop; product identity not readable. Marked unreadable beyond a dark rectangular silhouette. |
| image14.png | Large studio render of a handheld (used on DT66 trigger and reused). High-res RGBA product photo. |
| image15.png | Black fabric carrying pouch with hook-and-loop flap (photo on a table). |
| image16.png | Small grey single-slot cradle, side view. |
| image17.png | Black 4-slot battery charger, top view. |
| image18.png | Black 5-slot device cradle. |
| image19.png | Black 5-slot cradle variant (ethernet-class layout in the sheet mapping). |
| image20.png | Very large photo of a phone-shaped PDA (DT66 row mapping). Front home screen not fully transcribed at contact-sheet scale; device is a 6.5-inch-class smartphone form. |
| image21.png | Pistol-grip trigger, black/orange, side studio shot. |
| image22.png | DT610-class tall phone, front 08:11. |
| image23.png | DT630-class phone, lock screen 05:18 Saturday June 18 2024 and a second 08:18 lock-screen crop in the same asset. |
| image24.png | Rugged phone pair: left lock 15:05 teal wallpaper; right colorful wallpaper, orange side keys — DT630/DT610 family. |
| image25.png | UROVO wordmark lockup **UROVO mobility redefined** (header logo reused on several sheets at A1). |
| image26.png | Grey tablet hand-strap / holder. |
| image27.png | Tablet in a case, dark screen, on a table. |
| image28.png | Tablet rear with hand-strap, rugged housing. |
| image29.png | Black charging cradle for a tablet (P8100P-class). |
| image30.png | 10-inch-class tablet front, lock screen **10:32 PM**, used for both P8100P 4G and 5G rows (same media). |
| image31.png | Tablet rear / docking interface on black. |
| image32.png | Small 146×53 px crop; UROVO wordmark fragment / thin graphic. Little independent product fact. |
| image33.png | Blue/grey nylon shoulder strap. |
| image34.png | Grey carrying pouch with shoulder strap attached. |
| image35.png | Black fabric hand strap on light background. |
| image36.png | CT48C-class compact PDA, front lock screen. |
| image37.png | Rugged PDA rear/side on black, yellow scanner window. |
| image38.png | Gun-style handheld front, numeric keypad, large display (RT40S 29-key class). |
| image39.png | Black hand strap. |
| image40.png | Black UROVO single-slot cradle. |
| image41.png | Dual-bay UROVO charging dock. |
| image42.png | Multi-slot cradle with a gun-style device seated. |
| image43.png | Multi-slot cradle, empty bays, gun-style outline. |
| image44.png | Black rubber/TPU boot case, cutouts. |
| image45.png | RT40S 38/51-key class handheld, front Android 7:35, numeric/function keypad, orange scan key. |
| image46.png | Black UROVO pistol-grip / handle cradle or holster cup. |
| image47.png | i9100-class handheld POS, front 08:11, numeric keypad. |
| image48.png | POS accessory cluster: printer-up housing, side skins, rear. |
| image49.png | White handheld POS with printer on top, blank screen (i9200-class). |
| image50.png | White handheld POS printer-up, Android 08:11, 商家 on printer bezel (sample UI). |
| image51.png | Black handheld 1D/2D scanner gun (R70-class). |
| image52.jpeg | Wearable wrist computer, grey strap, UROVO on the mount (U2S-class). |
| image53.png | Four-bay battery charger loaded with batteries. |
| image54.png | Six-bay charger loaded with batteries. |
| image55.png | Rugged square wearable / wrist PDA, lock **20:06**, Android icons (SR5750-class). |
| image56.png | Small low-contrast graphic (176×143, greyscale); identity not clearly readable — treated as a small accessory icon. |
| image57.png | Black watch/wrist band. |
| image58.png | Black neck/shoulder lanyard on a table. |
| image59.png | Black dual-slot charger. |
| image60.png | Black 4-slot charger bar. |
| image61.png | Bluetooth ring scanner on a finger, yellow/black imager head (SR5600 Pro-class). |
| image62.png | Ring scanner in a charging cup, extra rings beside it. |
| image63.png | 20-bay host charging dock, grid of cups, plus a 5-bay bar below. |
| image64.png | 30-bay host charging dock grid. |
| image65.png | Ring scanner, yellow/black, three-quarter studio shot. |
| image66.png | Black lanyard with a small scanner-shaped fob. |
| image67.png | Handheld wireless scanner, yellow imager, UROVO (S716-class). |
| image68.png | K388 Pro-class mobile printer, grey/orange buttons, UROVO on the flip cover. |
| image69.png | K329-class mobile printer, grey body, orange latch, paper in the path. |
| image70.png | K419-class / 4-inch mobile printer, brown/grey, green button. |
| image71.png | Desktop printer close-up, UROVO, green button (D81R/D8100 family). |
| image72.png | UROVO desktop barcode/RFID printer, blue-grey, media window. |
| image73.png | Rugged handheld with yellow side rails (possible D81R portable or mis-mapped product shot). |
| image74.png | Tiny 53×83 px blurry cable-like object; unreadable beyond a dark connector silhouette. |
| image75.png | Black adapter plus a 4-bay charger with red/green status rings on posts (printer battery charger). |
| image76.png | Grey desktop RFID pad / antenna plate with cable. |
| image77.png | Black finned fixed RFID reader, multiple SMA antenna ports on the top edge (FR1000-class). |


## Routing notes (do not invent Hubs)

Canonical Product Hubs covered by named model/series rows: DT66, CT58C, DT50 Pro, DT50S (series cell `DT50` / model `DT50S`), DT50P, DT610, DT630, UPad (`UPAD`), U100, P8100P 4G, P8100P 5G, CT48C, RT40S (series `RT40S` / model `SQ47S`), i9100, i9200 (including `i9200 EMV` as a variant row), i9600 (including `i9600 mini`), i5300, i5300L, U2S (model `SQ46S`), R7 (model `R70`), SR5750, K388 Pro, K329, K419, D81R Series (model `D812R`), D8100 Plus (`D8120plus` / `D8130plus`/`D813iplus` rows), FR1000, FR2000.

Additional labels **without** a dedicated Hub in this package: **SR5600 Pro**, **S716**, **D9100** (`D9120plus` / `D9130plus`/`D9130iplus`), **RFDT50** (DT50P optional accessory `TRG-DT50-06`). Sheet title `RT40,CT48C` is a sheet name; the body series is RT40S. Sheet title `P8100, P8100P，UPAD，U100` has P8100P 4G/5G rows but **no P8100 4G** model row.

Optional config adders in this edition: sheet `DT66,DT50, CT58` has `HS7:+15USD/pcs` and `8+128G:+22USD/pcs`; sheet `P8100, P8100P，UPAD，U100` has only `8+128G:+22USD/pcs`; sheet `DT610，DT630` has none. Sheets `RT40,CT48C` and `FIXED RFID READER` still print `HS7:+15USD/pcs`; `5500(Mid-to Long distance scanner):+100USD/pcs`; `5800(Long distance scanner):+180USD/pcs`; `8+128G:+22USD/pcs`.
