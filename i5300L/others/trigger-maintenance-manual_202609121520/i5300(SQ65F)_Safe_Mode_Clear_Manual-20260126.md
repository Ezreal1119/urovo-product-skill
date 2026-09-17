# i5300L Trigger Maintenance Manual

> Canonical original: `i5300L/others/trigger-maintenance-manual_202609121520/i5300(SQ65F)_Safe_Mode_Clear_Manual-20260126.doc` (bytes and filename unchanged, including `i5300(SQ65F)`).
> SHA-256: `3491d4e7bed8c88327581c98da6175d9256351de790a49a28111ddad5daf2bfc`
> Companion inspection PDF was generated only for vision; it is not a canonical source.
> Visual protocol: **12/12** converted-PDF pages; **34/34** embedded `word/media` files inspected.
> Body title **i5300L Trigger Maintenance Manual**. Filename says i5300 / SQ65F; internal map is SQ65F = i5300L (SQ65B = i5300). Routed to the **i5300L** Hub, not i5300.
> Filename **Safe_Mode_Clear** does not match the body: this is a **hardware-trigger / tamper** repair guide (yellow/red lock screens), not a generic Android safe-mode UI manual.
> Filename date **20260126**. Not a live spec. Lead hard specs from `i5300L/specs/`.

---

## 1.1. Common Trigger Codes & Corresponding Circuits (page 1)

| Code | Meaning |
| --- | --- |
| 0xff000000 | System & SE communication failure |
| 0x71000000 | First system connection & activation after initial assembly |
| 0x72000001 | Channel 1 triggered |
| 0x72000002 | Channel 2 triggered |
| 0x72000003 | Channel 1 & 2 triggered simultaneously |
| 0x72000004 | Channel 3 triggered |
| 0x72000005 | Channel 1 & 3 triggered simultaneously |
| 0x72000006 | Channel 2 & 3 triggered simultaneously |
| 0x72000007 | Channel 1, 2 & 3 triggered simultaneously |
| 0x72000008 | Channel 4 triggered |
| 0x72000009 | Channel 1 & 4 triggered simultaneously |
| 0x7200000a | Channel 2 & 4 triggered simultaneously |
| 0x7200000b | Channel 1, 2 & 4 triggered simultaneously |
| 0x7200000c | Channel 3 & 4 triggered simultaneously |
| 0x7200000d | Channel 1, 3 & 4 triggered simultaneously |
| 0x7200000e | Channel 2, 3 & 4 triggered simultaneously |
| 0x7200000f | Channel 1, 2, 3 & 4 triggered simultaneously |
| 0x72000010 | Channel 5 triggered |
| 0x7200001x | Channel x & 5 triggered simultaneously |
| 0x7300xxxx | Physical trigger points installed, trigger state not cleared |

## 1.2. Trigger Fault Troubleshooting Examples (pages 1–2)

### Yellow screen (e.g., 0x73000002)

Device has experienced hardware trigger disconnection/short-circuit protection; now in pending activation state. Inspect for tampering; reassemble fully and perform trigger deactivation.

**Visual — yellow lock UI:** status bar **Turn on cellular data**. Banner **WARNING!** with code **(0x73000002)**. Body **This device has been locked. Please activate this device**. Toggles **No service** and **Select Wi-Fi**. Footer **ACTIVE**. Yellow header/footer chrome.

### Red screen (e.g., 0x72000002)

Device in protection trigger state; hardware trigger circuit remains open/shorted. From the trigger codes above, **0x72000002** indicates a **Channel 2** hardware trigger state. Follow the corresponding trigger troubleshooting steps below to inspect hardware issues one by one.

First check for missing components, then check for foreign matter affecting trigger contact, and replace the faulty parts accordingly. Reassemble and power on the device for verification. If the issue persists with the same code, replace the components of the corresponding trigger circuit one by one until the device returns to the state shown in the previous example. If fault persists, swap face shell, main-board, or rear shell to isolate the faulty assembly.

**Visual — red lock UI:** same layout as the yellow screen; banner **WARNING!** with **(0x72000002)**; footer **ACTIVE**; bottom chrome **safe mode**.

## 1.3. Trigger Maintenance

### 1.3.1. RTC Battery Voltage Check (pages 2–3)

For all red trigger screens, first check whether the RTC battery voltage is within the standard range. If the RTC is faulty, replace the RTC battery before proceeding with trigger inspection and repair.

As shown in the figure below: **A** is the left test point of the RTC, **B** is the right test point of the RTC, and **C** is the grounded shell of the SIM card holder. Both conditions must be satisfied for the RTC battery to be qualified:

1. Multi-meter in mV range: measure points A & B; voltage **<5 mV** (The measured voltage must be less than 5 mV. A momentary spike exceeding 5 mV also results in a FAIL.)
2. Multi-meter in V range: measure point A & C; voltage **>3.1 V**.

**Visual:** white printer-top POS (sample unit, **UROVO** visible on the printer deck) with the battery well open; red arrows to RTC test points. Fluke-style meter: one shot near **2.0** on the mV range (red probe circled); second shot **3.1951** V with a probe on the SIM-holder ground. Printed circuit block diagram under the heading **Channel 1 Trigger** (series blocks: Channel 1 Trigger → zebra strip / carbon particles / zebra strip / baffle / LCD connector pins).

### 1.3.2. Channel 1 Trigger (pages 3–6)

Inspect in the order of the figures above from left to right, top to bottom. If any abnormality is found, replace the components at the relevant positions sequentially.

Figures **1.1–1.9** (photos of rear-shell carbon particles / zebra strips, KeyMesh / LCD-connector pins, PCB pins 1 & 5, LCD FPC pin **12** / **6** / GND, mainboard LCD connector).

1. Inspect rear shell anti-tamper carbon particles and zebra strips: replace if missing, deformed, or dirty. (Figure 1.1 & 1.2)
2. Check KeyMesh continuity: Press and hold C1 and C2, measure with the multi-meter in diode mode. Connect the red probe to B and the black probe to pin 6 of the LCD connector (normal voltage range: **0.5V–1V**). If the KeyMesh is damaged, replace it with a new one for verification. (Figure 1.3 & 1.4)
3. Check PCB pins 1 & 5 continuity: First press switch1 with a carbon particle. Use a multi-meter in resistance mode to measure the continuity between pin 1 and pin 5 (normal: **R ≤ 100 Ω**). Then measure the insulation resistance between pin 1 and GND, and between pin 5 and GND (normal: Multi-meter displays **OL**). If the measured resistance is abnormal, replace the PCB for verification. (Figures 1.5, 1.6 & 1.7)
4. Ensure LCD_FPC is fully seated to main-board LCD connector; reconnect if loose.
5. Check the LCD FPC for cracks or damage. Use a multi-meter in resistance mode to measure the resistance between pin 12 and pin 6 of the FPC (normal: approximately **R ≤ 50 Ω**). Then measure the insulation resistance between pin 12 and GND, and between pin 6 and GND (normal: Multi-meter displays **OL**). If the LCD FPC is damaged, replace the front case assembly for verification. (Figure 1.8)
6. Check the main-board LCD connector for dirt or damage (check for cold solder joints on the base and deformation of the connector). Clean the dirt, re-solder, or replace the connector if necessary. (Figure 1.9)
7. Replace main-board if all above are normal but trigger remains.

### 1.3.3. Channel 2 Trigger (pages 6–9)

Figures **2.1–2.6**. Inspect left to right, top to bottom.

1. Inspect main-board large zebra strip and front case small zebra strip: replace if missing, deformed, or dirty. (Figure 2.1 & Figure 2.2)
2. Check KeyMesh continuity: Press and hold C1 and C2, measure with the multi-meter in diode mode. Connect the red probe to B and the black probe to **A1** (normal voltage range: **0.5 V–1 V**). If the keyMesh is damaged, replace it with a new one for verification. (Figure 2.3)
3. Check the LCD Mesh for damage. Use a multi-meter in resistance mode to measure the resistance between pin 2 and pin 4 (normal: **R ≤ 500 Ω**). Then measure the insulation resistance between pin 2 and GND, and between pin 4 and GND (normal: Multi-meter displays **OL**). Replace the LCD Mesh if it is damaged or the resistance is abnormal. **(Note: LCD Mesh is a disposable component; it will be damaged once peeled off.)** (Figure 2.4)
4. Check the continuity between pin 2 and pin 4 on the PCB: Use a multi-meter in resistance mode to measure the resistance (normal: **R ≤ 100 Ω**). Then measure the insulation resistance between pin 2 and GND, and between pin 4 and GND (normal: Multi-meter displays **OL**). Replace the PCB for verification if the resistance is abnormal. (Figure 2.5 & Figure 2.6)
5. Replace main-board if all above are normal but trigger remains.

Callout overlay on the mesh photo: pins **1**, **4**, **GND**.

### 1.3.4. Channel 3 Trigger (pages 9–10)

Figures **3.1–3.3**. Overlay pins **2**, **5**, **GND**.

1. Inspect front case zebra strip and anti-tamper carbon particles: replace if missing, deformed, or dirty. (Figure 3.1)
2. Check the continuity of the KeyMesh: Press and hold C1 and C2, measure with the multi-meter in diode mode. Connect the red probe to B and the black probe to **A2** (normal voltage range: **0.5 V–1 V**). If the KeyMesh is damaged, replace it with a new one for verification. (Figure 3.2)
3. Check the LCD Mesh for damage. Use a multi-meter in resistance mode to measure the resistance between pin 2 and pin 5 (normal: **R ≤ 500 Ω**). Then measure the insulation resistance between pin 2 and GND, and between pin 5 and GND (normal: Multi-meter displays **OL**). Replace the LCD Mesh if it is damaged or the resistance is abnormal. **(Note: LCD Mesh is a disposable component; it will be damaged once peeled off.)** (Figure 3.3)
4. Replace main-board if all above are normal but trigger remains.

### 1.3.5. Channel 4 Trigger (pages 10–11)

Figures **4.1–4.3**. Overlay pins **3**, **12**.

1. Ensure magnetic head FPC is fully seated to main-board magnetic head connector; reconnect if loose. (Figure 4.1)
2. Check the magnetic head FPC for cracks or damage. Use a multi-meter in resistance mode to measure the resistance between pin 3 and pin 12 (normal: approximately **R ≤ 10 Ω**). Replace the magnetic head for verification if the FPC is damaged or the resistance is abnormal. (Figure 4.2)
3. Check the magnetic head connector for contamination or damage (check for cold solder joints on the base and deformation of the connector). Clean, re-solder, or replace the connector if necessary. (Figure 4.3)
4. Replace main-board if all above are normal but trigger remains.

### 1.3.6. Channel 5 Trigger (pages 11–12)

Figures **5.1–5.2**.

1. Inspect back case anti-tamper carbon particles: replace if missing, deformed, or dirty. (Figure 5.1)
2. Clean main-board corresponding gold fingers if contaminated or blocked. (Figure 5.2)
3. Replace main-board if all above are normal but trigger remains.

**Visual — remaining photos:** close-ups of carbon particles on the rear shell, zebra strips, gold fingers, magnetic-head FPC, and LCD/mesh connectors. No additional trigger codes beyond the table on page 1.
