# Electronic Shelf Label Base Station Specifications (F24A7)

> Canonical original retained (bytes unchanged). PDF text layer is noisy (running header **1.6英寸系列** on pages 2–7). All 7 pages were rendered and inspected visually.
>
> - Original: `ESL/others/base-station-spec-en_202608182031/ESL_Base_Station_Specification_EN.pdf`
> - Cover titles: 电子价签 基站规格书 / ELECTRONIC SHELF LABEL BASE STATION SPECIFICATIONS
> - Version: 3.0, Base Station Specification Information, 2026/2/2, Tang Cunshe
> - Product named in body: **F24A7**
> - Pages: 7/7 inspected
> - Footer: https://www.urovo.com

The running header “1.6英寸系列” is printed on pages 2–7 of this base-station PDF. The body, drawings, and filename describe the F24A7 base station, not a 1.6-inch tag spec.

---

## Cover (page 1)

Chinese title **电子价签 基站规格书**. English title **ELECTRONIC SHELF LABEL BASE STATION SPECIFICATIONS**. Blue digital-city background. Four ESL mockups: Fresh Salmon €3.99 SPECIAL OFFER 200g; ORGANIC GREEN TEA $8.50 100% Natural; BIG SALE -50% NOW $15.99 with barcode and QR; SUMMER DEAL 55" 4K UHD SMART TV NOW $399 with 4K / HDD / Wi-Fi icons.

## Revision (page 2)

Header: **1.6英寸系列**. Page 2 /.

| Version Number | Description | Release Date | Author |
| --- | --- | --- | --- |
| 3.0 | Base Station Specification Information | 2026/2/2 | Tang Cunshe |

Remaining table rows are blank.

## Table of Contents (page 3)

1. Product Overview — 4
2. Product Advantages — 4
3. Product Specs — 5
4. Drawing (Unit: mm) — 7
5. Network structure — 7

## 1. Product Overview (page 4)

The **F24A7** electronic shelf label base station is an active RFID base station device operating in the **2.4GHz** frequency band. It can achieve omnidirectional/directional reading and writing functions when paired with omnidirectional/directional antennas. The product adopts an external antenna installation method, allowing flexible configuration of various omnidirectional and directional antennas. It features wide recognition range, high recognition rate, powerful functionality, high reliability, strong scalability, with a coverage distance of up to **100 meters**.

The F24A7 electronic shelf label base station has a simple and elegant appearance, compact and lightweight, sturdy and durable, with a sense of technology and modernity. The product adopts software fault tolerance and hardware anti-interference design, enabling it to work continuously and stably for a long time in harsh working environments.

## 2. Product Advantages (page 4)

1. The base station supports **100M Ethernet** communication interface and **WIFI**.
2. The base station supports control of matching electronic shelf labels.
3. The base station antenna adopts external installation, which can flexibly configure various omnidirectional and directional antennas to meet the needs of various application scenarios.
4. Provides a powerful API user interface, enabling quick integration and connection with the user's existing information systems for use.
5. The communication protocol is independently developed and can be customized and extended for special user requirements.
6. Supports **802.3af** standard **POE** power supply.

## 3. Product Specifications (pages 5–6)

### 3.1 Product Appearance (page 5)

3D render of a black rectangular unit with side cooling fins and a four-corner mounting base plate. Top surface: stylized wireless/signal icon. Front panel visible: two LED indicators (one red, one green), one RJ45 Ethernet port, a small rectangular service port, a green multi-pin terminal block, and a gold-threaded SMA antenna connector.

### 3.2 Technical Specifications

| Item | Value |
| --- | --- |
| CPU | Rockchip RK3128, quad-core, 1.3G |
| Memory | 1G |
| Built-in Storage | EMMC 8G |
| Operating System | Android |
| Network Support | Ethernet |
| Ethernet | 1 port, 10M/100M auto-negotiation Ethernet |
| RTC Real-Time Clock | Supported |
| Scheduled Power On/Off | Supported |
| RF Operating Frequency | 2.4G |
| Receiver Sensitivity | -95dbm |
| Communication Rate | 1Mbit/s |
| Recognition Angle | Omnidirectional / Directional (depending on whether a directional or omnidirectional antenna is used) |
| Polarization Mode | Vertical Polarization |
| Communication Interface | Standard: Ethernet port |
| APP Version Upgrade | Supports remote network upgrade |
| Application Software Platform | Provides Software Development Kit (SDK) and API |
| Light Strip / ESL Communication Protocol | Self-developed active electronic shelf label 2.4G wireless communication protocol |
| Wireless Operating Mode | Half-Duplex Mode |
| Wireless Communication Distance | 100m (depending on antenna and tag output power) |
| Power Supply Method | POE (802.3af_44-57V) / DC12V |
| Dimensions | 150mm×95.5mm×23.8mm (actual dimensions may have slight error) |
| Standby Current | <500mA (DC12V) |
| Operating Current | ≤2A (DC12V) |
| Operating Temperature | -20℃～+65℃ |
| Storage Temperature | -20℃～+85℃ |
| Operating Humidity | 5%RH-95%RH (non-condensing) |

Page 4 lists WIFI among advantages; the Network Support row on page 5 lists Ethernet only.

## 4. Drawings (Unit: mm) (page 7)

Front view: overall **150.20 mm** wide × **95.20 mm** high. Mounting holes **142.70 mm** horizontal × **86.70 mm** vertical, hole diameter **3.30 mm**. Side view total thickness **23.50 mm**; front bezel **2.50 mm**. Four-corner mounting holes. Front icon: hand/card with wireless arcs. Side cooling ribs.

These drawing values differ slightly from the table dimensions 150×95.5×23.8 mm.

## 5. Network Architecture (page 7)

Network users (laptops) and Controllers access a **WMS server** and **ESL server** via **Internet Network** (cloud) and **Lan Network**. Mobile users connect to the LAN. **TCP/IP** to field gateways:

- Gateway 1: **2.4G** to a three-color light tower (red/yellow/green) and ESL tags
- Gateway 2: **Bluetooth** to a handheld terminal that interacts with ESL tags

## Visual coverage

7/7 pages inspected.
