# UPad — Enterprise Tablet

> **Source Hub**: [[products/UPad|UPad Source Hub]]

> Source: UPad/specs/default_202601010000/UPad Product Spec Sheet.pdf

Category: [[categories/other-devices|Enterprise Tablet]]

> [!warning] Active source discrepancies
> The current product specification uses “under 7 mm” in marketing copy and the 2026-08-26 Europe brochure states 7 mm, but the product specification table and newer accessory-system specification list 260 × 180 × 11 mm. The product specification supports MicroSD up to 1 TB, while the accessory-system specification states 2 TB. Preserve both values with source qualification until resolved.

## Overview

UPad is a next-generation commercial mobility platform combining payment, data capture, and modular scalability in a portable form factor. Built for modern retail and enterprise operations with Wi-Fi 6E connectivity, in-display RFID, and an 11-inch WUXGA display.

## Product Highlights

**11" WUXGA Display** — Large, clear viewing experience in a precision-crafted metal body at 500 g. Source materials disagree between an “under 7 mm” marketing claim and an 11 mm tabulated dimension.

**Dual-Mode Data Capture** — Integrated barcode scanner + in-display RFID reader for fast reading of barcodes and RFID tags.

**Quick-Lock Modular Design** — Magnetic snap-on system for secure attachment to modular accessories in seconds.

**SoftPOS Payment** — Contactless payment directly on the tablet.

**Wi-Fi 6E Connectivity** — High-speed, low-latency wireless for seamless real-time data synchronization.

**Smart Battery Management** — 8000 mAh service-replaceable battery for sustained operation.

## Specifications

| Parameter | Specification |
| --- | --- |
| Display | 11 inch WUXGA |
| Dimensions / thickness | 260 × 180 × 11 mm in the specification tables; “under 7 mm” in marketing copy (unresolved) |
| Weight | 500 g |
| Processor | Qualcomm 4390 octa-core, 2.2 GHz (new accessory-system specification) |
| OS | Android 16, upgradable to Android 20 |
| Battery | 3.87V, 8000 mAh, 30.96Wh |
| Camera | Rear: 16 MP autofocus; Front: 8 MP fixed focus |
| Scanner | Integrated barcode scanner |
| RFID | In-display RFID reader |
| Payment | SoftPOS contactless |
| Wi-Fi | Wi-Fi 6E |
| Modular | Magnetic quick-lock accessories |

## Storage Difference

| Field | Current product specification | 2026-07-22 accessory-system specification |
| --- | --- | --- |
| Maximum MicroSD capacity | 1 TB | 2 TB |

The sources do not explain whether this is a revision or configuration difference. Do not present either capacity as universal without identifying its source.

## Dual-Screen Printer Dock

The current accessory-system source describes a multifunction dock and thermal printer intended for UPad deployments.

### Dock

- 2 × USB Type-A 3.0, 2 × USB Type-A 2.0, 1 × USB Type-C 3.0.
- RJ45, RJ12, COM serial, Micro USB debug, and a 4-pin power connector.
- Adapter input: 100–240 V AC; printed output: 24 V / 3 A DC, marked **“具体待定” (to be determined)**.
- Operating temperature 0°C to 55°C; storage -40°C to 70°C; 5% to 95% RH non-condensing.
- ESD: ±15 kV air discharge and ±8 kV contact discharge.

### Thermal Printer

| Parameter | Specification |
| --- | --- |
| Printing | Direct thermal, 203 dpi |
| Maximum speed | 250 mm/s |
| Maximum print width | 72 mm |
| Paper | 58 mm / 80 mm; maximum roll diameter 80 mm |
| Media | Receipt paper and liner-backed labels |
| Cutter | Partial cut and full cut |
| Sensors | Paper-out and cover-open alerts |
| Communication | USB and Bluetooth |
| Power | Supplied by the dock |

See [[products/UPad|UPad Source Hub]] for the complete current source set and exact provenance.

## Target Industries

Retail, Enterprise, Service, Mobile Operations
