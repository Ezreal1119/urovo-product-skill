# DT66 Service Manual

> Canonical original: `DT66/others/maintenance-service-manual_202609121520/DT66_Maintenance_Service_Manual_20241218.pdf` (bytes and filename unchanged).
> SHA-256: `9193360716aadd436fabe8df3b1d15bcf6fb3c91c41a713fae45447862d1fef7`
> Visual protocol: **14/14** PDF pages rendered and inspected.
> Filename date **20241218**. Body title **DT66 Service Manual**. Printed inner page numbers 1–12 after the cover/TOC.
> Interior header: UROVO / 优博讯 and the U mark.
> Source spellings **Antennae**, **Card pedestal board**, **light sense**, **POGOPIN** retained.
> Not a live spec. Lead hard specs from `DT66/specs/`.

---

## Cover (page 1)

Title only: **DT66 Service Manual**. No revision or author on the cover.

## Contents (page 2)

| Section | Printed page |
| --- | --- |
| 1. Product appearance | 1 |
| 2. Accessories | 1 |
| 3. Disassembly steps | 2 |
| 1、Back shell disassembly | 2 |
| 2、Card pedestal board disassembly | 3 |
| 3、Motherboard bracket disassembly | 3 |
| 4、Motherboard disassembly | 4 |
| 5、Rear camera bracket disassembly | 5 |
| 6、Scan head disassembly | 5 |
| 7、Antennae bracket disassembly | 6 |
| 8、SUB board disassembly | 7 |
| 4.Product parts | 8 |
| 5.Repair of common faults | 8 |

## 1. Product appearance (PDF page 3 / printed 1)

**Visual — two-view photo:**

- Front: black smartphone-class handheld, dark screen, slim bezel, no physical keypad.
- Rear: circular camera + flash; gold **pogo-pin** array; **urovo** wordmark on a rear bar; green LED near the bottom; yellow triangular sticker at the top; orange side key visible.

## 2. Accessories (same page)

| Name | Photos (visible evidence) |
| --- | --- |
| Power Adapter | Black USB wall wart, two-pin / EU-style plug in this photo |
| USB cable | Black USB-A to USB-C (or similar) cable |
| Battery | Black pack shown label-side and blank-side |

## 3. Disassembly steps

### 1、Back shell disassembly (PDF page 4 / printed 2)

First remove the back cover and battery, then remove the **6 socket head cap screws** at the bottom of the fuselage and the **4 socket head cap screws** at the top of the fuselage.

Gently break open the rear shell, separate the fingerprint module FPC and motherboard, and remove the rear shell **(pay attention to the MIC silicone sleeve in the back shell do not lose)**.

**Visual:** rear after battery-cover/battery removal; top and bottom screw groups; fingerprint FPC still attached while the rear shell is peeled; MIC silicone called out.

### 2、Card pedestal board disassembly (PDF page 5 / printed 3)

Firstly, remove the **4 screws** on the card pedestal board and **1 screw** on metal sheet of card pedestal board, remove metal sheet of card pedestal board.

Separate the capacitor FPC and the card pedestal board FPC, and remove the capacitor and card pedestal board respectively.

**Visual:** card-holder / SIM-TF board at the lower chassis; metal sheet; capacitor FPC separated.

### 3、Motherboard bracket disassembly (same page)

Remove the **8 screws** on the motherboard bracket, remove the bracket, and then remove the card pedestal board FPC.

**Visual:** mid-frame / motherboard bracket lifted; card-pedestal FPC freed.

### 4、Motherboard disassembly (PDF page 6 / printed 4)

Separate the Main FPC、LCD&TP FPC、front camera FPC、scanning head FPC、light sense FPC and coaxial line, and remove the motherboard.

**Visual:** mainboard in the chassis with those FPCs/coax still seated; then the board removed.

### 5、Rear camera bracket disassembly (PDF page 7 / printed 5)

Separate the rear camera FPC, first remove the rear camera, then remove the rear camera bracket.

**Visual:** rear-camera module and its bracket lifted.

### 6、Scan head disassembly (same page)

Remove the **3 screws** from the scanner head bracket, separate the earpiece FPC, and remove the scanner head.

Take out the front camera, remove **1 screw** on the light sense FPC metal sheet, and take out the light-sensitive FPC, then remove the earpiece FPC from the scan head holder. **(pay attention to the light sense silicone sleeve in the face shell do not lose)**

**Visual:** scan-head bracket screws; engine out; front camera and light-sense FPC removed.

### 7、Antennae bracket disassembly (PDF page 8 / printed 6)

Remove the **5 screws** on the antenna bracket, then remove the antenna bracket.

**Visual:** antenna bracket at the upper/rear area; five screws.

### 8、SUB board disassembly (PDF page 9 / printed 7)

Remove the **2 screws** on the SUB board, separate the SUB board from the coaxial line、main FPC, and remove the coaxial line、SUB board and waterproof ring.

**Visual:** SUB board at the bottom; coaxial and main FPC separated; waterproof ring called out.

## 4. Product parts (PDF pages 10–12 / printed 8–10)

Header: **DT66 Main maintenance parts**.

| Part name | Photos |
| --- | --- |
| Back shell | Rear housing |
| Face shell | Front housing / display assembly |
| Motherboard | Main PCB |
| Card pedestal board | SIM/TF card board |
| SUB board | Bottom I/O board |
| Scan head | Scan-engine module |
| Rear camera | Rear-camera module |
| Front camera | Front-camera module |
| Motherboard bracket | Mid-frame bracket |
| Antenna bracket | Antenna bracket |
| Rear camera bracket | Camera bracket |
| Capacitance | Capacitor / capacitance module |
| Earpiece FPC | Earpiece flex |
| Light sense FPC | Ambient / proximity flex |
| Card holder board FPC | Card-board flex |
| Metal sheet of card holder board | Small metal sheet |
| Coaxial line | RF coaxial |
| waterproof ring | Sealing ring |

Screws (source counts retained):

| Name | Printed count / use |
| --- | --- |
| Screw 1 | Card holder board screws *4, scan head screws *3, SUB board screws *2, Light-sensitive FPC screw *1 |
| Screw 2 | motherboard bracket screws *8, Antenna bracket screws *5 |
| Screw 3 | metal sheet of card pedestal board screw *1 |
| Screw 4 | Back shell top screws *4 |
| Screw 5 | Back shell bottom screws *4 |

## 5. Repair of common faults (PDF pages 13–14 / printed 11–12)

### 5.1 Battery charging relevant issues: no charging

① Check whether the battery, power adapter, and data cable are well connected.  
② Replace the power adapter data cable and battery access device that function normally and check whether it is charging normally.  
③ Check whether the USB port is damaged, and replace the USB port if it is damaged.  
④ None of the above problems exist, replace the SUB board or motherboard.

### 5.2 Equipment start-up relevant issues: No display on the screen or screen flashes but doesn't switch on

① Check if the battery is well connected and if the battery is dead, replace the battery with a normal one and check again.  
② Check whether the LCD_FPC is connected correctly, to confirm that there is no problem with the installation before testing.  
③ None of the above problems exist, replace the screen replacement.

### 5.3 NFC relevant issues: NFC test no sound

① Check if the NFC antenna is installed properly.  
② Check if the software is correct or if the NFC module is turned on.  
③ Check if there is sound from the speaker, if the speaker is damaged, please replace it and retest.

### 5.4 Display and touch relevant issues

① Check whether the LCD&TP_FPC is connected correctly.  
② None of the above problems exist, replace the face shell.

### 5.5 SIM relevant issues

① Check whether the SIM card is damaged, and test with another SIM card.  
② Check whether the card holder is properly welded, re-welding or replacement of the card holder.  
③ None of the above problems exist, replace the Card pedestal board.

### 5.6 TF card relevant issues

① Check if the SD card is damaged and cannot be read, change a TF card for testing.  
② Check whether the card holder is properly welded, re-welding or replacement of the card holder.  
③ None of the above problems exist, replace the Card pedestal board.

### 5.7 Camera relevant issues: splash screen or error reporting

① Check if the camera is installed or if the camera FPC is connected correctly.  
② None of the above problems exist, replace the camera.

### 5.8 OTG relevant issues: data not detected

① Please check whether the USB flash drive is normal, Test again after replacing the USB flash drive.  
② check whether the USB OTG cable is broken or not working, Test again replacing USB OTG cable with a good one.  
③ Check that the Type-C connector of the device is intact, replace the USB interface if damaged.  
④ All the above do not exist problems, replace the SUB board or motherboard.

### 5.9 Speaker relevant issues: no sound output

Please Check whether the FPC of the horn is damaged, and replace the horn if it is damaged.

### 5.10 Earpiece relevant issues: no sound or noise

① Check if the earpiece is in good contact with the earpiece FPC.  
② Check if the earpiece FPC is damaged, and replace it if it is damaged.  
③ All the above do not exist problems, replace the earpiece.

### 5.11 Fingerprint relevant issues: Fingerprint not recognized

① Check if the fingerprint module FPC is connected correctly.  
② Check if the fingerprint module FPC is damaged, and replace it if it is damaged.  
③ All the above do not exist problems, replace the fingerprint module.

### 5.12 Scan head relevant issues: scanning head does not produce light

① Check whether the scanning head is installed correctly.  
② Check whether the scanning head type is selected correctly, enter **\*#1261\*#** to see whether the scanning head type is correct.  
③ Replace the scanning head.

### 5.13 POGO PIN relevant issues

① Check if the POGOPIN wire is contacting properly.  
② Check if the device probe is installed properly.  
③ Replace the POGOPIN cable and test again.

### 5.14 Proximity sensor and light sensor relevant issues

① Check whether the light sense FPC is installed correctly or if it is missing.  
② Check if the light sense FPC is damaged, and replace it if it is damaged.
