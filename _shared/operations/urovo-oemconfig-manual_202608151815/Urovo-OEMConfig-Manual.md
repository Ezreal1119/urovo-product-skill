# Urovo OEMConfig User Manual

> **Canonical original:** `_shared/operations/urovo-oemconfig-manual_202608151815/Urovo-OEMConfig-Manual.pdf`
> **Language:** English
> **Version:** Urovo OEMConfig 1.0, User Manual — Release 1, Revision 0, 2023-03-17 (first release)
> **Scope:** Platform-wide operational manual for the UrovoOEMConfig application across UROVO Android devices.

## Revision History

| Release | Revision | Date | Changes |
| --- | --- | --- | --- |
| 1 | 0 | 2023/03/17 | First release |

## About this Manual

Many device manufacturers (OEMs) support custom, OEM-specific management policies. OEMConfig is a standard that enterprise mobility management (EMM) providers and OEMs follow to make these policies available to IT admins. This manual discusses the features of Urovo OEMConfig and how to use it with an EMM to configure Urovo-specific management policies.

## 1 — Introduction

The firmware of Urovo devices supports custom, OEM-specific management policies (or configurations). OEMConfig opens those OEM-specific configurations to the EMM software solution (for example, SOTI MobiControl), so IT admins can manage and monitor devices with a variety of EMMs while still configuring Urovo-specific settings.

The OEMConfig application uses "managed configurations" on Google Play Store. Because those managed configurations are visible to EMM solutions, EMMs can show the available Urovo-specific settings to IT admins and let them change the configurations.

OEMConfig can be extended to any application that follows the standard (e.g., Google's Chrome browser exposes some configurations via OEMConfig). The UrovoOEMConfig application opens Urovo-specific firmware settings to EMM solutions.

The Urovo-specific configurations exposed via the OEMConfig v1.0 interface include:

- Common Android settings (WiFi, Date & Time, Display, NFC, Language, IME)
- Urovo device-capability settings
- Urovo ScanService configurations
- Urovo application configurations (KeyRemap, Scanner, Wireless General, Update, WlanAdvanced)
- Update the OS via a local OTA file

## 2 — Feature Highlights

### 2.1 Features

The settings configurable by OEMConfig 1.0 are shown embedded inside the EMM solution. When the user submits changes, the configurations are sent to the Urovo device for processing.

| Setting group | Items |
| --- | --- |
| Clock | Time Mode, Manual Date, Manual Time, Time Zone Mode, Manual Time Zone, Time Format |
| Display | Display Timeout, Stay Awake, Font Size, Backlight Level, Auto Brightness, Auto Rotate |
| NFC | NFC On/Off |
| FOTA | Update OS via Local File |
| General UI | System Language, IME (set current keyboard) |
| KeyRemap | Enable/Disable KeyRemap, Import Settings, Export Settings, Reset Settings, Add a key remap setting |
| Power | Reboot, Reset (factory), ShutDown |
| Wireless General | Location Mode |
| WLAN | Set Profile, Remove Profile, Remove All Profiles |
| WlanAdvanced | PowerSaveMode, SignalTrigger (roaming threshold 50–80), SignalDelta (roaming value 0–10), SignalScanPeriod (0–60000 ms) |
| Scanner | Import settings, Export settings |
| Device Management | Device Capability: Camera, GPS, WIFI, Bluetooth, ADB, USB, StatusBar, Left/Right Virtual Key, Home Key |

## 3 — How to Use OEMConfig

### 3.1 Overview

To create a managed configuration for Urovo OEMConfig with your preferred EMM, first refer to your EMM's user manual. The procedure to open the Managed Configuration page differs across EMMs, but the configuration page itself looks the same.

To create a Managed Configuration: (1) find how to create one with your EMM (consult your EMM provider); (2) specify the Configuration Name; (3) make the necessary changes to the configuration groups, actions, and items; (4) click Save to send the configuration to the device.

Terminology:

- **Configuration Name** — the name of the Managed Configuration you are creating.
- **Configuration Group** — a group of similarly themed settings (e.g., the "Clock" group contains settings for Date, Time, Timezone).
- **Configuration Action** — each group begins with an Action setting that tells OEMConfig what to do with that group of settings. Different groups may have different actions, but the "None" action is always available (leave the settings alone).
- **Configuration Items** — the related settings under each group. You fill in some or all items depending on the chosen action and other items.

Example (KeyRemap group): Action `None`/`Reset` requires no items; `Enable/Disable` requires Programmable Keys; `Import/Export` requires File Path.

### 3.2 Clock

- **Action "None"** — no items.
- **Action "Configure"** — all Clock items used.

Configuration items:

- **Time Mode** — Auto (NTP sync) or Manual (requires Manual Date/Time).
- **Manual Date** — format `dd/MM/yyyy`; ignored if Time Mode is Auto.
- **Manual Time** — format `HH:mm`; ignored if Time Mode is Auto.
- **Time Zone Mode** — Auto (cellular/location) or Manual (requires Manual Time Zone).
- **Manual Time Zone** — Olson time-zone ID, e.g., `Asia/Shanghai` (see https://en.wikipedia.org/wiki/List_of_tz_database_time_zones).
- **Time Format** — 12 or 24 hour.

### 3.3 Display

- **Action "None"** — no items.
- **Action "Configure"** — all Display items used.

Configuration items:

- **Display Timeout** — choose from a list.
- **Stay Awake** — toggle on/off (a developer-option setting).
- **Display Font Size** — set the system font size.
- **Backlight Level** — set the display brightness level.
- **Auto Brightness** — toggle on/off.
- **Auto Rotate** — toggle on/off.

### 3.4 NFC

- **Action "None"** — no items.
- **Action "Configure"** — all NFC items used.

Configuration item:

- **NFC Adapter** — turn on or off NFC.

### 3.5 FOTA

- **Action "None"** — no items.
- **Action "Configure"** — all FOTA items used.

Configuration item:

- **Fota OS Update File Path** — update the device OS via the specified OTA ZIP file path. The OTA ZIP file must be downloaded to the device before executing this configuration.

### 3.6 General UI

- **Action "None"** — no items.
- **Action "Configure"** — all General UI items used.

Configuration items:

- **System Language** — enter a language ID like `en_US`, `zh_CN` (see https://www.science.co.il/language/Locale-codes.php).
- **IME Current Keyboard** — enter the package name of the IME to set as current keyboard, e.g., `com.sohu.inputmethod.sogou/.SogouIME`.

### 3.7 KeyRemap

- **Action "None"** — no items.
- **Action "Reset"** — reset KeyRemap settings to factory default.
- **Action "Enable/Disable"** — enable/disable KeyRemap globally; requires Programmable Keys.
- **Action "Import/Export"** — import settings from a file or export settings to a file; requires File Path.

Configuration items:

- **File Path** — path to the setting file.
- **Programmable Keys** — add one or more keys via "Add Group". For each key:
  - **KeyName** — the key to re-program (a supported programmable key; differs by model). Examples: EA630 — `VOLUME_UP`, `VOLUME_DOWN`, `BARCODE_SCAN_1`, `BARCODE_SCAN_2`, `FUNCTION_2`; PA760 — Volume Up, Volume Down, Scan Left, Scan Right, Function Key.
  - **Key Code** — remap to another keycode or Start an activity.
  - **Remap to Key** — Android key code (see Appendix 1). Examples: keycode `3` = HOME, `4` = BACK, `187` = APP_SWITCH.
  - **Remap to App** — package name of the app to launch.
  - **WakeUp screen** — toggle to wake the screen when the key is pressed.
  - **Broadcast KeyDown Action** — optional; broadcast an action on KeyDown (e.g., `VolumeUp.Down`).
  - **Broadcast KeyDown Extras** — optional; Key-Value JSON, e.g., `[{"Key":"Name","Value":"Urovo"}]`.
  - **Broadcast KeyUp Action** — optional; broadcast an action on KeyUp (e.g., `VolumeUp.Up`).
  - **Broadcast KeyUp Extras** — optional; Key-Value JSON, e.g., `[{"Key":"City","Value":"Shenzhen"}]`.
  - **Start Activity Extras** — optional extra data to launch the app with, Key-Value JSON, e.g., `[{"Key":"mode","Value":"default"}]`.

### 3.8 Power

- **Action "None"** — no items.
- **Action "Reboot"** — reboot the device.
- **Action "Reset"** — factory reset the device (use with caution).
- **Action "Shutdown"** — shut down the device.

### 3.9 Wireless General

- **Action "None"** — no items.
- **Action "Configure"** — all items used.

Configuration item:

- **Location Mode** — turn on or off GPS location.

### 3.10 WLAN

- **Action "None"** — no items.
- **Action "Set Profile"** — create or set a WiFi profile; mandatory items: SSID, Password, Security Mode, IP Assignment, Proxy Mode. If IP Assignment is Static IP, the Static IP items (Address, Prefix Length, Gateway, DNS1, DNS2) are also mandatory. If Proxy Mode is PAC or Static, the Proxy PAC/Static items are mandatory.
- **Action "Remove Profile"** — remove the profile named in SSID; mandatory: SSID.
- **Action "Remove All Profiles"** — remove all WiFi profiles.

Configuration items:

- **SSID** — mandatory for Set Profile / Remove Profile.
- **Password** — mandatory for Set Profile.
- **Security Mode** — authentication method for the WiFi network.
- **IP Assignment** — DHCP or Static IP.
- **Static IP – Address / Prefix Length / Gateway / DNS Server 1 / DNS Server 2** — mandatory when IP Assignment is Static IP (prefix length e.g., `32`).
- **Proxy Mode** — None / PAC / Static.
- **Proxy PAC – PAC File URL** — mandatory when Proxy Mode is PAC.
- **Proxy Static – Host URL / Port / Exclusive List** — mandatory when Proxy Mode is Static.

### 3.11 WlanAdvanced

- **Action "None"** — no items.
- **Action "WlanAdvanced PowerSaveMode"** — configure; all items used.

Configuration items:

- **Power save Mode** — switch power-saving mode.
- **RoamingThreshold** — set roaming threshold (50–80).
- **RoamingDifference** — set roaming value (0–10).
- **RoamingScanPeriod** — set roaming scan period (0 ms ~ 60000 ms).

### 3.12 Scanner

- **Action "None"** — no items.
- **Action "Import"** — import Scanner settings from a setting file (must already be uploaded to the device); requires Scanner Settings Folder Path.
- **Action "Export"** — export scanner settings to a file; requires Scanner Settings Folder Path.

Configuration item:

- **Scanner Settings Folder Path** — the folder where setting files are exported to or imported from.

### 3.13 Device Management

The Device Management group enables or disables device capabilities in the firmware. Different device models may support different sets of Device Capability (see Appendix 2).

There are no actions in this group. To enable or disable a capability, add one or more "Device Management" configuration items via "Add Group". For each item:

- **Device Capability Enabled** — toggle on/off the specified capability.
- **Device Capability Item** — specify which capability to toggle (Camera, GPS, WIFI, Bluetooth, ADB, USB, StatusBar, Left/Right Virtual Key, Home Key).

## Appendix

- **Appendix 1** — Android key codes (keycode `3` = HOME, `4` = BACK, `187` = APP_SWITCH, etc.).
- **Appendix 2** — Device Capability list per model.

---

Urovo Headquarter
Email: info@urovo.com
Tel: +86 400-888-6969
Website: http://www.urovo.com
Address: 37F, 36F, United Headquarters Building, High-tech Zone, No. 63, Xuefu Road, Yuehai Street, Nanshan District, Shenzhen, Guangdong Province, the People's Republic of China
