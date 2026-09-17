# SR5750 — Android Wearable Computer Product Spec Sheet

> Source: `SR5750/specs/default_202601010000/SR5750 Product Spec Sheet.pdf`
>
> Update date shown in the source: 2026-04-23
>
> Product specifications are subject to change without prior notice.

## Meet the SR5750

The SR5750 is more than just a scanner—it is a fully integrated, enterprise-grade wearable computer built for next-generation warehouse operations. Combining high-performance Android computing with professional-grade scanning, it streamlines workflows from picking and inventory management to inbound and outbound logistics.

Weighing just 70 g, the SR5750 runs on Android and features a 2.1-inch AMOLED touchscreen, allowing workers to complete end-to-end workflows directly on the device.

Equipped with Wi-Fi 6, 2×2 MU-MIMO, and Bluetooth 5.3, the SR5750 delivers fast and stable connections. An optimized antenna design ensures consistent performance in any wearing mode.

A professional scan engine, paired with a 13 MP PDAF camera, enables simultaneous millisecond barcode decoding and high-resolution image capture.

Designed for flexibility, the SR5750 can be worn on the wrist, finger, back of the hand, or via a neck strap. Four physical buttons enable true hands-free operation, maximizing efficiency. In-display NFC allows instant login, seamless data exchange, and quick accessory changes, keeping workflows continuous throughout the shift.

## Product Highlights

### Compact, Mighty, All-in-one Host

Powered by a high-performance octa-core 2.0 GHz processor and Android 13, this compact wearable host delivers strong computing capability in a lightweight form factor. Featuring a tailored Watch UI, it enables users to complete end-to-end tasks directly on the device, eliminating the need to carry both a mobile computer and a ring scanner and simplifying workflows.

### 2.1-inch Touchscreen Display

The SR5750 delivers full Android computing through a responsive 2.1-inch AMOLED touchscreen, enabling users to view tasks, navigate workflows, and interact with applications directly on the device. The bright, high-clarity display requires no backlight and consumes less power, ensuring excellent visibility and longer battery life for uninterrupted operation.

### Reliable Connectivity

The SR5750 delivers seamless, real-time data flow with Wi-Fi 6 and Bluetooth 5.3, combining high-speed, low-latency, reliable wireless communication. It supports dense device connections with enhanced security and reduced congestion while optimizing BLE performance with faster pairing, extended range, improved power efficiency, and stable connections.

### Adaptable Wearability

The SR5750 supports wrist strap, glove, finger ring, back-of-hand, and neck-strap configurations, with left- and right-hand wear support. It adapts to picking, replenishment, sorting, and inspection tasks. Four tactile triggers, including a programmable shortcut key, provide precise control and flexibility.

### Intelligent Data Capture

The integrated scan engine quickly decodes standard and complex barcodes for high-volume workflows such as order picking and sortation. Motion and proximity sensors trigger automatic scans, reducing repetitive actions and improving ergonomics.

The 13 MP PDAF camera supports visual documentation such as damage verification and proof of process, eliminating the need for a secondary device.

### Simplified Device Provisioning and User Authentication

In-display NFC supports tap-to-log-in authentication, rapid device pairing, and streamlined staging, reducing IT deployment time while supporting shared-device environments common in multi-shift operations.

### Programmable Button: One-Touch Efficiency

The programmable button can be mapped to functions such as push-to-talk (PTT) communication or quick app launch. Users can access key functions with one press to reduce task steps and save time.

### Complex Tasks: Heads-Up, Hands-Free Operations

Paired with AR glasses or headsets via Bluetooth, the SR5750 provides real-time visual and voice guidance aligned with natural movement. Operators can stay focused ahead, reduce device checks and fatigue, and improve efficiency in complex tasks.

### Purpose-Built for Extreme Conditions

The SR5750 has IP67 sealing and 1.8 m drop resistance for reliable operation in picking zones, cross-docks, and high-mobility workflows.

### Visualized Fleet Management

UROVO UMS (Unified Management System) provides visualized management, enabling IT administrators to centrally manage multiple mobile devices from one dashboard across different device types and operating systems. It supports shared-device access control, application whitelisting and blacklisting, and granular user and device-group permissions.

From deployment to decommissioning, UMS streamlines device and smart-battery lifecycle management, remote data wipe, and password-policy enforcement, helping enterprises protect critical data while improving workforce productivity.

### Streamlined Device Setup and Enterprise Management

UROVO U-Stage makes device setup faster and simpler. A staging file containing the required configurations, settings, and applications can be deployed remotely, imported locally, or applied by scanning a QR code, without manual procedures.

## Specifications

### Performance Characteristics

| Parameter | Specification |
| --- | --- |
| CPU | Octa-core 2.0 GHz |
| AnTuTu score | 308,016 (V11) |
| Operating system | Android 13 |
| Memory | 4 GB RAM + 64 GB ROM |

### Physical Characteristics

| Parameter | Specification |
| --- | --- |
| Dimensions | 60 mm L × 58 mm W × 14 mm D |
| Weight | 70 g |
| Display | 2.1 inches, 410 × 502, AMOLED, 700 nits |
| Touch panel | Multi-mode capacitive touch with bare or gloved fingertip input or stylus (sold separately); Corning Gorilla Glass; water-droplet rejection; fingerprint-resistant anti-smudge coating |
| Power | Non-removable battery; standard capacity 3.85 V, 1150 mAh / 4.43 Wh; Smart Battery Management |
| Interface | Bottom: 5-pin charging connector and communication I/O; rear: 2-pin communication I/O |
| Notification | Audible tone, vibration, and LED |
| Keypad and buttons | On-screen keypad and Enterprise Keyboard; power button; functional button; dual-action side scan buttons |
| Voice and audio | One microphone; high-quality single speakerphone; Bluetooth wireless-headset support; SWB and FB audio |
| PTT hot key | Supports the functional button |

### Wireless LAN

| Parameter | Specification |
| --- | --- |
| Radio | IEEE 802.11 a/b/g/n/ac/d/h/i/r/k/v/w/mc/ax; 2×2 MU-MIMO; Wi-Fi 6; IPv4 and IPv6 |
| 5 GHz data rates | 802.11a/n/ac/ax, 20 MHz / 40 MHz / 80 MHz, up to 400 Mbps |
| 2.4 GHz data rates | 802.11b/g/n/ax, 20 MHz / 40 MHz, up to 286.8 Mbps |

The source's Wi-Fi label prints `Wi-Fi™6 (801.11ax)` while the protocol list correctly prints `802.11.../ax`; preserve the intended standard as IEEE 802.11ax without silently treating the printed `801.11ax` as a separate protocol.

#### Security and Encryption

- WEP, 40-bit or 104-bit.
- WPA/WPA2 Personal with TKIP and AES.
- WPA3 Personal with SAE.
- WPA/WPA2 Enterprise with TKIP and AES.
- WPA3 Enterprise with AES.
- EAP-TTLS with PAP, MSCHAP, or MSCHAPv2.
- EAP-TLS.
- PEAPv0-MSCHAPv2.
- PEAPv1-EAP-GTC.
- LEAP and EAP-PWD.
- WPA3 Enterprise 192-bit mode with GCMP-256 and EAP-TLS.
- Enhanced Open (OWE).
- WPA3-FT.
- SCV (Server Certificates Validation).

### Wireless PAN

| Parameter | Specification |
| --- | --- |
| Bluetooth | Configurable Class 1 and Class 2; Bluetooth v5.3; Classic Bluetooth (BR/EDR) and Bluetooth LE |

### Data Capture

| Parameter | Specification |
| --- | --- |
| Scanning | Standard Range 1D/2D scan engine; FlexRange 1D/2D scan engine optional; “presentation model” optional (source wording) |
| Camera | Top: 13 MP autofocus, flash LED, PDAF, and torch mode |
| NFC | ISO 14443 Type A; Sony FeliCa and ISO 15693 cards; Card Emulation via Host; MIFARE 1K/4K; MIFARE DESFire; ISO/IEC 18092 (Type F); Host Card Emulation; Peer-to-Peer |

### Sensors

| Parameter | Specification |
| --- | --- |
| Light sensor | Ambient light |
| Other sensors | Accelerometer, geomagnetic sensor, gyroscope, and proximity sensor; optional |

### User Environment

| Parameter | Specification |
| --- | --- |
| Operating temperature | -20°C to 50°C / -4°F to 122°F |
| Storage temperature | -40°C to 70°C / -40°F to 158°F |
| Humidity | 5% to 95%, non-condensing |
| Drop specification | 1.8 m / 5.9 ft drops to tile over concrete across the operating-temperature range, per MIL-STD-810H |
| Tumble specification | 1,000 tumbles at 1.6 ft / 0.5 m at room temperature without rugged boot |
| Sealing | IP67 |
| Vibration | 12.2 g PK sine, 10 Hz to 55 Hz; 2.0 mm double amplitude at constant displacement; 60-minute duration per axis across three axes |
| Thermal shock | -40°C to 70°C / -40°F to 158°F; 12 cycles, with each cycle consisting of one hour at -40°C and one hour at 70°C; two-hour recovery at room temperature before inspection |
| Electrostatic discharge | ±15 kV DC air discharge; ±8 kV DC direct discharge; ±8 kV DC indirect discharge |

## Software Solutions

### Enterprise Management

- Unified Management System (UMS)
- UStage Provisioning
- UTalk 2.0 PTT platform
- OTA / Firmware Update Management

### Device Productivity

- ScanWedge
- U-Browser
- Enterprise Launcher

### Diagnostics and Maintenance

- Log Capture
- WiFi Diagnostics
- Smart Battery Management

## Accessories

- Charging cradle for one SR5750 device.
- Four-slot charging cradle for four SR5750 devices.
- Watch band.
- Ring trigger.
- Neck strap.
- Back-of-hand mount.
- Scan grip.
- 10 W (5 V / 2 A) wall adapter and USB 2.0 Type-C cable.

## Industry and Applications

| Industry | Applications |
| --- | --- |
| Warehouse | Sorting; put-away; order picking |
| Transportation and logistics | Sorting; put-away; order picking; loading and unloading |
| Retail | Customer assistance; push-to-talk (PTT); team communication; item lookup |

## Contact Information

| Region | Email | Website | Address |
| --- | --- | --- | --- |
| UROVO PTE. LIMITED | urovo@urovo.com | en.urovo.com | 1 Raffles Place, #21-01 One Raffles Place Tower 1, Singapore 048616 |
| Urovo Europe | urovo@urovo.com | europe.urovo.com | de Maas 9, 5684PL, Best, the Netherlands |
| Urovo North America | urovo@urovo.com | us.urovo.com | 1990 Main Street, Suite 750, Sarasota, Florida 34236 |
