# PDA Platform, Memory, and Android Summary

User-authored multi-product configuration matrix mapping market models to internal device projects, chipset/platform identifiers, memory configurations, and Android versions.

## Synchronized Source

- Canonical Markdown: `_shared/specs/pda-info-summary_202608111748/pda-info-summary.md`
- Source form: user-authored canonical Markdown; explicitly confirmed by the user during the 2026-08-11 sync
- SHA-256: `36e23b22eeaecf4d1abc5439173b7a447d06d4f915311e13673a8db9d1ec75b2`
- Coverage: 36 data rows and 5 fields; the unchanged Markdown is both the canonical source and retrieval form
- No separate Office/PDF original or duplicate Markdown companion is required for this approved source form

## Covered Product Hubs

- [[products/DT40|DT40]], [[products/DT50S|DT50S]], and [[products/DT50-Pro|DT50-Pro]]
- [[products/CT48|CT48]], [[products/CT48C|CT48C]], [[products/CT58|CT58]], [[products/CT58C|CT58C]], and [[products/CT58S|CT58S]]
- [[products/RT30|RT30]], [[products/RT40S|RT40S]], and [[products/SP35|SP35]]
- [[products/DT66|DT66]], [[products/DT610|DT610]], [[products/DT610-Pro|DT610 Pro]], and [[products/DT630|DT630]]
- [[products/P8100-4G|P8100 4G]], [[products/P8100P-4G|P8100P 4G]], and [[products/P8100P-5G|P8100P 5G]]
- [[products/SR5750|SR5750]], [[products/U2S|U2S]], [[products/UPad|UPad]], and [[products/K388-Pro|K388 Pro]]

## Additional Models Present

The source also contains DT50 5G, CT58 Pro, DT510, XT40, XT4, and RT47 Pro, which do not currently have canonical Product Hubs. The `DT40s` spelling and `SQ53Pro` row require model-aware routing rather than automatic string equality; `DT50S` now routes to its canonical Product Hub. Duplicate CT58C and CT58S rows are retained because the canonical Markdown is unchanged.

## Content Scope

- Market-model to internal-device/project mapping.
- Qualcomm/MediaTek platform or chipset identifiers.
- Supported or listed RAM + storage combinations by project.
- Android major version by internal project, including multiple OS-generation projects for a market family.

## Query Guidance

Use this source for quick project/configuration lookup and cross-product discovery. Preserve all five fields together: market model, internal device model, platform, memory, and Android version. Do not merge rows merely because the market-model label is similar, and do not infer that an omitted configuration is unsupported. For full public product specifications, continue to read the product-specific `specs` sources; use this matrix as user-approved internal mapping evidence.

## Active Source Discrepancies

- **CT58S / SQ58S Android version:** this matrix lists SQ58S as Android 12 and SQ58SU as Android 14. The GMS/AER and MDM workbooks label SQ58S itself as Android 14. The product-specific CT58S specification also states Android 12 without an internal-project qualifier. Keep Android 12 and 14 evidence separate and surface the exact project/source context.
- **SP35 memory options:** this matrix lists `6+64/8+128`; the SP35 product specification and device/accessories guide list `8+128` with `4+64` optional. This remains unresolved.
- **SQ53Pro market-model label:** this matrix labels SQ53Pro as `DT50`, while the MDM workbook and canonical Product Hub use `DT50 Pro` and the SQ53PRO/SQ53ST Battlecard uses `DT50PRO`. Treat the internal project as exact and surface the label difference.
- **SQ53ST market-model label:** this matrix and the Device and Accessories Guide label SQ53ST as `DT50S`, while the SQ53PRO/SQ53ST Battlecard labels the same project `DT50`. Route by the exact internal project and preserve the source-specific market label.
- **DT66 Android project label:** this matrix lists SQ66 as Android 13. The GMS/AER workbook contains both Android 13 and a later Android 15 row labeled SQ66, while its maintenance note refers to the Android 15 project as SQ66V. Preserve this labeling ambiguity rather than treating all rows as one configuration.
