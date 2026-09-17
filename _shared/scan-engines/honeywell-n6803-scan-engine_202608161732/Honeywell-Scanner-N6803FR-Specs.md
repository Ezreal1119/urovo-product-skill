# Honeywell FlexRange™ N6803 Series — Compact Undecoded 2D Scan Engines (MR / FR / LR)

> 原文：`Honeywell-Scanner-N6803FR-Specs.pdf`（Honeywell）。本伴侣为忠实转写，供检索用；原始 PDF 保留在同一目录。

## Overview

Honeywell FlexRange™ N6803 系列是超薄（ultra-slim）未解码 2D 扫描引擎系列，三个型号共享同一外形尺寸（6.8 mm H × 23.5 mm W × 16.2 mm D），读距逐级提升：

| 型号 | 读距 | 光学架构 |
| --- | --- | --- |
| **N6803MR** | 至 6 m [20 ft] | Smart Adaptus™ 8.0 单镜头 solid-state，可读失焦图像 |
| **N6803FR** | 至 10 m [30 ft] | 双镜头架构，近/远快速切换 |
| **N6803LR** | 至 25 m [80 ft] | 极远距，仓库/配送中心货架顶端、叉车作业 |

- 同一超薄外形适配单一移动设备，覆盖近/中/远多场景，减少设备种类。
- OS 设备可配最新 host decoder 软件；非 OS 设备可配 **Gen8 DB Decoder Board**。

## Potential Applications

专业级移动设备：手持终端、平板、可穿戴扫描器、零售/仓库配件，以及配送、取件/派件、现场服务。

## Features and Benefits

- 超薄小尺寸长距离扫描引擎，单一设备覆盖多工作流。
- Smart Adaptus 8.0 单镜头扩展读距 + 双镜头设计同步近/远图像采集；多工作流（近/中/远）一台设备搞定。
- 极轻 3g，耐 3500G 冲击。
- 较同档长距引擎功耗更低，单次充电续航更长。
- host decoder 软件 或 Gen8 DB 板灵活选择。
- 锐利激光点瞄准，几米/英尺外也能定位条码。

## Technical Specifications

### Table 1 — Mechanical

| Characteristic | Parameter |
| --- | --- |
| Dimensions (H × W × D) | 6.8 mm × 23.5 mm × 16.2 mm [0.27 in × 0.93 in × 0.64 in] |
| Weight | 3 g [0.11 oz] |
| Interface | MIPI |

### Table 2 — Electrical

| Characteristic | N6803MR | N6803FR | N6803LR |
| --- | --- | --- | --- |
| Input voltage | 1.71 V to 3.45 V | 3.3 Vdc ±5% | 3.3 Vdc ±5% |
| Current | 303 mA (typical) | 270 mA (typical) | 230 mA (typical) |

### Table 3 — Performance

| Characteristic | N6803MR | N6803FR | N6803LR |
| --- | --- | --- | --- |
| Sensor technology | Global shutter | Global shutter | near: Global shutter; far: Rolling shutter |
| Resolution | 1920 × 800 pixel | near: 1920 × 800 pixel; far: 1280 × 800 pixel | near: 1920 × 800 pixel; far: 1920 × 800 pixel |
| Scan rate | 60 fps default | 40 fps default (60 fps max) | 30 fps default |
| Illumination | white (LED) | white (LED) | white (LED) |
| Aimer | 650 nm laser dot | 520 nm laser dot (green aimer) | 650 nm red laser dot |
| Field of view | 37° × 16° | near: 48° × 21°; far: 20° × 12° | near: 48° × 21°; far: 13.7° × 7.6° |
| Symbol contrast | 20% | 20% | 20% |
| Minimum resolution | 3 mil 1D | 5 mil 1D | 3 mil 1D |

### Table 4 — Environmental

| Characteristic | N6803MR | N6803FR | N6803LR |
| --- | --- | --- | --- |
| Operating temperature¹ | -30°C to 60°C [-22°F to 140°F] | -30°C to 60°C [-22°F to 140°F] | -25°C to 50°C [-13°F to 122°F] |
| Storage temperature | -40°C to 70°C [-40°F to 158°F] | -40°C to 70°C [-40°F to 158°F] | -30°C to 70°C [-22°F to 158°F] |
| Humidity (non-condensing) | Up to 95% at 60°C [140°F] | Up to 95% at 50°C [122°F] | Up to 95% at 50°C [122°F] |
| Shock | 3500 G for 0.4 ms at 23°C [73°F] | 3500 G for 0.4 ms at 23°C [73°F] | 3500 G for 0.4 ms at 23°C [73°F] |
| Vibration | 3 axes, 1 hour per axis: 2.54 cm [1 in] peak-to-peak displacement (5 Hz to 13 Hz); 10 G acceleration (13 Hz to 500 Hz), 1 G acceleration (500 Hz to 2,000 Hz) | (same as MR) | (same as MR) |
| Ambient light² | 0 lux to 100,000 lux | 0 lux to 100,000 lux | 0 lux to 100,000 lux |
| Mean time between failure³ | 320,000 hours | 395,000 hours | 307,000 hours |

### Warranty

15-month limited warranty，自 Honeywell 发货之日起算。

### Table 5 — Read Ranges⁴ (mm [in])

| Symbology | MR Near | MR Far | MR Delta | FR Near | FR Far | FR Delta | LR Near | LR Far | LR Delta |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| 13 MIL UPC | 65 [2.6] | 965 [38.0] | 900 [35.4] | 68 [2.7] | 1690 [66.5] | 1622 [63.9] | 67 [2.63] | 1923 [75.7] | 1856 [73.08] |
| 5 MIL C39 | 85 [3.3] | 350 [13.8] | 265 [10.4] | 137 [5.4] | 396 [15.6] | 259 [10.2] | 146 [5.74] | 437 [17.2] | 291 [11.46] |
| 10 MIL DM | — | — | — | — | — | — | 148 [5.82] | 448 [17.63] | 300 [11.82] |
| 10 MIL C128 | 65 [2.6] | 760 [30.0] | 695 [27.3] | 90 [3.5] | 1399 [55.1] | 1309 [51.5] | 95 [3.74] | 1928 [75.9] | 1833 [72.17] |
| 20 MIL C39 | 85 [3.3] | 1500 [59.0] | 1415 [55.7] | 66 [2.6] | 2848 [104.1] | 2760 [108.7] | 77 [3.03] | 6066 [238.81] | 5989 [235.79] |
| 55 MIL C39 | — | 3200 [126.0] | — | — | 7060 [278.0] | — | — | 15040 [592.12] | — |
| 100 MIL C39 | — | 5500 [216.5] | — | — | 11370 [447.6] | — | — | 26782 [1054.4] | — |
| 100 MIL DM | — | — | — | — | 6221 [244.9] | — | — | 13634 [536.77] | — |
| 10 MIL QR | 70 [2.8] | 320 [12.6] | 250 [9.8] | 128 [5.0] | 412 [16.2] | 284 [11.2] | — | — | — |

### Table 6 — Symbologies

- **Linear:** Codabar, Code 11, Code 128, Code 2 of 5, Code 39, Code 93 and 93i, EAN/JAN-13, EAN/JAN 8, IATA Code 2 of 5, Interleaved 2 of 5, Matrix 2 of 5, MSI, GS1 Databar, UPC-A, UPC E, UPC-A/EAN-13 with Extended Coupon Code, Coupon GS1, Coupon Code 32 (PARAF), EAN-UCC Emulation
- **2D Stacked:** Codablock A, Codablock F, PDF417, MicroPDF417
- **2D Matrix:** Aztec Code, Data Matrix, MaxiCode, QR Code, Chinese Sensible (Han Xin), Grid Matrix, Dot Code
- **Postal:** Australia Post, British Post, Canadian Post, China Post, Japanese Post, Korea Post, Netherlands Post, Planet Code, Postnet

### Footnotes

1. Extreme temperatures will reduce the depth of field.
2. Extreme ambient light conditions will reduce the depth of field.
3. Based on MIL-HDBK-217F (released December 1, 1991). The calculation is based on the part count method for the Ground Benign (GB) environmental conditions.
4. Barcode quality and environmental conditions may affect performance.

## Laser Safety (Figure 1. Laser Dot Aimers)

- N6803FR (green aimer): MAX. 1 mW: 515–530 nm
- N6803FR (red aimer): MAX. 1 mW: 645–660 nm
- IEC 60825-1:2014. Pulse duration of 10 mSec. Complies with 21CFR 1040.10 and 1040.11 except for conformance with IEC 60825-1 Ed.3., as described in Laser Notice No. 56, dated May 8, 2019.
- CLASS 2 LASER PRODUCT / APPAREIL A LASER DE CLASSE 2.

## Warranty / Remedy

Honeywell 保修其产品在适用保修期内无材料与工艺缺陷。标准产品保修适用，除非 Honeywell 书面另行约定。退回保修期内产品，Honeywell 可选择免费维修或更换。规格如有更改，恕不另行通知。
