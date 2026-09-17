# UROVO Electronic Shelf Labels Overview

> Canonical original retained (bytes unchanged). Slide text layer plus visual inspection of all 22 rendered slides.
>
> - Original: `ESL/presentation/overview-en_202608182031/ESL-Presentation-EN-0514.pptx`
> - File title in core properties: 空白演示; last modified 2026-05-14; revision 167
> - Slides: 22/22 inspected (LibreOffice PDF render)
> - Speaker notes present on slides 1, 4, 7, 13, 14, 15, 19, 21 (Chinese notes on 13–15, 19, 21)

Source spelling on slides is preserved (Effciency, labeland, loT, Al shelf).

---

## Slide 1 — Cover

Aerial teal forest-road photo with trucks and light trails. Large white **UROVO**. Subtitle **Electronic Shelf Labels Overview**. Small urovo wordmark top-right. Digital overlay (squares, binary-like digits).

Notes: (empty in extraction)

## Slide 2 — Section 1

Blue geometric title card. Large **1**. **Why Electronic Shelf Labels?**

## Slide 3 — Why Electronic Shelf Labels?

Center ESL graphic: red **UROVO** header; product **Bika Pika/Bagi-bagi Stick Corn Snacks 40pcs/bag (Halal)**; price **S$5.53** with yellow **30%↓**; barcode and serial **A1250000219** on the left edge.

| # | Title | Body |
| --- | --- | --- |
| 01 | Accuracy | Price accuracy and eliminating pricing discrepancy between the labeland the register. |
| 02 | Product info | More product information for customers can be provided through expanded display options. |
| 03 | Picking Effciency | Navigation and LED lighting for order picking-generating a picking route with flashing lights to help delivery order pickers quickly find their next item. |
| 04 | Retail Digitalization | Serves as the building block loT device for communication with expanded retail digitalization technology from Al shelf monitoring to just-walk-out fully autonomous stores. |

## Slide 4 — Why Choose Electronic Shelf Labels From UROVO?

Three columns:

1. **End-to-End Solution** — Seamless Integration: complete ecosystem from high-performance ESLs and robust base stations to an intelligent cloud platform; single point of responsibility. Icon: networking/gateway silhouette.
2. **Reliability & Industrial-Grade Design** — Set-and-Forget Operation: industry-leading **15-year battery life** and **IP68** dust/water resistance; continuous maintenance-free operation. Icon: chip/antenna-like square.
3. **Powerful Management Platform** — Command at Your Fingertips: remotely manage prices, promotions, and templates for thousands of items across all stores from one dashboard. Icon: monitor with chart.

## Slide 5 — Section 2

Blue title card. Large **2**. **Product Matrix**

## Slide 6 — Four Different Sizes Of ESL

Four white four-color (black/white/red/yellow) tags, left to right:

| Caption on slide | Visible sample content |
| --- | --- |
| 1.54-inch | Two small square units; yellow price **3.99**, red **ORGANIC**, Horizon Organic Whole Milk |
| 2.13-inch | Vertical rectangle; red **MART**, 有机苹果, red apple icon, **¥25.00** |
| 2.66-inch | Horizontal; red **UROVO**, Bika Pika snack copy, **30% ↓**, **S$5.53**, vertical barcode |
| 4.2-inch | Square; **4.2 inch e-Paper**, **400*300 Pixel**, four color squares (white/red/yellow/black), Bluetooth and cloud icons, barcode, **MAC: D43D397CFCBC**, top-center bezel sensor/LED |

## Slide 7 — Panoramic Overview of Core Performance Parameters

Four modules. Values match the T2664 / 2.66-inch datasheet, presented here as “core” parameters:

**Wireless Communication:** 2.40–2.48 GHz; reception sensitivity better than -95dBm; 1 Mbit/s; GFSK; frequency error within 20ppm; stable communication within **100 meters**.

**Size & Environmental Adaptability:** **83mm × 42mm × 12mm**; operating -20℃ to 60℃; storage -30℃ to 70℃; humidity 5%–95% (non-condensing); **IP68**.

**Display Parameters:** **2.66-inch** e-ink; **184 × 360**; active area 30.69mm×60.05mm; pixel pitch 0.1668mm×0.1668mm; rectangular pixels.

**Battery Life:** Built-in **600mA** battery; standby 3uA; reception 10mA; transmission 20mA; with twice-daily refresh, battery life **up to 15 years**.

## Slide 8 — Ultra-Slim ESL

Left: same snack ESL sample as slide 3. Right features:

- **Multicolor Display:** black, red, white, and yellow
- **E-Paper Screen:** 1.54-inch, 2.13-inch, 2.66-inch, and 4.2-inch; high-resolution e-ink; **180°** wide viewing angle
- **Multicolor LED Indicator:** blinking LED for fast product locating
- **Built-in NFC:** standard NFC; instant updates with a tap
- **Customizable Templates:** QR codes, barcodes, images, color blocks, icons

## Slide 9 — Specifications (2.66-inch table)

Same table as the T2664 spec: RF 2.40～2.48G / -95dbm / 1Mbit/s / ≤20ppm / GFSK; private protocol; read 100m; activation 16S; size 83×42×12 mm; built-in battery ×2; 3uA / 10mA / 20mA; -20℃～60℃ / -30℃～70℃; humidity 5%–95%; screen 2.66 inches; 184×360; 30.69×60.05mm; 0.1668×0.1668mm; rectangle.

## Slide 10 — Electronic Shelf Label Base Station

Photo: black rectangular rugged unit with ribbed sides, top wireless/tag icon, thick black external antenna on top-left, shown roughly horizontal.

- Wide reading range up to **100 meters**; high tag recognition accuracy
- External **omnidirectional or directional** antennas
- **100Mbps Ethernet** port for base station ↔ backend
- Open **API** for IT integration

## Slide 11 — Base Station Specifications

| Group | Item | Value |
| --- | --- | --- |
| Hardware | CPU | Rockchip RK3128, Quad-core, 1.3G |
| Hardware | Cache | 1G |
| Hardware | Built-in memory | EMMC 8G |
| Hardware | Operating System | Android |
| Hardware | Network support | Ethernet |
| Hardware | Ethernet | One, 10M/100M Adaptive Ethernet |
| Hardware | RTC | Support |
| Hardware | power on/off | Support |
| RF | Operating frequency | 2.4G |
| RF | Reception sensitivity | -95dbm |
| RF | Communication rate | 1Mbit/s |
| RF | Identification angle | Omnidirectional/Directional |
| RF | Polarization | Vertical polarization |
| Interface | Communicate interface | Standard: Network port |
| Interface | App Version upgrade | Supports remote network upgrades |
| Interface | App software platform | Provide SDK and API |
| Light bar communication | Protocol | Self-developed 2.4G wireless protocol for active ESL |
| Light bar communication | Wireless working | Half-duplex mode |
| Light bar communication | Distance | 100m |

This slide’s hardware table does not list POE/DC12V, dimensions, or currents that appear in the F24A7 PDF spec.

## Slide 12 — Three-Step Implementation Guide

Three photo panels of NFC phone-to-tag workflow:

1. **USER DEVICE NFC TAP-TO-READ** — phone near white ESL; NFC arcs; Urovo app grid
2. **GET & MODIFY PRODUCT INFO** — form with **MAC: A12300000018**, product name Mineral Water (Chinese), barcode/price fields
3. **NFC TAP-TO-SYNC UPDATE** — green check **UPDATE SUCCESSFUL!**; overlay **ELECTRONIC SHELF LABEL UPDATED**; sample price changes **12.00** → **12.90**

## Slide 13 — Section 3

Blue title card. Large **3**. **Platform and System Software Architecture**

Notes: 平台与系统软件架构

## Slide 14 — Operations Management Ecosystem — Operation Management Platform

Three cards:

- **Strategic Foundation Module:** Insight Dashboards; Organizational Hierarchy
- **Universal Data Framework:** Intelligent Quick-start Templates
- **System Integrity & Security:** Comprehensive Audit Trails

Notes: 运营管理平台

## Slide 15 — Operations Management Ecosystem — Smart Digital Labeling Platform

Four columns:

- **Strategic Foundation Module:** Real-time Analytics; Granular Access Control (User/Role Management); Global Fleet Management
- **Data & Asset Library:** Product Management; Creative Layout Studio
- **Core Retail Execution:** ESL Lifecycle Management; Smart Infrastructure Connectivity; Precision Asset Pairing; Visual Pick-to-Light Tasks
- **Governance & Compliance:** Transparent Event Logs

Notes: 价签管理平台

## Slide 16 — Platform feature breakdown

Two columns (Operation Management Platform | Smart Digital Labeling Platform).

**Operation Management Platform**

- Basic Data Module — Organization Management; User Roles
- Business Data Module — Data Dashboard (price tags, products, base station quantities); Initial Templates (public templates for organizations)
- System Information Module — Operation Logs (various organizations)

**Smart Digital Labeling Platform**

- Basic Data Module — Store Management; User Roles (accounts and permissions)
- Business Data Module — Data Dashboard; Template Management (public + private); Product Management; Price Tag Management (push updates); Blink Task; Binding Records; Base Station Management
- System Information Module — Operation Logs (within the organization)

## Slide 17 — Application System Architecture

**Client:** PC ↔ Nginx; APP ↔ Nginx and APP ↔ MQTT.

**Application Server:** Nginx to File storage server, api, admin. File storage ↔ admin. api ↔ MySQL and Redis. admin ↔ Redis, MySQL, and MQTT.

## Slide 18 — Business Data Flow Diagram

Left paragraph: Users manage products, templates, and price tag information through the management platform, and push price tag or flashing light tasks to the base station APP via interface services and message push services. After receiving the messages, the base station APP performs operations on the price tags and feeds back the execution status through the interface.

Flow: Management Platform (Bind/Push, Flash Light Task) → Interface Program → MQ (Send Message) and Polling → Base Station → Electronic shelf label; Feedback from Base Station to Interface Program.

## Slide 19 — Section 4

Blue title card. Large **4**. **Simplified Deployment and Zero-touch Operations.**

Notes: 简化部署与零接触运维

## Slide 20 — Minimalist deployment, go live in four steps

1. **Base Station Installation** — ceiling or wall; POE switch; powered on and online
2. **Tag Activation** — activated within **16 seconds** after unboxing; auto-connect to strongest-signal base station
3. **Platform Deployment** — server backend, database, frontend, middleware; network connection of tags, base stations, devices
4. **Batch Binding** — batch bind products, one-click templates; thousands of tags in a store initialized within **two hours**

## Slide 21 — Zero-Touch Maintenance & Remote Control

1. **Real-Time Monitoring** — battery voltage, signal strength, refresh success rate; automatic low-battery alerts
2. **Remote Upgrade** — batch remote firmware upgrades; no manual disassembly
3. **Cleaning & Protection** — **IP68**; wash shelves with water jets without removing tags

Notes: 零接触维护与远程管控

## Slide 22 — Industry Solutions Empowered by Electronic Shelf Labels

Four photos with labels: **supermarket** (aisle/cart); **Drug Store** (pharmacy shelves); **Fashion** (cosmetics/lipstick counter); **Electronics** (phones on security stands).

## Visual coverage

22/22 slides inspected. Decorative icons/SVGs on later slides are section icons; product facts on those slides are transcribed above.
