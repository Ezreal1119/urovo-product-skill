# Heating App Instructions v1.2

**Source type:** Shared software-operation instruction.

**Paths:**

- Markdown: `_shared/operations/heating-app-instructions_202608281943/Instruction-on-how-to-use-Heating-App_v1.2.md`
- Original: `_shared/operations/heating-app-instructions_202608281943/Instruction-on-how-to-use-Heating-App_v1.2.doc`

## Scope

The source documents UROVO Heating App v1.2.0, revised 2026-08-17. It explains automatic and one-touch LCD/scanner heating, but does **not** name compatible device models. Use it only after separate product-specific evidence establishes that the target device includes the Heating App and relevant heating hardware.

## Key Behavior

- Auto Heating is event-based and does not continuously maintain a fixed temperature.
- Fast-rise default trigger: at/below 5°C, then +2°C within 15 seconds; one-minute heating session.
- Rapid-cooling default trigger: 5°C down to -3°C within 20 minutes; one minute of scanner-only heating.
- One-touch Heating can select LCD, scanner, or both for one to five minutes; scanner-only is the default channel selection.
- Global heating button replaces the circular in-app button with a floating control and requires `Display over other apps` permission.
- Documented overtemperature default: 35°C, selectable 10°C-35°C or 60°C.
- Low-power automatic-heating cutoff: default 10%, selectable 5%-15%.
- Includes a recommended starting point for approximately -20°C cold-store use.

## Visual and Internal-Value Note

All 10 rendered pages and six application screenshots were inspected. Figure 2-2 and Figure 2-3 visibly show an overtemperature value of 25°C, while the narrative states a factory default of 35°C. Treat 25°C as a displayed example/configured state and preserve 35°C as the documented default; do not silently conflate them.

## Product Hub Backlinks

No product model is named, so no Product Hub backlink is created. This prevents generic app behavior from being injected as proof of hardware compatibility.

## Query Guidance

Use the full companion for Auto Heating trigger logic, LCD/scanner channel behavior, One-touch Heating, protection limits, Global heating button troubleshooting, and cold-store setup. Always keep application logic separate from product compatibility.
