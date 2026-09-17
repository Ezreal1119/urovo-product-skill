# Honeywell N570X Series — Compact Undecoded 2D Scan Engines

> 原文：`Honeywell-Scanner-HS7-Specs.pdf`（Honeywell）。本伴侣为忠实转写，供检索用；原始 PDF 保留在同一目录。

## Overview

N570X 系列是 Honeywell 最新 Compact Series 未解码 2D 条码扫描引擎，提供 **SR（Standard Range）与 HD（High Density）** 两种光学型号，针对紧凑尺寸、高运动容差、低功耗、易集成优化，用于下一代紧凑移动设备。

- **N5703SR**：1 Mpx global shutter 传感器，可读 Code 39 至 0.86 m（33.86 in），白色 LED 照明 + Honeywell 标志性激光十字准星/角框瞄准，适合物流（直射阳光+室内）。
- **N5701HD**：近距离识读，暖白 LED + 亮绿色 LED 点瞄准，可读小至 **1D 2 mil / 2D 4 mil**，适合零售、医疗、点码与手机屏幕条码。
- MIPI 接口便于软件 host decode 集成；非 OS 场景可配 **Gen7M DB**。
- 紧凑尺寸 8.1 mm × 21.6 mm × 10.4 mm。
- 电气向后兼容 Honeywell **N670X / N660X / N4603 / N360X** 系列（同连接器）。

## Potential Applications

专业级移动设备：平板、可穿戴扫描器、移动终端、零售/医疗配件，以及配送、取件/派件、现场服务。

## Features and Benefits

- 紧凑尺寸适配最受限的移动设备设计。
- global shutter 运动容差 6 m/s（对比 rolling shutter 0.1 m/s），提升「跟手」体验。
- 宽工作温度 -30°C 到 60°C [-22°F 到 140°F]。
- 可选 Honeywell 功能如 OCR、EasyParse™（驾照、登机牌）。
- 与其他 Honeywell 扫描引擎系列兼容，减少集成时间与设计成本。

## Technical Specifications

### Table 1 — Mechanical

| Characteristic | Parameter |
| --- | --- |
| Dimensions (H × W × D) | 8.1 mm × 21.6 mm × 10.4 mm [0.32 in × 0.85 in × 0.41 in] |
| Weight | 2.1 g [0.07 oz] N5703SR；1.9 g [0.067 oz] N5701HD |
| Interface | MIPI |

### Table 2 — Electrical

| Characteristic | Parameter |
| --- | --- |
| Input voltage | 3.3 Vdc ±5 % |
| Current | N5701HD: 165 mA (Max)；N5703SR: 180 mA (Max) |

### Table 3 — Performance

| Characteristic | Parameter |
| --- | --- |
| Sensor technology | Global shutter |
| Resolution | 1280 × 800 |
| Illumination | White LED (N5703SR)；Warm White LED (N5701HD)；exempt risk group |
| Aimer | N5703SR: 650 nm 高可见红色激光（advanced red laser, cross target and framers）；N5701HD: Green LED dot aimer |
| Scan rate | 60 fps max. |
| Motion tolerance | 6 m/s [19.7 ft/s] |
| Field of view | horizontal: 44°, vertical: 28.5° |
| Scan angles | tilt: 360°, pitch: ±55°, skew: ±70° |
| Symbol contrast | 20% minimum print contrast ratio |
| Mean time between failure (MTBF)* | 327,786 hours (N5703SR)；725,680 hours (N5701HD) |

### Table 6 — N5703SR Read Ranges**

| Symbology | Near Distance (mm/in) | Far Distance (mm/in) | Delta (mm/in) |
| --- | --- | --- | --- |
| 13 mil UPC-A | 44/1.7 | 573/22.6 | 529/20.8 |
| 5 mil C39 | 70/2.8 | 311/2.2 | 241/9.4 |
| 10 mil C39 | 40/1.6 | 536/21.1 | 496/19.5 |
| 20 mil C39 | 68/2.7 | 868/34.2 | 800/31.5 |
| 5 mil C128 | 75/3.0 | 272/10.7 | 197/7.7 |
| 10 mil DM | 64/2.5 | 297/11.7 | 233/9.2 |
| 20 mil QR | 57/2.2 | 513/20.2 | 456/18.0 |
| 10 mil PDF | 45/1.8 | 425/16.7 | 380/15 |

### Table 7 — N5701HD Read Ranges**

| Symbology | Near Distance (mm/in) | Far Distance (mm/in) | Delta (mm/in) |
| --- | --- | --- | --- |
| 13 mil UPC-A | 44/1.73 | 480/18.90 | 436/17.17 |
| 3 mil C39 | 76/2.99 | 170/6.69 | 94/3.7 |
| 5 mil C39 | 50/1.97 | 285/11.22 | 235/9.25 |
| 10 mil C128 | 33/1.3 | 430/16.93 | 397/15.6 |
| 5 mil DM | 82/3.23 | 150/5.91 | 68/2.67 |
| 10 mil DM | 44/1.73 | 280/11.02 | 236/9.3 |
| 6.67 mil PDF | 48/1.89 | 295/11.61 | 247/9.72 |

### Table 4 — Environmental

| Characteristic | Parameter |
| --- | --- |
| Operating temperature | -30°C to 60°C [-22°F to 140°F] |
| Storage temperature | -40°C to 70°C [-40°F to 158°F] |
| Humidity (operating and storage) | up to 95 %RH, non-condensing at 60°C [140°F] |
| Shock | 3500 G for 0.4 ms at 23°C [73°F] |
| Vibration | 3 axes, 1 hour per axis: 2.54 cm (1 in) peak-to-peak displacement (5 Hz to 13 Hz)；10 G acceleration (13 Hz to 500 Hz)，1 G acceleration (500 Hz to 2,000 Hz) |
| Ambient light | 0 lux to 100,000 lux (total darkness to bright sunlight) |

### Table 5 — Symbologies

- **Linear:** Codabar, Code 11, Code 128, Code 2 of 5, Code 39, Code 93 and 93i, EAN/JAN-13, EAN/JAN 8, IATA Code 2 of 5, Interleaved 2 of 5, Matrix 2 of 5, MSI, GS1 Databar, UPC-A, UPC E, UPC-A/EAN-13 with Extended Coupon Code, Coupon GS1, Code…

## Laser Safety

- CLASS 2 LASER PRODUCT / APPAREIL A LASER DE CLASSE 2.
- N5703SR aimer: MAX. 1 mW: 630–680 nm, IEC 60825-1:2014, pulse duration 16.8 mSec；符合 21CFR 1040.10/1040.11（除 IEC 60825-1 Ed.3. 按 Laser Notice No. 56, May 8, 2019）。

## Warranty

15-month limited warranty，自 Honeywell 发货之日起算。
