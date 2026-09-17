# i9200 Trigger Repair Guidebook

> Canonical original: `i9200/others/trigger-repair-guidebook_202609121520/i9200 Trigger Repair Guidebook V1.0.doc` (bytes and filename unchanged; spaces retained).
> SHA-256: `26ce4929e7c003fe37d35d69e1530a129fbe6570924d50daeee3ef8efc764b42`
> Companion inspection PDF was generated only for vision; it is not a canonical source.
> Visual protocol: **7/7** converted-PDF pages; **12/12** embedded `word/media` files inspected.
> Inbox also contained byte-identical `i9200(SQ68)_Safe_Mode_Clear_Manual.doc` (same SHA-256). One original retained under this filename. The duplicate is **not** a separate safe-mode UI manual.
> Body is trigger codes / circuit repair. i9200 maintenance manual §5.1 points here as the **Trigger Maintenance Guide**.
> Not a live spec. Lead hard specs from `i9200/specs/`.

---

## Common trigger codes and corresponding trigger circuit (pages 1–2)

| Code | Meaning |
| --- | --- |
| 0xff000000 | System and SE communication failure |
| 0x71000000 | Online activation for the first time |
| 0x72000001 | One-way trigger |
| 0x72000002 | Two-way trigger |
| 0x72000003 | One-way and two-way trigger |
| 0x72000004 | Three-way trigger |
| 0x72000005 | One-way and three-way trigger |
| 0x72000006 | Two-way and three-way trigger |
| 0x72000007 | One-way、two-way and three-way trigger |
| 0x72000008 | Four-way trigger |
| 0x72000009 | One-way and four-way trigger |
| 0x7200000a | Two-way and four-way trigger |
| 0x7200000b | One-way、two-way and four-way trigger |
| 0x7200000c | Three-way and four-way trigger |
| 0x7200000d | One-way、three-way and four-way trigger |
| 0x7200000e | Two-way、three-way and four-way trigger |
| 0x7200000f | One-way、two-way、three-way and four-way trigger |
| 0x72000010 | Five-way trigger |
| 0x7200001... | ...and Five-way trigger |
| 0x72000100 | Low temperature trigger |
| 0x72000200 | High temperature trigger |
| 0x72000400 | RTC battery low voltage trigger |
| 0x72000500 | RTC battery low voltage and low temperature triggered simultaneously |
| 0x72000600 | RTC battery low voltage and high temperature triggered simultaneously |
| 0x72000800 | RTC battery high voltage trigger |
| 0x72000900 | RTC battery high voltage and low temperature triggered simultaneously |
| 0x72000a00 | RTC battery high voltage and high temperature triggered simultaneously |
| 0x74000001 | Key vector table self-test failed |
| 0x74000002 | High pass side key self-test failed |
| 0x74000004 | SE side key self-test failed |
| 0x74000003 | Key vector table and high pass side key failed self check simultaneously |
| 0x74000005 | Key vector table and SE side key self check failed simultaneously |
| 0x74000006 | Simultaneous self-test failure of Qualcomm side key and SE side key |
| 0x74000007 | Key vector table, high pass side key, SE side key failed self check simultaneously |
| 0x73000…… | Trigger status not deactivate |

Source punctuation **、** in several rows retained. **High pass** / **Qualcomm** both appear for the side-key self-test rows.

## Example of trigger issue check (pages 2–3)

After the device is switched on, if it prompts the yellow interface shown in the figure below (e.g. code **0x73000002**), it means that the device has been triggered by the hardware to disconnect or short the protection line signal, and it is now in the state of being activated, so check whether the device's appearance has been dismantled or damaged. If not, assemble the device completely and do the de-trigger activation action.

**Visual — yellow lock UI:** **Turn on cellular data**. **WARNING!** **(0x73000002)**. **This device has been locked. Please activate this device**. Toggles **No service** and **Select Wi-Fi**. Version **(1.40.25.061236)**. Footer **ACTIVE**. Yellow header/footer chrome.

If the red interface shown in the figure below is prompted after the device is switched on (e.g. code **0x72000008**), it means that the device is already in the protection triggering state, and the hardware trigger protection line is still in the open circuit or short circuit state. **0x72000008** is a **four-way** hardware trigger state. Check hardware problems one by one: first check whether the material has been missed, then check whether there is any foreign matter affecting the trigger contact, and replace the corresponding abnormal material, then assemble and switch on. If the problem still exists and the code is the same, replace the corresponding trigger circuit materials one by one until the device returns to the corresponding picture of the previous example. Finally, replace components to lock the problem location (face shell components, motherboard components, rear shell components, etc.) to see if the fault follows the components.

**Visual — red lock UI:** status **47%**. **Turn on cellular data**. **WARNING!** **(0x72000008)**. Same locked-device body. Version **(1.40.25.061204)**. Footer **ACTIVE**. Bottom chrome **safe mode**.

## RTC battery voltage check (page 4)

For all red trigger interfaces, first verify that the RTC battery voltage falls within the standard range. If an RTC malfunction is detected, replace the RTC battery before proceeding with trigger inspection and repair.

**A** is the left test point of the RTC, **B** is the right test point of the RTC, **C** is the SIM card slot grounding housing. Both points must be satisfied:

1. Set the multimeter to the mV range and measure the voltage between points A and B. (The measured voltage must be less than **5mV**. If it fluctuates above 5mV at any moment, it is also deemed a failure.)
2. Set the multimeter to the V range and measure the voltage between points A or B and C. (**U ≥3.1V** is normal.)

**Visual:** photo of a mainboard / SIM-holder area with probes at A / B / C (labels printed on the page).

## Trigger Circuit Repair

Inspect each photo sequence left to right, top to bottom, and replace the relevant materials in order if there is a problem.

### One-way trigger (pages 4–5)

Photos labeled **zebra strips** and **LCD Mesh**.

1. Check whether the zebra strips are missing, deformed or dirty, and if so, please reinstall and replace the zebra strips.
2. Check whether the LCD mesh has good electrical continuity. Use a multimeter set to the ohms (Ω) range to measure the resistance between pins **2 and 5** (**R≤1kΩ** is normal). Then measure whether pins 2 and 5 are shorted to GND (multimeter display of **0L** is normal). If the LCD Mesh is damaged, replace it and verify. **(Note: The LCD Mesh is a one-time use component; it is damaged upon removal.)**
3. If the above checks are fine and the trigger still exists, please replace the mainboard for verification.

### Two-way trigger (pages 5–6)

Photos labeled **Mainboard LCD connector** and **screen LCD_FPC**. Overlay pins **34** and **31**.

1. Check to confirm that screen LCD_FPC is well connected to the LCD connector of the mainboard.
2. Check whether the LCD_FPC is dirty or damaged（whether the connection port is falsely soldered, and whether the pins are deformed, and measure resistance between **31 and 34** in the above figure（**R ≤30Ω** is normal）. If so, remove dirt or replace screen components for verification.
3. Check whether the motherboard LCD connector is dirty or damaged (whether the base is soldered falsely, whether the connector is deformed), if there is, please remove the dirt, re-solder, or replace the connector (if there is no operating condition, replace the motherboard for verification).
4. If the above checks are fine and the trigger still exists, please replace the mainboard for verification.

### Three-way trigger (page 6)

Photos labeled **zebra strips** and **LCD Mesh**.

1. Check whether the zebra strips are missing, deformed, or dirty, and if so, please reinstall or replace zebra strips.
2. Check whether the LCD mesh has good electrical continuity. Use a multimeter set to the ohms (Ω) range to measure the resistance between pins **1 and 4** (**R≤1kΩ** is normal). Then measure whether pins 1 and 4 are shorted to GND (multimeter display of **0L** is normal). If the LCD Mesh is damaged, replace it and verify. **(Note: The LCD Mesh is a one-time use component; it is damaged upon removal.)**
3. If the above checks are fine and the trigger still exists, please replace the mainboard for verification.

### Four-way trigger (page 6)

Photos labeled **Rear shell carbon particle**, **mainboard gold finger**, **SE_IC wall**.

1. Check whether rear shell carbon particles are missing or dirty, and if so, please replace or clean the rear shell carbon particles.
2. Check whether mainboard carbon particle gold finger is dirty, and if there is, please clean the mainboard carbon particle gold finger.
3. Check whether the surface of the SE_IC wall is damaged, and if so, please replace the SE_IC wall (if there are no operating conditions, replace the motherboard for verification).
4. If the above checks are fine and the trigger still exists, please replace the mainboard for verification.

### Five-way trigger (page 7)

Photos labeled **Rear shell carbon particle**, **magnetic head**, **magnetic head connector**, **mainboard gold finger**. Overlay pins **1** and **9**.

1. Check whether the carbon particles in the back shell are missing or dirty, and if so, please replace or clean the zebra strips.
2. Check whether the head FPC is connected to the connector, if the connection is not in place, reconnect the head FPC.
3. Check that the head FPC is cracked and damaged, and use a multimeter to measure the resistance between Figure **1 and 9** above (**R≤20 Ω** is normal), if the head is damaged, please replace the head for verification.
4. Check whether the head connector and the motherboard carbon particle gold finger are foreign objects, and whether the head connector is soldered; If there is, please clean the head connector and motherboard carbon gold finger, and replace the head connector (if there is no operating condition, replace the motherboard verification).
5. If the above checks are fine and the trigger still exists, please replace the mainboard for verification.
