# Zebra SE55 Advanced Range Scan Engine

> 原文：`Zebra-SE55(00)-Specs.pdf`（Zebra Technologies）。本伴侣为忠实转写，供检索用；原始 PDF 保留在同一目录。

## Overview

SE55 Advanced Range Scan Engine 搭载 Zebra **IntelliFocus™** 技术（智能自动对焦），可在手边到 **40 ft / 12.2 m** 远范围内可靠识读条码。绿色激光瞄准器在强日光下比红色瞄准高 7 倍可见度；PRZM Intelligent Imaging 提供「first-time, every-time」解码。高度 <7.5 mm，可装入大多数口袋型设备，适合零售与仓储。

## Key Features

- **IntelliFocus™** 智能自动对焦：手边到远距自适应识读。
- **PRZM Intelligent Imaging**：对污损/低对比/覆膜/低对比条码也能稳定解码。
- **绿色激光瞄准器**：宽瞄准图案，比红色瞄准高 7 倍可见度。
- **4MP 高分辨率传感器**：同时支持条码解码和高分辨率图像/文档采集，可省掉第二个摄像头。
- **超宽工作范围**：2.2 in./5.6 cm 到 40 ft/12.2 m+。
- **坚固耐用**：高抗冲击等级 + 宽工作温度。
- **灵活解码策略**：
  - 硬件解码：**PL5000A MIPI** 微小解码板 / **PL5000C Ball Grid Array**（焊接到主机板）。
  - 软件解码：**SDL**（无硬件，省空间、功耗、电池循环时间）。

## Markets and Applications

- 零售前店（micro-fulfillment center / BOPIS）。
- 后仓与仓储：从料箱分拣到室外收货托盘上架（叉车作业）。
- 工业/零售多功能应用。

## Technical Specifications

### Physical Characteristics

| Parameter | Value |
| --- | --- |
| Dimensions | 7.2 mm H × 26.4 mm W × 14.9 mm D |
| Weight | 5.4 g +/- 0.10 g |
| Interface | Camera Port on 24-pin board-to-board connector. Supports MIPI interface |

### Performance Characteristics

| Parameter | Value |
| --- | --- |
| Sensor Resolution | 2688 × 1520 |
| Adaptive Field of View | Maximum Horizontal: 37°, Maximum Vertical: 21°² |
| Skew, Pitch, Roll | Skew Tolerance: ±60°; Pitch Tolerance: ±60°; Roll Tolerance: 360° |
| Focal Distance | From front of engine: 3 in. to infinity |
| Aiming | Green Laser 520 nm |
| Illumination | 2 Warm-White LED |

### Regulatory

| Parameter | Value |
| --- | --- |
| Classification | Intended for use in CDRH Class II laser/IEC 60825-1 Class 2 laser devices |
| Electrical Safety | Complies with IEC/EN 62368-1:2014 and UL 62368-1 Second Edition, 2014-12-01 and CAN/CSA C22.2 No. 62368-1-14, Second Edition, 2014-12-01 |
| Environmental | RoHS Compliant |

### User Environment

| Parameter | Value |
| --- | --- |
| Ambient Light | Max 107,639 lux (direct sunlight) |
| Operating Temp. | -30° C to 60° C |
| Storage Temp. | -30° C to 70° C |
| Humidity | Operating: 95% RH, non-condensing at 122° F/50° C; Storage: 85% RH, non-condensing at 158° F/70° C |
| Shock Rating | 2500 ± 100 g, ½ sine, 0.70 ± 0.1 msec shock at 20° C; 2000 ± 100 g, ½ sine, 0.85 ± 0.1 msec shock at -30° C and at 60° C |

### Power

- **Operational input Voltages:**
  - VCC_ENGINE: 3.135 V to 3.6 V
  - VDD_IO_HOST: 1.71 V to 3.6 V
  - VCC_ILLUM: 2.9 V to 5.5 V
- **Operating Current (Typical):**
  - VCC_ENGINE + VDD_IO_HOST (3.3 V): 130 mA
  - VCC_ILLUM (3.3 V) Up to 480 mA; (5 V) up to 400 mA
- **Current Draw in Low-Power Modes (Idle / Low Power):** 65 mA / <3 mA Typical

### Footnotes

1. Printing resolution, contrast and ambient light dependent.
2. Field of view limited.

### Decode Ranges (Typical)¹

| Barcode Type | Near Distance | Far Distance |
| --- | --- | --- |
| 3 mil Code 39 | 2.7 in./6.9 cm | 16.2 in./41.1 cm |
| 5 mil Code 39 | 2.5 in./6.4 cm | 26.6 in./67.6 cm |
| 5 mil PDF417 | 2.8 in./7.1 cm | 19.6 in./49.8 cm |
| 6.7 mil PDF417 | 2.6 in./6.6 cm | 25.6 in./65.0 cm |
| 10 mil DataMatrix | 2.2 in./5.6 cm | 27.1 in./68.8 cm |
| 100% UPC (13 mil) | 2.5 in./6.4 cm | 71 in./180 cm |
| 15 mil Code 128 | 7.2 in./18.2 cm² | 72 in./182.9 cm |
| 20 mil Code 39 | —² | 109 in./276.9 cm |
| 55 mil Code 39 | —² | 293 in./744.2 cm |
| 100 mil Code 39 | —² | 554 in./1407.2 cm |
| 100 mil DataMatrix | —² | 270 in./685.8 cm |

## Warranty

受 Zebra 硬件保修声明约束，SE55 自发货之日起 **15 个月** 内对工艺与材料缺陷提供保修。完整声明见 www.zebra.com/warranty。
