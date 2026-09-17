# GMS and AER Certification Summary

Multi-product internal workbook covering GMS/MADA, EDLA, and Android Enterprise Recommended certification status, regional scope, certification windows, and SMR/MR maintenance history by product and internal project.

## Synchronized Source

- Original: `_shared/certificates/gms-aer-certification-summary_202609071236/GMS+AER认证汇总.xlsx`
- Markdown: `_shared/certificates/gms-aer-certification-summary_202609071236/GMS+AER认证汇总.md`
- Workbook metadata modified: 2026-09-07 sync; no explicit internal publication or revision date is stated
- Workbook coverage: 5 sheets, 981 non-empty cells, 77 merged ranges, 2 hyperlinks, 3 embedded drawings, and no formulas or comments
- Date-valued cells in the Markdown are normalized to ISO 8601; the unchanged workbook preserves layout, drawings, formatting, and colors

## Covered Product Hubs

- [[products/i9000S|i9000S]] and [[products/i9100|i9100]]
- [[products/DT40|DT40]], [[products/DT50S|DT50S]], [[products/DT50-Pro|DT50-Pro]], and [[products/RT40S|RT40S]]
- [[products/CT58S|CT58S]], [[products/DT66|DT66]], [[products/DT610|DT610]], and [[products/DT630|DT630]]
- [[products/P8100-4G|P8100 4G]], [[products/P8100P-4G|P8100P 4G]], and [[products/P8100P-5G|P8100P 5G]]
- [[products/U2S|U2S]] and [[products/K388-Pro|K388 Pro]]

## Additional Models Present

The workbook also contains certification records for models without a canonical Product Hub: i6310, EA510, XT30, i6200 Series, EA320, U2, RT40, DT20, DT20 Pro, DT50 5G, XR2, XT4, and XT40. These include UROVO, Unitech, Janam, and other customer-brand contexts. Do not transfer a customer-brand result to a UROVO model merely because the products share an internal project.

## Content Scope

- Product/project GMS and AER status by platform, chipset vendor, Android version, **认证类型** (MADA / MADA-LR / EDLA / AER), base region, optional regions, and remarks. The 市场型号 column is the market label. New GMS row: SQ53Pro / DT50 / Android 16 / MADA / ROW+EEA completed 2026.7.29.
- SMR/MR sheet adds an FP fingerprint column and additional IR-marked rows (SQ51Q, SQ46S, SQ610, K388 Pro, XR2).
- Official Google device-list links included in the workbook.
- MADA and EDLA regional definitions and restrictions.
- Android-version certification windows and Google security-patch maintenance deadlines.
- SMR/MR history, latest patch dates, website-update requirements, and project-specific maintenance remarks.

## Query Guidance

Use this source as the primary local record for GMS/AER project status, certified region, certification-window dates, and SMR/MR history. Always preserve the exact internal project, market model, Android version, MADA-versus-EDLA mode, region, customer brand, and maintenance date. Certification and maintenance data are time-sensitive; state the workbook's last-updated context and do not generalize a historical or project-specific row into a model-wide current claim.

For general product specifications, retain the normal product-specific source hierarchy. Platform and Android columns here describe the certification configuration and may differ legitimately from another hardware or OS variant.

## Active Source Discrepancies

- CT58S/SQ58S is labeled Android 14 here, while the user-authored PDA matrix maps SQ58S to Android 12 and SQ58SU to Android 14; the product-specific CT58S specification also states Android 12 without an SQ qualifier.
- This revision labels the Android 15 DT66 project **SQ66V** on both the GMS and AER blocks. The earlier workbook had printed that Android 15 GMS row as SQ66. The PDA matrix still maps SQ66 to Android 13; keep using SQ66 for Android 13 and SQ66V for Android 15.

Other differences across SQ projects, regions, customer brands, and dated SMR/MR records are contextual and must not be collapsed.
