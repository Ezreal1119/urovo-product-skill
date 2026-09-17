# Zebra SE58 Extended Range Scan Engine

> 原文：`Zebra-SE58(00)-Specs.pdf`（Zebra Technologies）。本伴侣为忠实转写，供检索用；原始 PDF 保留在同一目录。

## Overview

SE58 Extended Range Scan Engine 搭载 Zebra **IntelliFocus™** 技术，可在 **<2 in./5 cm 到 >105 ft./32 m** 范围内无缝识读条码（行业最宽工作范围）。绿色激光瞄准器（带宽十字图案）比红色瞄准高 7 倍可见度，可室内外全解码范围及强日光（约 10 ft./3 m）下轻松瞄准。**10.6 g 重量 + 10.6 mm 高度**，比竞品轻 50%+、小 18%¹。

- **1 MP 近距固定对焦** + **2 MP 远距变焦**双传感器，全程无缝条码捕获。
- **PRZM Intelligent Imaging** + Zebra 自研算法，在污损、低对比、覆膜、反射面/LCD 屏等条件下首次即可解码。
- **SDL 软件解码**：直接用主机 CPU，无需硬件解码器，省空间/功耗/成本；支持 Qualcomm/MediaTek/NXP + Android/Linux；使用 Android Camera Native API 兼容未来 Android 版本。
- **行业最低失效率**：Zebra 数据采集产品失效率 <0.5%，15 个月保修。

## Key Features

- **IntelliFocus™** 智能判断距离并捕获条码。
- **绿色激光瞄准器**：宽十字图案，比红色瞄准高 7 倍可见度。
- **超宽工作范围**：105 ft./32 m（100 mil Code 39）+ 24 ft./7.3 m（55 mil QR）。
- **轻巧紧凑**：10.6 g / 10.6 mm 高，可集成至口袋型手持到超坚固工业设备。
- **SDL 软件解码**：省硬件、功耗、空间。

## Markets and Applications

- Warehousing（仓储）
- Transportation and Logistics（运输与物流）
- Retail（零售）

## Technical Specifications

### Physical Characteristics

| Parameter | Value |
| --- | --- |
| Dimensions | 0.42 in. H × 1.19 in. W × 0.87 in. D; 10.6 mm H × 30.1 mm W × 22.1 mm D |
| Weight | 0.37 ± 0.02 oz./10.6 ± 0.5 g |
| Interface | 24-pin 0.4 mm pitch board-to-board connector, MIPI (2 data lanes) |

### Performance Characteristics

| Parameter | Value |
| --- | --- |
| Shutter Type | Global |
| Sensor Resolution | Far: 1920 horizontal × 1080 vertical pixels; Near: 1280 horizontal × 800 vertical pixels |
| Field of View | Far: Horizontal: 14.0°, Vertical: 7.9°; Near: Horizontal: 42.1°, Vertical: 27° |
| Skew Tolerance | ±60° |
| Pitch Tolerance | ±60° |
| Specular Dead Zone | ±18° |
| Roll Tolerance | 360° |
| Focal Distance | Near camera: 8 in./20.3 cm fixed focus; Far camera: from 8 in./20.3 cm to infinity |
| Aiming | Green Laser 520 nm |
| Illumination | 2 warm-white LEDs 2700K |
| Min. Print Contrast Minimum | 25% |

### Regulatory

| Parameter | Value |
| --- | --- |
| Laser/LED Classification | Class 2 laser per IEC/EN 60825-1; Class II laser per FDA CDRH; Risk Group 1 LEDS per IEC/EN 62471 |
| Electrical Safety | Complies with IEC/EN 62368-1 and UL 62368-1 and CAN/CSA C22.2 No. 62368-1-14 |
| Environmental | RoHS compliant |

### User Environment

| Parameter | Value |
| --- | --- |
| Ambient Light | Max 107,639 lux (direct sunlight) |
| Operating Temperature | -4° F to 140° F / -20° C to 60° C |
| Storage Temperature | -40° F to 158° F / -40° C to 70° C |
| Humidity | 5% to 95% (non-condensing), not intended for exposed operation |
| Shock Rating | 2500 ± 100 g, any mounting surface, at 20° C for 0.70 ± 0.10 ms; 2000 ± 100 g, any mounting surface, at -20° C and 60° C for 0.85 ± 0.1 ms |

### Power

- **Operational Input Voltage:**
  - VCC = 3.3 +0.3 / -0.165 V
  - VDD_IO_HOST: 1.71 to 3.6 V
  - VCC_ILLUM: 3.0 to 5.5 V
- **Current Draw:**
  - Total VCC=VDD_IO_HOST=3.3 V, VCC_ILLUM=5 V: 340 mA RMS, 750 mA Peak
  - Total VCC=VDD_IO_HOST=VCC_ILLUM=3.3 V: 475 mA RMS, 1000 mA Peak
  - VCC_ILLUM=5 V: 360 mA RMS, 900 mA Peak
  - VCC=VDD_IO_HOST=3.3 V: 215 mA RMS, 670 mA Peak
- **Current Draw in Low-Power Modes:**
  - Idle = 75 mA RMS
  - Low Power = 3 mA RMS

### Footnotes

1. Measured in total volume
2. Distance dependent on symbology type and size; range is reduced under lower ambient light level.
3. Dependent on the width of the barcode (shorter barcodes can be read even closer, and wider barcodes farther)

### Decode Ranges (Typical Working Ranges)²

| Symbology/Resolution | Near Distance | Far Distance |
| --- | --- | --- |
| 5 mil Code 39 | 2.1 in./5.3 cm | 4.8 ft./1.45 m |
| 10 mil Code 39 | *³ | 9.6 ft./2.92 m |
| 100% UPC A | 2.2 in./5.6 cm | 12.2 ft./3.71 m |
| 15 mil Code 128 | *³ | 13.7 ft./4.17 m |
| 20 mil Code 39 | *³ | 19.7 ft./5.99 m |
| 40 mil Code 39 | *³ | 41.2 ft./12.55 m |
| 55 mil Code 39 RFL | *³ | 61.2 ft./18.64 m |
| 100 mil Code 39 (paper) | *³ | 107.1 ft./32.64 m |
| 100 mil Code 39 RFL | *³ | 105.2 ft./32.05 m |
| 100 mil Code 128 RFL | *³ | 87.1 ft./26.54 m |
| 10 mil DataMatrix | 2.4 in./6.1 cm | 5.2 ft./1.58 m |
| 10 mil QR | 2.4 in./6.1 cm | 4.6 ft./1.39 m |
| 55 mil QR | *³ | 24 ft./7.32 m |

## Warranty

受 Zebra 硬件保修声明约束，SE58 自发货之日起 **15 个月** 内对工艺与材料缺陷提供保修。完整声明见 www.zebra.com/warranty。
