# Urovo Spec Comparison 241030

Dated internal competitive specification workbook covering multiple UROVO products and competitor families. It is a comparison source, not a live competitor-spec feed.

## Synchronized Source

- Original: `_shared/comparison/urovo-spec-comparison_202609102000/Urovo_spec_comparation_241030.xlsx`
- Markdown: `_shared/comparison/urovo-spec-comparison_202609102000/Urovo_spec_comparation_241030.md`
- SHA-256: `a3cbb03e6670762ba07af75fef5a9ba0b1291e0fe7608614a99e058200f01d40`
- Version log (`Updates`): v1.0 / 240924 Gawin Zhao (CT58S vs Zebra/Honeywell); v1.1 / 241025 add RFID overview; V1.1 / 241030 add iData/Newland/Chainway/Unitech/Emdoor RFID and tablets
- Package: 9 sheets; 2957 non-empty cells; 3 `DISPIMG` formulas; 143 merged ranges; 84 placed drawings; 87 media files (3 unused)
- Conversion coverage: every non-empty sheet name (including leading/trailing/double spaces), cell value, formula, and merged range; every drawing inspected and transcribed

This workbook is a different document identity from [[shared/urovo-pda-battlecard|Urovo PDA Battlecard 2025-12-05]] (Excel 2024-10-30 vs PPTX 2025-12-05). Do not treat one as a replacement for the other.

## Covered Product Hubs

- [[products/DT50S|DT50S]] and [[products/CT58S|CT58S]]
- [[products/DT66|DT66]]
- [[products/CT48|CT48]]
- [[products/RT40S|RT40S]]
- [[products/P8100-4G|P8100 4G]], [[products/P8100P-4G|P8100P 4G]], and [[products/P8100P-5G|P8100P 5G]] (P8100P 4G/5G share one column)
- [[products/DT50D|DT50D]]
- [[products/RFG91|RFG91]]

## Additional UROVO Models Present

The workbook also names DT40S, DT50U, DT51U, DT51D, and RFDT50, which do not currently have canonical Product Hubs. Preserve those source model strings. Do not fold DT40S into [[products/DT40|DT40]], DT50U into [[products/DT50P|DT50P]], or RFDT50 into RFG91.

Source spellings retained in the companion include `Zewland`, `Chianway`, `Camere`, and `Upgradebable` where they appear.

## Competitive Coverage

- DT50S / CT58S against Zebra TC52x/TC72/TC21, Honeywell EDA52/CT60/CT45/CT30 XP, Point Mobile PM90/PM86/PM75/PM84, Unitech EA630/EA520, Newland NLS-MT93, and iData T3 Pro.
- DT66 against Zebra TC22/TC5X/TC73/TC15, Honeywell CT47/EDA57, Point Mobile PM95, and Unitech EA660/PA768.
- CT48 / DT40S against Zebra MC2200/MC2700, Honeywell EDA51K/EDA61K/EDA40K, and Point Mobile PM67.
- RT40S against Zebra MC3300X/MC3300AX/MC9400/MC9300/MC2200, Honeywell CK65/EDA61K/CK67/CK62, and Point Mobile PM452/PM352/PM560.
- P8100 / P8100P against Zebra ET51/L10/ET40/ET80/ET60, Honeywell EDA10A/EDA71/RT10, and Emdoor EM-Q885M/EM-Q185M.
- Long-range UHF (DT50U/DT51U) against Zebra MC3300, Chainway C66 UHF back clip, and Unitech HT730UHF.
- Short-range UHF (DT50D/DT51D) against Bluebird HF550X/VX500 and Chainway C71/C66 built-in UHF.
- RFID sled (RFG91/RFDT50) against Zebra RFD40/RFD8500/RFD90, Bluebird RFR900/RFR901, Point Mobile RF88/RF750/RF900/RF300/RF851, Chainway C66, and Unitech RG768/RG630/RP200.

## Query Guidance

Use this source for dated sales positioning (cut-off 2024-10-30), competitor discovery, and identifying which UROVO fields require verification. Do not treat competitor values as current without a newer authoritative source. For UROVO hard specifications, lead with the product-specific `specs` source, retain valid option/region context, and surface the Hub discrepancies below. A blank cell means only that the workbook supplies no value.

## Active Source Discrepancies

Same-context UROVO differences versus current dedicated specs. Dated comparison values are not silently preferred.

| Product | Field | 241030 comparison value | Other current local value | Status |
| --- | --- | --- | --- | --- |
| DT50S | Android | Android 13 | Android 11 (Android 13 optional) in product specs | Unresolved dated difference; do not drop the optional-11 framing |
| CT58S | CPU | MT 6762, Octa-core 2.0 GHz | Octa-core 2.2 GHz in product specs | Unresolved |
| CT48 | CPU | Octa-core 2.0 GHz MT8768 | 2.2 GHz in product specs and brochure (also in the 2025-12-05 Battlecard as 2.0 GHz) | Unresolved; use product specs first |
| P8100 4G | Bluetooth | Bluetooth 4.2+BR/EDR+BLE | BT 5.0 + BR/EDR + BLE in product specs | Unresolved |
| P8100 4G | Drop | Can withstand the impact of multiple drops from a height of 1.5 meters onto a smooth concrete floor | Multiple 1.2 m drop to concrete at room temperature in product specs | Unresolved |
| P8100 4G | Sealing | IP54/67 | IP67 in product specs | Unresolved; comparison lists both classes |
| P8100P 5G | Bluetooth | BT5.0+BR/EDR+BLE (shared P8100P 4G/5G column) | BT 5.2 + BR/EDR + BLE in the 5G product spec; P8100P 4G spec is BT 5.0 | Unresolved for the 5G SKU |
| DT50D | CPU | MTK eight-core 2.0 GHz | Octa-core 2.45 GHz in product specs / brochure / internal mapping | Unresolved |
| DT50D | Battery | 可拆卸4300mAh | 3.85V, 5000 mAh in product specs / brochure / user-guide figure | Unresolved |
| DT50D | Android | Android 11 | Android 11.0 (Android 13.0 optional) in product specs | Unresolved dated difference |
| DT50D | Display | 5.5 inches | 5.7" in product specs / brochure | Unresolved |
| DT50D | Thickness | 162.8mmx76mm×15.6mm (21.9mm at the thickest point) | 162.8 × 76 × 13.6 mm (thickest: 21.9 mm) in product specs | Unresolved body-thickness figure; thickest-point 21.9 mm agrees |
| RFG91 | Standard battery | Smart battery 3.6V 5000mAh / 6700mAh (optional) | 4900 mAh / 18 Wh in product specs and accessory guide; 5000 mAh also appears in other current shared sources | Unresolved; optional 6700 mAh agrees |

DT50S tumble `400 1.0m tumbles` is additional coverage (dedicated spec is silent; the 2022-09-01 SQ53S reliability report PASS is the same 400 × 1000 mm protocol). Absence from the dedicated spec is not treated as a contradiction.
