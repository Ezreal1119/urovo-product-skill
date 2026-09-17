# POS Financial Certification Kernel Versions

Multi-product internal workbook mapping POS hardware projects to ICCR/PCD and payment-application kernel names and version numbers for EMV and major contactless schemes.

## Synchronized Source

- Original: `_shared/certificates/pos-financial-certification-kernel-versions_202608111723/POS金融认证（L1& L2）版本号统计.xlsx`
- Markdown: `_shared/certificates/pos-financial-certification-kernel-versions_202608111723/POS金融认证（L1& L2）版本号统计.md`
- Workbook metadata modified: 2026-08-11; no explicit internal publication or revision date is stated
- Workbook coverage: 1 sheet, 251 non-empty cells, and no formulas, comments, hyperlinks, merged ranges, or embedded drawings

## Covered Product Hubs

- [[products/i9000S|i9000S]]
- [[products/i9100|i9100]]
- [[products/i5300|i5300]]
- [[products/i9200|i9200]]
- [[products/i9600|i9600]]

## Additional Models Present

The workbook also contains version columns for i2000 (SQ28W) and i5000 (SQ65A), which do not currently have canonical Product Hubs. It distinguishes multiple i9000S and i9100 hardware projects; preserve the exact SQ identifier for every lookup.

## Content Scope

- ICCR, ICCR-HW, ICCR-SW, PCD, PCD-HW, and PCD-SW version identifiers.
- EMV L2 application kernel versions.
- payWave, PayPass, AMEX Expresspay, JCB, Discover/D-PAS, PURE, RuPay, QuickPass/qUICS, NSICCS, VCCS, and MIR kernel versions where present.
- Explicit `/` or blank cells showing that the matrix states no version for that project/scheme.

## Query Guidance

Use this source for payment-kernel names and version numbers, while [[shared/pos-certificates|POS Certificates and Firmware Validity]] remains the primary source for certification status, report/certificate identifiers, approval dates, expiry dates, and PCI firmware validity. Never infer that a listed kernel version is currently certified or unexpired without the corresponding dated certificate record. Preserve the market model, internal SQ project, certification family, component layer, exact capitalization, and version string.

## Active Source Discrepancies

No unresolved same-context contradiction with the POS certificate workbook was identified during this sync. The two sources are complementary: one records software/kernel versions and the other records dated certification evidence.
