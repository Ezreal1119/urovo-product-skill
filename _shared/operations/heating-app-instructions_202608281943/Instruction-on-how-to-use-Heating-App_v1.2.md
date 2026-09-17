# Instruction on How to Use Heating App

> **Canonical original:** `_shared/operations/heating-app-instructions_202608281943/Instruction-on-how-to-use-Heating-App_v1.2.doc`  
> **Current version:** v1.2.0  
> **Current revision date:** 2026-08-17  
> **Language:** English  
> **Scope:** The source does not name any compatible device model. Treat it as application-level operational guidance only; do not infer that a particular product supports LCD or scanner heating without separate product-specific evidence.  
> **Pages visually inspected:** 10 of 10 after read-only LibreOffice rendering

## Page 1 - Revision History

| Date | Author | Version | Description |
| --- | --- | --- | --- |
| 2024-08-09 | Zhou Jie | v1.1.11 | Heating App instruction documentation. |
| 2026-08-17 | - | v1.2.0 | Updated for the current Heating App: Auto Heating switch, LCD and scanner channels, corrected fast-rise and rapid-cooling scenarios, Global heating button, and default values. |

## Pages 2-3 - Introduction and Main Interface

Heating App provides two modes:

1. **Auto Heating**, including Advanced Settings.
2. **One-touch Heating**.

On the current interface:

- **Auto Heating** is the switch under the `Auto heating duration` section.
- **One-touch Heating** starts from the circular button, or from a floating button when **Global heating button** is enabled.
- The top of the interface shows the LCD temperature and `LCD Heating: On / Off`.
- It also shows the `ENVIR` environment/scanner temperature and `Scanner Heating: On / Off`.
- Auto Heating decisions use the **ENVIR/scanner temperature**, not the LCD temperature. The LCD value is mainly informational.

The screen in Figure 1-1/1-2 visibly contains:

- `LCD 34°C` and `ENVIR 32°C` sample readings.
- `LCD Heating: Off` and `Scanner Heating: Off` sample states.
- `One-touch Heating Config`.
- `Scan heating duration (min)` with sample value `1`.
- `Lcd heating duration (min)` with sample value `1`.
- Scanner Heating and Lcd Heating channel switches.
- `Auto heating duration`, Auto Heating, and Advanced Settings.
- `Save` and `Restore` buttons.
- A circular blue heating button; Figure 1-1 labels it `One key heating` and labels Advanced Settings as `Customized heating`.

> **Important behavior:** Auto Heating is event-based. When trigger conditions are met, the app runs a heating session for a configured duration and then stops. It is not a thermostat that maintains a fixed temperature such as -20°C. In a stable cold environment, use One-touch Heating when needed.

## Pages 3-4 - Auto Heating and Fast Temperature Rise

### Auto Heating Switch

Turn on Auto Heating and tap **Save** to start the background heating service.

- When Auto Heating is off, Advanced Settings are greyed out and cannot be edited, and automatic heating does not run.
- Default: **ON**.
- When enabled, the service starts again after device reboot.

### Advanced Settings

Tap **Advanced Settings** to expand environment-dependent heating parameters.

### Fast Temperature Rise Heating

This scenario covers movement from a low-temperature environment toward a warmer one, such as leaving a cold store. It uses the ENVIR/SCAN temperature.

1. When temperature is at or below **5°C** by default, the app records the lowest encountered temperature, checking about once per second. The selectable upper limit of the minimum temperature is **0°C to 10°C**.
2. If the current temperature becomes **2°C or more** above that lowest value and the change occurs **within 15 seconds**, the app starts a heating session. Default heating duration: **1 minute**.

Channel behavior depends on the switches:

- Factory default: Scanner Heating ON and LCD Heating OFF -> scanner only.
- LCD Heating ON and Global heating button OFF -> LCD only.
- Global heating button ON -> both LCD and scanner.

Figure 2-1 shows the fast-rise fields and defaults:

| Field | Visible value |
| --- | --- |
| Upper limit of the minimum temperature | 5 |
| Heating duration (min) | 1 |
| Temperature interval (s) | 15 |

The screenshot also shows sample top readings of `LCD 34°C`, `ENVIR 33°C`, and both heating states Off.

## Pages 5-6 - Rapid Cooling and Channel Matrix

### Rapid Cooling Heating

This scenario covers movement from a warmer environment into a low-temperature environment, such as entering a cold store.

1. Record the time when temperature first reaches **5°C or below**; this is the default `monitor the maximum temperature at the beginning` value.
2. Record the time when temperature first reaches **-3°C or below**; this is the default `minimum temperature at the end of the test` value.
3. If the two events occur within **20 minutes**, activate **scanner heating only** for **1 minute** by default. LCD is not heated by this logic.
4. The rapid-cooling trigger is then disabled until temperature rises above the start value, default 5°C, after which it can trigger again.

Figure 2-2 visibly shows:

| Field | Visible value |
| --- | --- |
| Monitor the maximum temperature at the beginning | 5 |
| Minimum temperature at the end of the test | -3 |
| Temperature drop interval (min) | 20 |
| Overtemperature protection (°C) | 25 in this screenshot |

### LCD vs. Scanner Behavior

| Scenario | Scanner | LCD |
| --- | --- | --- |
| Entering a cold store - rapid cooling | Can heat automatically | Not heated by this logic |
| Leaving a cold store - fast temperature rise | Can heat automatically when Scanner Heating is on | Can heat automatically when LCD Heating or Global heating button is on |
| One-touch Heating - manual | Yes, when Scanner Heating is on | Yes, when LCD Heating is on |

## Pages 6-8 - Protection, Saving, and One-Touch Heating

### Overtemperature Protection

- Documented default: **35°C**.
- Selectable values: **10°C to 35°C**, or **60°C**.
- Heating is forced to stop when detected temperature exceeds the configured value.
- The same limit applies to LCD and scanner.

> Figure 2-2 and Figure 2-3 visibly show `Overtemperature protection (°C) 25`, while the narrative states the default is 35°C. Preserve the screenshot as an example/configured state; do not reinterpret it as the documented default.

### Low Power Stop Heating

- Defines the battery level below which **automatic** heating will not start.
- Range: **5% to 15%**.
- Default: **10%**.
- Manual One-touch Heating is not blocked by this setting in the app itself, although firmware may still limit heating at low battery.

Figure 2-4 shows `Low power stop heating (%) 10` as the visible value.

### Save and Restore

- Tap **Save** after modifying parameters.
- **Restore** returns parameters to their initial factory values.
- Tap **Save** again after Restore if Auto Heating should use the restored values.

### One-Touch Heating

Intended for emergency use when the screen and/or scanner are heavily fogged.

- Tap the circular One-touch Heating button to start.
- Select LCD, scanner, or both.
- Default: scanner only - LCD Heating OFF, Scanner Heating ON.
- Duration per session: **1 to 5 minutes**.
- If a selected channel is already heating, wait for it to finish before starting another session.

## Pages 8-9 - Global Heating Button and Stop Events

### Global Heating Button

When **Global heating button** is enabled and saved:

- The circular main-screen button is hidden.
- A floating button appears and starts the same One-touch Heating operation.
- The application requires the Android permission **Display over other apps**.
- If the floating button is absent, verify that permission.

Figure 3-1 shows the default channel state: Scanner Heating ON, LCD Heating OFF. It also shows sample `LCD 33°C` and `ENVIR 34°C` readings, both active heating-status labels Off, one-minute scan/LCD durations, Auto Heating ON, and the blue floating heating button.

### Heating Stop Events

1. Automatic heating is prohibited below the Low power stop heating threshold: default 10%, selectable 5%-15%.
2. When the device enters sleep, ongoing heating stops after the current heating cycle ends; the source labels this device/firmware behavior.
3. If battery removal is detected, ongoing heating stops; the source labels this device/firmware behavior.
4. Heating is prohibited above the Overtemperature protection value. The documented default is 35°C, configurable in Advanced Settings; it is not a fixed 40°C.

## Page 10 - Suggested Starting Point for About -20°C Cold-Store Use

These are recommendations to adjust as needed and then save:

- Auto Heating: ON.
- Scanner Heating: ON.
- LCD Heating: ON, so One-touch Heating and fast-rise automatic heating can heat the LCD.
- One-touch duration: 3-5 minutes for LCD and scanner.
- Rapid-cooling end temperature: approximately -15°C to -20°C.
- Rapid-cooling heating duration: 2-5 minutes.
- Overtemperature protection: keep 35°C.
- Low power stop heating: 10%-15%.

Entering a cold store can trigger scanner automatic heating once through rapid cooling. Heating does not remain continuously active while the device stays near -20°C. If the LCD becomes slow or dark, use One-touch Heating. Charge the battery before entering because low temperature reduces capacity and heating consumes additional power.

## Contact Information

- Shenzhen Urovo Technology Co., Ltd.
- Address: Fl. 36, United Headquarters Bldg., High-tech Zone, No. 63, Xuefu Rd., Nanshan Dist., Shenzhen, Guangdong, China
- Tel: (86) 755 8618 6300
- Fax: (86) 755 8618 6290
- Website: `www.urovo.com`
