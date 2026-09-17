# ESL — Electronic Shelf Labels

> **Source Hub**: [[products/ESL|ESL Source Hub]]

> Sources: size-specific specs under `ESL/others/` and F24A7 base-station spec. Presentation is not used as the sole authority for hard specs.

Category: [[categories/esl|Electronic Shelf Labels]]

Size-specific documents disagree with the English overview on battery life, IP, range, viewing angle, and NFC. See the Hub discrepancy table. Values below are labeled by source.

## Overview

UROVO electronic shelf labels are 2.4 GHz active e-paper tags updated from a base station or a phone app. The synchronized English overview lists four sizes: **1.54-inch**, **2.13-inch**, **2.66-inch**, and **4.2-inch**. Synchronized tag specs exist for 2.13-inch (ET0213), 2.66-inch (T2664), and 4.2-inch (ET0420). The matching base station is named **F24A7**.

## Tag models (from size specs)

| Source | Model(s) | Screen | Resolution | Body size | Weight | Battery | Colors |
| --- | --- | --- | --- | --- | --- | --- | --- |
| 2.1-inch spec v3.0 | ET0213-81 (table); temperature row also names ET0213-33/B, ET0213-39/B | 2.13 inch | 250×122 | 71.28×34.78×12.3 mm | 32 g | CR2450 × 2, 不低于7年 | 4/3/2 color options |
| T2664 spec | T2664 | 2.66 inch | 184×360 | 83×42×12 mm | — | 内置电池×2 | 四色 refresh |
| 4.2-inch spec v3.0 | ET0420-84 (4-color); ET0420-42 (B/W 快刷) | 4.2 inch | 400×300 | 99.16×89.16×12.3 mm | 82 g | CR2450 × 3, 不低于7年 | 4-color / 3-color (B/W on ET0420-42) |

## 2.13-inch (ET0213) hard specs

| Parameter | Value (2.1-inch spec) |
| --- | --- |
| Wireless | Bluetooth 5.0 private protocol; 2.400–2.480 GHz; max EIRP ≤ 10 mW |
| Range | 30 m (50 m open) |
| IP | IP65 default, IP68 optional |
| LED | RGB, 7 colors; blink 1/s, count user-set |
| Update rate | >30000/hour (500/min) |
| NFC | Optional |
| Pages | 8 |
| Certifications | CE, RoHS, FCC, MIC, SRRC |
| Pack | 450/box, 15.4 kg, 390×300×260 mm |
| Operating temp | 0–40℃ ET0213-81 and ET0213-33/B; -25–25℃ ET0213-39/B |

## 2.66-inch (T2664) hard specs

| Parameter | Value (T2664 spec) |
| --- | --- |
| RF | 2.40–2.48 GHz; sensitivity better than -95 dBm; 1 Mbit/s; ≤20 ppm; GFSK |
| Protocol | Private |
| Read distance | 100 m (base-station antenna and power) |
| Activation | 16 s |
| Currents | Sleep 3 µA; RX 10 mA; TX 20 mA |
| Environment | Operating -20–60℃; storage -30–70℃; humidity 5–95% non-condensing |

The English overview “core performance” slide repeats this 2.66-inch mechanical/RF set and adds **IP68**, **600 mA**, and **15-year** life at twice-daily refresh. Those extras are not in the T2664 spec sheet.

## 4.2-inch (ET0420) hard specs

| Parameter | Value (4.2-inch spec) |
| --- | --- |
| Wireless | Bluetooth 5.0 private protocol; 2.400–2.480 GHz; max EIRP ≤ 10 mW |
| Range | 30 m (50 m open) |
| IP | IP65 default, IP68 optional |
| LED | RGB, 7 colors |
| Update rate | >30000/hour (500/min) |
| NFC | Optional |
| Pages | 8 |
| Operating temp | 0–40℃ (3-color, 4-color); 0–50℃ (B/W) |
| Pack | 180/box, 15.76 kg, 390×350×240 mm |
| APP | 价签管理1.0.1 (ET0420-84); NFCDemo1.0.1 (ET0420-42) |

## F24A7 base station

| Parameter | Value (F24A7 PDF) |
| --- | --- |
| CPU | Rockchip RK3128, quad-core, 1.3 GHz |
| Memory / storage | 1G RAM; eMMC 8G |
| OS | Android |
| Network | 1× 10/100 Ethernet (p.5). Advantages (p.4) also list WIFI. |
| RF | 2.4 GHz; -95 dBm; 1 Mbit/s; vertical polarization; omni/directional by antenna |
| ESL radio | Self-developed 2.4 GHz active-ESL protocol; half-duplex; 100 m (antenna/tag power) |
| Power | POE 802.3af 44–57 V / DC12V; standby <500 mA; operating ≤2 A (DC12V) |
| Size (table) | 150×95.5×23.8 mm (slight error allowed) |
| Size (drawing) | 150.20×95.20×23.50 mm; hole spacing 142.70×86.70 mm; hole Ø 3.30 mm |
| Environment | Operating -20–+65℃; storage -20–+85℃; humidity 5–95% RH non-condensing |
| Software | SDK and API; remote network upgrade; scheduled power on/off; RTC |

## Related Products

- [[pb/ESL|ESL Brochure / Product Page]]
- [[categories/esl|Electronic Shelf Labels]]
