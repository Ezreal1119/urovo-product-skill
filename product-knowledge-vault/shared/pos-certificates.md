# POS Certificates and Firmware Validity

Multi-product internal workbook tracking payment, security, platform, regulatory, and quality certifications by POS model, hardware project, software configuration, report/certificate number, approval date, and expiry date.

## Synchronized Source

- Original: `_shared/certificates/pos-certificates_202608111641/pos-certificates.xlsx`
- Markdown: `_shared/certificates/pos-certificates_202608111641/pos-certificates.md`
- Workbook metadata modified: 2026-08-11; no explicit internal publication or revision date is stated
- Workbook coverage: 18 sheets, 3,419 non-empty cells, 452 merged ranges, no formulas, comments, hyperlinks, or embedded drawings
- Date-valued cells in the Markdown are normalized to ISO 8601; the unchanged workbook preserves merged-cell layout, formatting, and status colors

## Covered Product Hubs

- [[products/i5300|i5300]] and [[products/i5300L|i5300L]]
- [[products/i9000S|i9000S]]
- [[products/i9100|i9100]]
- [[products/i9200|i9200]]
- [[products/i9600|i9600]]

## Additional Models Present

The workbook also contains certificate records for models or project names that do not currently have a canonical single-product directory or Product Hub: i2000, i5000, Q1000, Q1500, Q2000, Q3000, Q5000, T5000, i9101, and the i9200K/i9600K project variants. Query these records directly from the synchronized Markdown while retaining the exact sheet, device model, configuration, and project qualifiers.

## Content Scope

- Current and historical certifications for i9600/i9600K, i9200/i9200K, i5300/i5300L, i9100 project variants, i9000S project variants, and additional legacy or non-canonical POS models.
- Payment certification families including PBOC/qPBOC, EMV L1/L2 and contactless L1, PayPass, payWave, AMEX, Discover, JCB, PURE, RuPay, QUICS/QuickPass, NSICCS, and VCCS where present.
- PCI PTS or PCI PIN records, TQM statements, UnionPay security/application tests, national cryptography, hardware serial-number, regulatory, and other model-specific certifications.
- Report/certificate identifiers, approval dates, expiry dates, status labels, configuration strings, firmware-renewal dates, and workbook remarks.
- A dedicated `PCI固件续期` sheet that separates PCI hardware expiry from PCI firmware expiry by product and configuration.

## Query Guidance

Use this source as the primary local record for certificate status, certificate/report numbers, approval dates, expiry dates, and PCI firmware validity. Always preserve the exact product variant, internal project, OS, security-chip/configuration, certificate type, and report-versus-certificate distinction.

Certificate validity is time-sensitive. Do not treat the workbook label `已通过` as proof that a certificate is still currently valid: compare the applicable `有效期至` or PCI firmware expiry against the date of the user's question. Do not infer a missing date, and do not apply one project's certificate to a different configuration. For general product capability, retain the normal product-specific source hierarchy; for dated certification status, this workbook supplies the more specific temporal evidence.

## Active Source Discrepancies

No unresolved same-context contradiction with the synchronized product-specific sources was identified during this sync. Differences among SQ/project variants, OS versions, hardware/security-chip configurations, historical rows, and expiry dates are contextual and must not be collapsed into a single model-wide status.
