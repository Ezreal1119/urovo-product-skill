# MDM Certification Summary

Multi-product internal workbook tracking device validation or certification status for SOTI, AirWatch, Springdel, Ivanti Wavelink, and TeamViewer integrations.

## Synchronized Source

- Original: `_shared/certificates/mdm-certification-summary_202608111723/MDM认证汇总.xlsx`
- Markdown: `_shared/certificates/mdm-certification-summary_202608111723/MDM认证汇总.md`
- Workbook metadata modified: 2026-08-11; no explicit internal publication or revision date is stated
- Workbook coverage: 5 sheets, 521 non-empty cells, 7 merged ranges, 4 hyperlinks, and no formulas, comments, or embedded drawings
- Date-valued cells in the Markdown are normalized to ISO 8601; explicitly typed date strings remain unchanged

## Covered Product Hubs

- [[products/DT40|DT40]], [[products/DT50S|DT50S]], [[products/DT50D|DT50D]], [[products/DT50P|DT50P]], and [[products/DT50-Pro|DT50-Pro]]
- [[products/CT48|CT48]], [[products/CT58|CT58]], [[products/CT58C|CT58C]], [[products/CT58S|CT58S]], and [[products/RT40S|RT40S]]
- [[products/DT66|DT66]], [[products/DT610|DT610]], [[products/DT610-Pro|DT610 Pro]], and [[products/DT630|DT630]]
- [[products/P8100-4G|P8100 4G]], [[products/P8100P-4G|P8100P 4G]], and [[products/P8100P-5G|P8100P 5G]]
- [[products/U2S|U2S]] and [[products/K388-Pro|K388 Pro]]
- [[products/i9000S|i9000S]] and [[products/i9100|i9100]]

## Additional Models Present

The workbook also covers models without a canonical Product Hub, including i6200, i6300, i6310/i6310C, U2, DT20, RT40, DT50 5G, P8100P SQ83, and CT58 Pro. Keep market model, internal model, Android version, MDM product, agent/plugin mode, completion status, date, and customer-specific remark together.

## Content Scope

- SOTI Android Classic Agent and Android Enterprise Plugin certification/validation records, including Xsight notes.
- AirWatch device records.
- Springdel device records and GMS qualifiers.
- Ivanti Wavelink validated-device records and official lookup/download links.
- TeamViewer device records.

## Query Guidance

Use this source for MDM compatibility, validation status, tested Android version, and completion-date questions. A completed row applies only to the stated MDM system, agent/plugin mode, internal project, Android version, and any customer-specific context. Do not interpret completion for one MDM vendor as support for another, and do not treat a blank date or version as a known value. Because these ecosystems change, frame the workbook as the latest synchronized local evidence rather than a live vendor-directory lookup.

For the OEMConfig configuration mechanism itself, see [[shared/urovo-oemconfig-manual|Urovo OEMConfig User Manual]] and, for the SOTI deployment procedure, [[shared/soti-oemconfig-guide|SOTI-OEMConfig Guide]].

## Active Source Discrepancies

- SOTI rows label SQ58S as CT58S Android 14, while the user-authored PDA matrix maps SQ58S to Android 12 and SQ58SU to Android 14.
- The Springdel row labels SQ53Pro as DT50 Pro, while the PDA matrix labels the same internal project as DT50. Android 16 agrees; the market-model label does not.

Other similar market names with different internal projects or Android versions remain separate validation contexts.
