# FR2000 Desktop RFID (UHF) Reader — User Manual

> Original: `FR2000/user_guide/default_202608142020/User_Manual_for_FR2000_Desktop_RFID.docx`
>
> Document copyright: © 2023 Urovo Technology, Co., L. All rights reserved.
>
> Conversion note: This Markdown preserves the document's body text, tables, operational values, and material text embedded in screenshots. Product-only photographs and decorative graphics are represented by concise descriptions because synchronized source directories do not retain extracted images. Values shown in screenshots are identified as examples and must not be generalized beyond the depicted workflow.

## Statement

Without written permission from Urovo, no part of this publication may be reproduced or used in any form or by any electronic or mechanical means. This includes electronic or mechanical methods such as photocopying, recording, or information storage and retrieval systems. Information in this manual is subject to change without notice.

The software is provided strictly “as is.” All software, including firmware, provided to the user is licensed. Urovo grants the user a non-transferable and non-exclusive license to use each software or firmware program delivered under this agreement (the License Program). Except as expressly provided below, the user may not transfer, sublicense, or otherwise transfer this license without the prior written consent of Urovo. Unless permitted by copyright law, the user has no right to copy all or part of the licensed program. Without written permission from Urovo, the user may not modify, merge any form or part of the licensed program, or combine it with other program materials, create derivative works from the licensed program, or use the licensed program on a network.

The user agrees to retain Urovo's copyright notice on the authorized program delivered under this agreement and include the same copyright notice in full or in part in any authorized copies made by them. The user agrees not to decompile, disassemble, decode, or reverse engineer any licensed program or any part thereof delivered to the user. Urovo reserves the right to modify any software or product to improve reliability, functionality, or design. Urovo assumes no responsibility for any product liability arising from or related to the use or application of any product, circuit, or application described herein. No license, whether express or implied, estoppel, or otherwise, is granted to any Urovo technology intellectual property. Implied licenses apply only to devices, circuits, and subsystems included in Urovo products. Other product names mentioned in this manual may be trademarks or registered trademarks of their respective companies, and are hereby acknowledged.

## Contents

1. Appearance
2. Indicator Light Explanation
3. Get Started
   - 3.1 Connection
   - 3.2 Connection and Power Supply
   - 3.2.1 To Windows
   - 3.2.2 To Android
4. Setup
   - 4.1 Baud rate
   - 4.2 Output power
   - 4.3 Protocol
   - 4.4 Region
   - 4.5 Buzzer
   - 4.6 Temperature
5. RFID Tag Read and Write Operations
6. RFID Tag Lock and Kill
7. Environmental
8. Safety Precautions
9. Develop option
10. Troubleshooting
11. Appendix 1 — Specifications

## Chapter 1. Appearance

FR2000 is a state-of-the-art desktop UHF reader developed by Urovo Technology. This reader is versatile, supporting applications on Windows, Android, and iOS platforms. With its cutting-edge E710 RFID chip and proprietary high-efficiency signal processing algorithms, FR2000 excels in read-write capabilities across a broad reading range. Its exceptional performance allows for the precise reading of RFID tags from all directions, achieving an accuracy rate of up to 99.9%.

Designed for various applications, FR2000 is ideal for retail collection, logistics, identity verification, access control, anti-counterfeiting systems, and production process control. Its adaptability and accuracy make it a reliable choice for businesses across diverse industries.

The appearance pages show a thin square desktop reader pad with rounded corners, a dark reading surface, feet on the underside, and a rear connection area containing three status lights, a USB Type-C port, and an RJ45 port.

## Chapter 2. Indicator Light Explanation

The indicator lights on the device display different statuses, including power-on and communication status.

| Label | Indicator / function | Color or behavior shown |
| --- | --- | --- |
| BT | Bluetooth indicator / Bluetooth detected indication | Blue |
| WORK | Working-status / operation indicator; tag-detected indication | Green |
| PWR | Power-status / power-on indicator | Red |
| LAN | Ethernet connection and activity indicators | Connection and activity lights are shown on the RJ45 port |
| Buzzer | Audible tag-reading feedback | Beeps when tags are read successfully |

The source diagram also labels the three device LEDs `BT`, `WORK`, and `PWR`, and states that successful tag reading produces a buzzer prompt.

## Chapter 3. Get Started

### 3.1 Connection

**Real-time communication, interconnection**

The reader supports Type-C USB 2.0, Bluetooth BT5.0, RJ45 network-port, and other communication methods. It can interconnect with Windows, Android, iOS, and other devices with different operating systems to meet different operational scenarios.

### 3.2 Connection and Power Supply

The connection diagram shows Windows, Android, and iOS devices communicating with FR2000 through Bluetooth, Type-C, or RJ45-LAN.

The reader supports USB power supply and an optional PoE power-supply mode. A USB Type-C cable or RJ45 interface cable can complete data transmission and power-supply operations, reducing deployment and maintenance costs. Another diagram illustrates a single FR2000 connected to a computer for both power and data, and multiple FR2000 readers connected to network equipment.

### 3.2.1 To Windows

#### 3.2.1.1 Install the Driver

If USB is used for data communication, install the USB driver first.

The source screenshot shows the `CP210x_VCP_Windows` directory with these items:

| Item | Displayed modified time |
| --- | --- |
| `x64/` | 2023-07-26 18:27 |
| `x86/` | 2023-07-26 18:27 |
| `CP210xVCPInstaller_x64.exe` | 2013-10-25 11:39 |
| `CP210xVCPInstaller_x86.exe` | 2013-10-25 11:39 |
| `dpinst.xml` | 2013-10-25 11:39 |
| `ReleaseNotes.txt` | 2013-10-25 11:39 |
| `SLAB_License_Agreement_VCP_Windows.txt` | 2013-10-25 11:39 |
| `slabvcp.cat` | 2013-10-25 11:39 |
| `slabvcp.inf` | 2013-10-25 11:39 |

After installation, Windows Device Manager should show the device under **Ports (COM & LPT)**. The source example identifies it as `Silicon Labs CP210x USB to UART Bridge (COM8)`.

#### 3.2.1.2 Connect

1. Open `UHF Reader Pad\Demo\Demo\c#\EXE\UHFReader288Demo.exe` or another compatible demo.
2. Select the COM port shown in Device Manager.
3. The Windows demo screenshot uses `RS232`, serial port `COM8`, and baud rate `57600bps` as example values.

If the device has an RJ45-LAN port, use its IP address to connect. The TCP/IP screenshot uses these example values:

| Field | Example value |
| --- | --- |
| Connect type | TCP/IP |
| IP address | `192.168.0.250` |
| Port | `27011` |

### 3.2.2 To Android

#### 3.2.2.1 Search the Bluetooth Device

The Bluetooth name can be found on the bottom label or read in `UHFReader288Demo.exe`. Pair with the desktop RFID reader using PIN `1234`.

The source screenshots show an example device named `BT22522001` with address `DC:0D:30:52:7A:A1`. The Android pairing dialog notes that common PINs are `0000` or `1234`; this manual specifically instructs the user to enter `1234`. The Windows demo's example reader serial number is `22522001`.

#### 3.2.2.2 Open the App and Demonstration

##### 3.2.2.2.1 Connect to the RFID Device

Open the Bluetooth connection. After connection, the firmware version is shown. The example app screen contains tabs `CONNECT`, `CMD`, and `18000-6C`, displays firmware version `1.1`, and provides `Buzzer on`, `Buzzer off`, and `SET` controls.

##### 3.2.2.2.2 Setting Page

The example `CMD` page shows:

| Field | Example value or option |
| --- | --- |
| Frequency band | Chinese band2 |
| Minimum frequency | 902.75 MHz |
| Maximum frequency | 927.25 MHz |
| Power | 30 |
| Antenna selections displayed | Antenna1, Antenna2, Antenna3 |
| Actions | READ, SET |

The adjacent source text states: **Power (0–27 dBm), only one antenna.** This differs from the screenshot's displayed value of `30` and from the appendix's “up to 30 dBm” statement; preserve the contexts separately.

##### 3.2.2.2.3 Reading Tags

The example tag-reading screen shows `Antenna1` selected, a tag count of `2`, a `SCAN` button, and a `TID Check` option.

| EPC example | Times | RSSI | Antenna (4–1) |
| --- | ---: | ---: | --- |
| `23487654321573118ABCCCCC1511257` | 5 | 104 | `0001` |
| `E20051161502004220803C88` | 5 | 107 | `0001` |

## Chapter 4. Setup

### 4.1 Baud Rate

Use the demo's `RS232/485 baud rate` control to set the communication baud rate. The source screenshot uses `57600bps`.

### 4.2 Output Power (0–27 dBm)

Use the demo's `Power` control and `Set` action to configure output power. The source screenshot highlights `27 dBm`.

### 4.3 Protocol

Only ISO 18000-6C is supported.

### 4.4 Region

The Windows demo screen lists these region choices: Chinese band1, Chinese band2, US band, Korean band, EU band, US band3, and ALL band. The example selects `ALL band` and displays a minimum frequency of `840 MHz` and maximum frequency of `930 MHz`; it also includes a `Single` option and a `Set` action.

### 4.5 Buzzer

The demo provides `Open`, `Close`, and `Set` controls for the buzzer.

### 4.6 Temperature

Use `Working temperature monitoring` and the `Get` action to read device temperature. The source screenshot displays `25°C` as an example.

## Chapter 5. RFID Tag Read and Write Operations

1. Place the RFID tag to be read or written within the device's reading range.
2. Start the software, select the read or write operation, and follow the on-screen prompts.

**Note:** The default password is `00000000`.

The Windows demo screenshots show the `EPCC1-G2` and `Read/Write Tag` areas. The illustrated workflow first starts inventory, selects a tag, and then opens the read/write controls. The sample inventory includes EPC values `E20051161502004220803C88` and `123487654321573118ABCCCCC1511257`.

The read/write interface includes:

- A selected-tag field and tag list.
- Mask fields for start address (hex), length (hex), memory (`EPC`, `TID`, or `User`), and data (hex).
- `Read Data / Write Data / Block Erase` controls with start address, decimal length, password, read/write data, automatic PC calculation, and memory-bank choices (`Reserve`, `EPC`, `TID`, `User`).
- Example values: start address `0000`, length `4`, read/write data `0000`, PC `0800`, and password `00000000`.
- Actions including `Read`, `Write`, `Ext Read`, `BlockWrite`, `BlockErase`, and `Ext Write`.

## Chapter 6. RFID Tag Lock and Kill

The `Read/Write Tag` screen contains protection, lock, kill, EPC-write, privacy, and alarm controls. The source example uses selected tag `E20051161502004220803C88`.

### Protection and Lock Controls

- Protection targets: Kill Password, Access Password, PC, TID, and User.
- Lock states: Unlock, Lock, Unlock forever, and Lock forever.
- Password fields use hexadecimal values; the example displays `00000000`.
- An additional `U9` option and `Lock` action are shown.

### Kill and EPC Controls

- `Kill Tag` accepts a hexadecimal kill password and provides a `Kill` action.
- `Write EPC` accepts an EPC value and password and provides a `Write EPC` action.

### Read Protection and Privacy Controls

- `Read Protection-NXP` accepts a hexadecimal password.
- Actions shown: `Set Privacy By EPC`, `Set Privacy Without EPC`, `Reset Privacy`, and `Detect Privacy`.
- The adjacent alarm area provides password fields, `Configure`, `Alarm` / `No Alarm`, and `Detect` controls.

## Chapter 7. Environmental

- Position the FR2000 on a stable surface and ensure good ventilation in the surrounding environment.
- Avoid use in humid, high-temperature, or extreme-temperature conditions to prevent device performance from being affected.

## Chapter 8. Safety Precautions

When operating a desktop UHF reader such as FR2000, observe the following safety precautions to maintain a secure and efficient usage environment.

### Electrical Safety

- Connect the UHF reader only to power sources that comply with the voltage and power requirements specified in the manual.
- Avoid exposing the device to water or moisture to prevent electrical hazards.

### Ventilation

Ensure proper ventilation around the desktop UHF reader to prevent overheating. Do not block ventilation openings.

### Handling and Placement

- Handle the UHF reader carefully; do not drop it or subject it to physical impact.
- Place the reader on a stable, flat surface to prevent accidental falls.

### Cleaning

- Disconnect the UHF reader from the power source before cleaning.
- Use a soft, dry cloth. Do not use liquid or abrasive cleaners.

### RFID Tags

- Handle RFID tags carefully to prevent damage.
- Do not place metal objects or other interference sources near the reader, because they may affect performance.

### Firmware and Software Updates

Follow the manufacturer's guidelines for firmware and software updates to maintain security and optimal functionality.

## Chapter 9. Develop Option

Maintain continuous communication with technical personnel to obtain development materials.

The source screenshot shows `UHF Reader Pad/Demo/Demo/` containing:

| Development folder | Displayed modified time |
| --- | --- |
| `android/` | 2023-12-19 19:03 |
| `c#/` | 2022-12-09 16:35 |
| `C++/` | 2022-10-14 18:05 |
| `JAVA/` | 2021-10-16 17:07 |

## Chapter 10. Troubleshooting

- If issues occur during use, refer to the accompanying troubleshooting guide or contact the customer-service team for assistance.
- For further support, contact the customer-service team.

The source ends this chapter with: “Thank you for choosing the FR2000 Desktop RFID (UHF) Reader, and we wish you a pleasant user experience!” followed by “Will update...”

## Appendix 1. Specifications

### Basic Specifications

| Group | Item | Specification |
| --- | --- | --- |
| Basic | Model | UROVO FR2000 |
| Basic | Dimensions | 325 mm × 325 mm × 20 mm |
| Basic | Weight | 1850 g |
| RFID | Chip / protocol | Based on Impinj E710; fully supports ISO 18000-6C (EPC Class 1 Gen 2) protocol tags |
| RFID | Frequency | 840–960 MHz; frequency customization optional |
| RFID | Transmission | FHSS or fixed-frequency transmission; supports RSSI |
| RFID | RF output power | Up to 30 dBm, adjustable |
| RFID | Antenna / range | Built-in antenna; typical effective reading distance <50 cm |
| Power | Power supply | Type-C USB 2.0 power supply; PoE optional |
| Interfaces | Communication | Type-C USB 2.0; Bluetooth 5.0 and RJ45 optional |
| Environment | Operating temperature | -20°C to +50°C |
| Environment | Storage temperature | -40°C to +70°C |
| Environment | Humidity | 5% RH–95% RH, non-condensing |
| Environment | Sealing | IP54 |
| Environment | ESD | ±15 kV air; ±8 kV contact |

### Power Supply

Unless otherwise noted, the specifications are taken under `TA = 25°C` and `VCC = +5V` operating conditions.

| Item | Symbol | Minimum | Typical | Maximum |
| --- | --- | ---: | ---: | ---: |
| Power Supply | VCC | 4.8 V | 5 V | 5.5 V |
| Current Dissipation | IC | — | — | 2.5 A |

### Interfaces and Indicators

| Name | Item | Description | Remark |
| --- | --- | --- | --- |
| BT | Bluetooth LED | Bluetooth detected indication | Blue |
| WORK | Operation LED | Tag detected indication | Green |
| PWR | Power LED | Power-on indication | Red |
| USB INTERFACE | USB | Type-C USB 2.0 | — |
| BUZZER | Buzzer | Power-on indication | — |

Depending on the model and configuration, the power supply, communication interfaces, and indicator lights on the device may be adjusted slightly. Refer to the actual device configuration.

### Accessories

| Accessory class | Type |
| --- | --- |
| Standard Accessory | Type-C cable × 1 |
