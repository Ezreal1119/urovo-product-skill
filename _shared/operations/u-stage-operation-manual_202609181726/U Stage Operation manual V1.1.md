# U Stage User Manual V1.1

> Canonical original: `_shared/operations/u-stage-operation-manual_202609181726/U Stage Operation manual V1.1.pdf` (bytes and filename unchanged; space in `U Stage` retained).
> SHA-256: `c51d9a469eb6d4c21f521519ba9def011b5c2d39e1028d3bd1b9fea18e5b3222`
> Cover title **U Stage User Manual**, Version **V1.1**, **Urovo Technology Co., Ltd.**, **December 10, 2025**.
> PDF: WPS 文字; created/modified **2025-12-11 17:56:58 +08**; author 艾福杰尼背后的叔叔. **17** pages.
> Revision (printed page 1): V1.1 / 2025/12/10 / A / Yi Yang / APK `u-stage_1.4.8.20251208_1447_urovo_release.apk`.
> Platform-wide UEE staging tool. Operation is “subject to the functions of the customer's handheld device.” Not a live hardware spec. Do not treat screenshot device names as catalog coverage.
> Visual protocol: **17/17** pages rendered and inspected.

---

## PDF page 1 — Cover (printed unnumbered)

**UROVO** wordmark top right. App icon: cyan rounded square, white gear with circular arrows. Title **U Stage** / **User Manual** / Version: V1.1. Footer **Urovo Technology Co., Ltd.** / **December 10, 2025**.

---

## PDF page 2 — Statement (printed 1)

**UROVO** wordmark top right.

The rights of ownership and interpretation of this document belong to Urovo Technology Co., Ltd. Without written permission of Urovo Technology Co., Ltd., it shall not be copied, or disclosed and sold to a third party, otherwise, legal liability will be investigated according to law.

This document is the operation description of the functions of U Stage. The specific operation is subject to the functions of the customer's handheld device. Please read the user manual carefully before using it and standardize the operation.

| Version | Date | AMD | Revised by | Description |
| --- | --- | --- | --- | --- |
| V1.1 | 2025/12/10 | A | Yi Yang | u-stage_1.4.8.20251208_1447_urovo_release.apk |

(A-Add, M-Modify, D-Delete)

---

## PDF page 3 — Table of contents (printed 2)

Table of contents (source spelling **fle** in 3.7 retained as printed):

- Statement … 1
- 1. Function Description of U Stage … 3
  - 1.1 Configure … 3
  - 1.2 Export … 4
  - 1.3 Import … 4
- 2. Quick operation guide … 5
  - 2.1 Configure Settings and Export Configuration … 5
  - 2.2 Scheme 1: Upload to UMS … 5
  - 2.3 Scheme 2: Generate barcode … 8
  - 2.4 Scheme 3: Export to local … 11
- 3. Range of Settings for Synchronization … 12
  - 3.1 Scanner config … 12
  - 3.2 ScanWedge config … 13
  - 3.3 System settings … 13
  - 3.4 Special system settings … 14
  - 3.5 Keymap config … 15
  - 3.6 Enterprise Desktop config … 15
  - 3.7 SMB/FTP/HTTP fle download … 15
  - 3.8 RFID Config … 16
  - 3.9 UBrowser Config … 16

---

## PDF page 4 — Function description and Configure (printed 3)

**1. Function Description of U Stage**

U Stage provides enterprise IT administrators and agents with rapid device configuration synchronization capabilities. After the first device is configured according to enterprise requirements, subsequent devices can be synchronized in a simplified manner, enabling large quantities of devices to achieve the required operational state efficiently. This facilitates centralized enterprise management and reduces configuration errors caused by manual operations.

**Flow diagram (not in the text layer as a tree):** navy box **U Stage** branches to red **Configure**; orange **Export** → Upload to UMS / Generate barcode / Export to local; yellow **Import** → Scanner Qrcode Import / Camera Qrcode Import / Local File Import.

**1.1 Configure**

Before using this program, the current prototype must be configured to its required working state. The configuration scope includes system-level, scanner-related, and extended functional modules supported by U Stage, covering:

- Scanner config
- ScanWedge config
- System settings
- Special system settings
- Keymap config
- Enterprise Desktop config
- SMB/FTP/HTTP file download
- RFID Config
- UBrowser Config

---

## PDF page 5 — Export and Import (printed 4)

After completing all required configuration items, you may proceed to launch the U Stage program.

**1.2 Export** — three transmission modes:

1. **Upload to UMS** — If the device has been bound to the UMS, click to upload the current configuration directly to the UMS Configure Management page. The configuration can then be deployed in batches through silent import on the UMS backend.
2. **Generate barcode (QR code)** — Convert the configuration into a QR code. Other devices can scan the QR code to import the configuration quickly and conveniently.
3. **Export to local** — Export the configuration to sdcard/ storage to generate two files:
   - `ustage_00000000.pdf` — QR code representing the configuration; transfer or print for users to scan.
   - `ustage_00000000.txt` — can be uploaded to the MDM platform for remote silent deployment.

**1.3 Import**

1. **Scanner QR Code Import** — device scanner.
2. **Camera QR Code Import** — device camera.
3. **Local File Import** — select a stored configuration file.

---

## PDF page 6 — Quick operation guide / Scheme 1 start (printed 5)

**2. Quick operation guide**

**2.1 Configure Settings and Export Configuration**

- Step1: Prepare: Open U Stage.
- Step2: Set Up: Configure all required settings on one prototype device.
- Step3: Export (Three Methods): Upload to UMS; Generate Barcode (QR code image); Export to Local (QR image + TXT in the U Stage directory).
- Step4: Import: Receiving it from UMS; Scanning the QR code image; Loading the local TXT file.

**2.2 Scheme 1: Upload to UMS**

Step1: Click “Export”, and then select “Upload to UMS”. Upload the configuration to the UMS account corresponding to the device. You can select to upload the scanner configuration and system configuration to the UMS. You can customize remarks. If the remarks field is not displayed and the configuration is uploaded to the same device for multiple times, only one rule is displayed in the background to overwrite the previous files; That is, duplicate names are overwritten and different names are created based on the configured name.

---

## PDF page 7 — Upload-to-UMS screenshots (printed 6)

Three phone screens + one UMS web screenshot.

**Choose export function** (status 4:59):  
1.Upload to UMS — use UMS/UTMS for batch remote silent deployment.  
2.Generate barcode — other devices can scan the barcode to import.  
3.Export to local — export the configuration QR code as PDF and the file is on sdcard /Ustage.  
Buttons: **Upload to UMS** (grey, red box), **Generate barcode**, **Export to local**.

**Upload to UMS:** large cyan check; red box **Upload successfully config name is ustage_20250807530001**; **OK** / **Upload again**.

**Configuration import details:** header `ustage_20250807530001` / “configuration is imported, and the import details are as follows”. Rows all **success**: Configuration data parsing; Import : Scan config; Import : Advanced Scan config; Import : System settings; Import : Keymap config. **OK**.

**UMS Configure Management** (desktop): sidebar UMS / Dashboard / App Store / Group Management / Remote Management / **Stage Management** (Configure Management selected) / Data Center / Device Manager / System Customization / Account Center / Sub-account. Orange banner begins **Upload config, use ustage on the terminal** (export the configuration file; terminal upload generates a publishable rule). Table sample **Configuration Name** `ustage_20250807530001`, Configuration Type Scanner config, Version Number 1, Push Range GROUP (truncated), Status Published, **Execution Progress 10/10**, Create Time 2025-12-05 11:32:54, Update Time 2025-12-05 11:42:17, SN `20250807530001`. Footer Total 1 item. Export-path hint in the app: `sdcard /Ustage`.

Note: If the configuration fails to upload to UMS successfully, the following error message will be displayed: *(error UI is on the next page)*

---

## PDF page 8 — Upload errors and UMS release (printed 7)

**Choose export function** with black toast **Device does not have UMS installed** over Generate barcode.

**Upload to UMS** error: orange exclamation; **Failed to upload, please try againexport error** (source concatenation); **OK** / **Upload again**.

Body: (1) No UMS account is bound to the device. (2) The device is not connected to Wi-Fi.

Note: If the scanner configuration and system configuration are not enabled, the following prompt will appear: three cyan buttons Upload to UMS / Generate barcode / Export to local, with toast **Select at least one item**.

**Step2:** Configuration can be imported silently into all devices through remote deployment on the UMS – Configure Management page. Select the desired rule and click Release. Based on your requirements, you may choose either group release or SN release. Devices within the selected device group will execute the configuration rule once they receive the command. After the configuration is delivered, the number of completed executions will gradually increase. The progress is displayed in the format: Number of successfully executed devices / Total number of devices in the target group. When all devices have completed the configuration, the number of successfully executed devices will match the total number of devices shown in the progress bar.

---

## PDF page 9 — UMS progress callout + Generate barcode start (printed 8)

UMS table again; red box around **Execution Progress 0/1**. Same rule name `ustage_20250807530001`.

**2.3 Scheme 2: Generate barcode**

Step1: Click “Export”, and then select “Generate Barcode”.

**U Stage home:** 1. Import — Long press the scanner key to synchronize the configuration. 2. Export — Please configure the device to working state before exporting the configuration. **Export** boxed; overlay **Choose export function** with **Generate barcode** boxed.

---

## PDF page 10 — Generate barcode steps (printed 9)

**Step1** boxed on Generate barcode. **Step2** overlay lists toggles: Scanner config On, ScanWedge config On, System settings On, Special system settings Off, Keymap config On, Enterprise Desktop config Off, SMB/FTP/HTTP file down… ; Cancel / **OK**. **Step3 Confirm your settings:** Scan config **Confirmed**; ScanWedge config / System settings / Keymap config **Not confirmed**.

Step3 text: After finalizing the configuration items, generate the corresponding barcode. When synchronizing more than one configuration, swipe left or right to switch between QR codes for different configurations.

**Configure barcode** screen **Page1/4**: QR code; Config name:`scanner_00952546000379`; Config type Scanner config; page dots.

Step4: Open U Stage on other devices. After clicking "Import", you can import the configuration using one of the following methods:

---

## PDF page 11 — Import methods (printed 10)

- **Scanner Qrcode Import** — scanner activates (or physical scanner key). Scan the QR code. The device will execute the configuration and reboot automatically to complete deployment.
- **Camera Qrcode Import** — for devices without a scanner, use the camera. Same reboot behavior.

Screenshots: U Stage **Import** boxed; **Choose the import method** — 1. Import via URL (Through the url, you can download and import the configuration, download the zip to the specified location, download the specified installation package and install it on the device.) 2. Import by scanning code 3. Import via file. Buttons **Scanner Qrcode Import** / **Camera Qrcode Import** boxed; Local File Import. **Configuration import details** success: Configuration data parsing success; Import : Scan config success. OK / Retry on failure.

Display when scanning succeeded. Note: If the QR code is not a configuration file, **Configuration import details** shows row **Configuration data parsing** status **failed** (red box). **OK** / **Retry on failure**.

---

## PDF page 12 — Export to local (printed 11)

**2.4 Scheme 3: Export to local**

Step1: Click “Export”, then “Export to local”. PDF contains the QR code for print/scan. TXT can be uploaded to the UMS platform to update the corresponding rule. Export directory **`/sdcard/UStage`**.

Four-phone strip: Step1 Export to local boxed; Step2 toggles (Scanner / ScanWedge / System on; Special off; Keymap on; Enterprise Desktop off; SMB/FTP/HTTP file download; Notes “Enter notes to create a n…”); Step3 check **Saved to sdcard/UStage successfully config name is ustage_00952546000379**; file manager **UStage** with Images / Audio / Videos, folders **logs** / **profile**, files `ustage_0…`.

Step2: Import from Local Storage. Tap Import and select “Local File Import.” Navigate to the U Stage directory and select the required configuration file in **TXT** format.

---

## PDF page 13 — Local import screenshots + settings list start (printed 12)

Local import: **Import** / **Local File Import** boxed. File manager path **DT630 > UStage** (screenshot device label only; this is not a DT630-only manual). Highlighted file `rfid_0095…` under **profile**. Import details: Scan config success; Advanced Scan config success; Keymap config success; RFID Config success; System Setting wrapping **Importin g**; WiFi Connection Status wrapping **Connect ing**. U Stage home footer **Ver USDK:19.0.99.20251104** / **Ver Ustage:1.4.8.20251208**.

**3. Range of Settings for Synchronization** (same nine categories as §1.1).

**3.1 Scanner config** items 1–11: On-screen button; Enable Scanner Input; Scanner Selection; Display Overlay Window; Triggering Modes; Basic Multibarcode Config; Output Mode; Reader Parameters; UDI Data Formatting; Advanced Data Formatting; Basic Data Formatting.

---

## PDF page 14 — Scanner 12–18, ScanWedge, System 1–12 (printed 13)

**3.1 continued:** 12. Symbology Settings 13. OCR Scan 14. Special Settings 15. Import Profile 16. Export Profile 17. Reset Profile Configuration 18. Scanner Engine working normal

**3.2 ScanWedge config** 1–18: same as scanner 1–14 then 15. Reset Configuration 16. Import Profile 17. Export Profile 18. Reset Profile Configuration

**3.3 System settings** 1–12: Set time automatically; Automatic time zone; Time zone; Set ntp server; Time format; Brightness level; Adaptive brightness; Notifications on lock screen; Notification dot on app icon; Blink light; Auto-rotate screen; Battery percentage

---

## PDF page 15 — System 13–44, Special 1–9 (printed 14)

**3.3 continued:** 13. Font size 14. Display size 15. Screen timeout 16. Night Light 17. Dark Theme 18. On-screen keyboard 19. Languages 20. Media volume 21. Call volume 22. Alarm volume 23. Ring&Notification volume 24. Touch notification sound 25. Vibration 26. Vibrate for calls 27. Bluetooth On/Off 28. WLAN On/Off 29. WLAN continuous scanning 30. WLAN Detail 31. WLAN bands 32. WLAN Power Save 33. Hotpot 34. Location mode 35. Airplane mode 36. APN Settings 37. USB debugging 38. NFC 39. Home app 40. Browser app 41. Spell checker 42. Scan apps with Play Protect 43. Hold home for Assistant 44. Default Print Service

**3.4 Special system settings** 1–9: Enable featured device settings; Clear all third-party applications; Remove all saved wifi; Remove All Paired; Set the Kiosk mode; Set the time and date; Disable camera; Disable the status bar; Hide the bottom navigation bar

---

## PDF page 16 — Special 10–36, Keymap, Enterprise Desktop, FTP (printed 15)

**3.4 continued:** 10. Disable the left virtual key 11. Disable HOME key 12. Disable the right virtual key 13. Disable Wifi 14. Disable Bluetooth 15. Disable GPS 16. Disable screenshots 17. Disable emergency call 18. Disable sdcard 19. Disable button 20. Enable button 21. Disable notification display 22. Disable settings notifications 23. Disable app notifications 24. Enable app notifications 25. Set boot startup 26. Scan key value passed to application 27. The input method pops up automatically when scanning the code 28. Automatic phone recording 29. Three-finger screenshot 30. Screen stop 31. On-screen keyboard 32. OTG mode 33. USB tethering 34. Bluetooth tethering (text layer `Bluetooh tethering`) 35. Ethernet sharing 36. Lock screen mode

Visible §3.7 heading on this page: **SMB/FTP/HTTP fle download**.

**3.5 Keymap config:** 1. Enable intercept key 2. Key Remap 3. Show key remapping list 4. Wakeup

**3.6 Enterprise Desktop config:** 1. Choose config file

**3.7 SMB/FTP/HTTP file download:** 1. FTP file download *(heading on TOC/page 3 prints `fle`)*

---

## PDF page 17 — SMB/HTTP, RFID, UBrowser (printed 16)

2. SMB file download  
3. HTTP file download

**3.8 RFID Config:** 1. RfidWedge 2. Power Enable Control 3. Default Config 4. Associated application 5. Beep 6. Scan Mode 7. Key Trigger 8. Data Sources 9. Output Mode 10. Filter 11. Label Format 12. Trigger Mode 13. Scan Power

**3.9 UBrowser Config:** 1. Settings in the app

---

*Source: `_shared/operations/u-stage-operation-manual_202609181726/U Stage Operation manual V1.1.pdf`. 17/17 pages. Publisher on cover: Urovo Technology Co., Ltd.*
