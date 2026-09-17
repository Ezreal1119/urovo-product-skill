# GMS Certification Reuse (套用) Statistics

Multi-product workbook recording which internal models reuse (套用) the GMS certification of a base certified model, keyed by the certified model's `ro.product.device` value, with the internal model and the application time (year-month).

## Synchronized Source

- Original: `_shared/certificates/gms-certification-reuse-statistics_202608151804/GMS认证套用统计.xlsx`
- Markdown: `_shared/certificates/gms-certification-reuse-statistics_202608151804/GMS认证套用统计.md`
- Workbook coverage: 1 sheet (工作表2), 29 non-empty cells, 10 merged ranges, no formulas, comments, hyperlinks, or drawings
- SHA-256: `89c3eb760275f013b91da7d666662bee2fd2b18b033dc8cd35246f660689b0e1`

## Covered Product Hubs

- [[products/CT48|CT48]] (SQ48) and [[products/CT48C|CT48C]] (SQ48C)
- [[products/CT58|CT58]] (SQ58 A12), [[products/CT58C|CT58C]] (SQ58C), and [[products/CT58S|CT58S]] (SQ58S)
- [[products/DT40|DT40]] (SQ45C)
- [[products/i9000S|i9000S]] (SQ27M) and [[products/i9100|i9100]] (SQ29M / SQ29MB / SQ29MR)
- [[products/i5300|i5300]] (SQ65B) and [[products/i5300L|i5300L]] (SQ65F)
- [[products/i9200|i9200]] (SQ68) and [[products/i9600|i9600]] (SQ69PC / SQ69D / SQ69DM / SQ69KB)
- [[products/P8100-4G|P8100 4G]] (SQ81) and [[products/P8100P-4G|P8100P 4G]] (SQ83)
- [[products/RT30|RT30]] (SQ310 A14)

## Additional Models Present

The workbook also references projects without a canonical Product Hub:

- **SQ57** — a base certified model (ro.product.device) with no current Hub; several models reuse its certification.
- **SQ53X** and **SQ52M** — reuse the SQ57 certification; no canonical Hub.
- **DT50 5G (SQ53B)** — a base certified model; the DT50 5G lineage (SQ53B/SQ53BV) is intentionally kept separate from DT50S and DT50-Pro and has no canonical Hub.
- **SQ48CU A14** and **SQ58CU A14** — Android 14 projects reusing the CT58S certification; no canonical Hub.

## Content Scope

- Five reuse (套用) groups, each headed by a base certified model (认证型号 ro.product.device) with its internal model (内部型号), the models that reuse its certification (套用机型), and the application time (套用时间/年月):

| Base certified model (ro.product.device) | Internal model | Reusing models |
| --- | --- | --- |
| SQ57 | SQ57 | SQ57, SQ29M, SQ29MB 12GO, SQ29MR, SQ27M, SQ65B, SQ65F, SQ45C, SQ53X, SQ52M |
| i9100 | SQ29MB | SQ29MB, SQ68\SQ68P\SQ68PN\SQ68MB, SQ69PC, SQ69D\SQ69DM, SQ69KB |
| DT50_5G | SQ53B | SQ53B, SQ48C, SQ58C, SQ48, SQ58 A12 |
| P8100 | SQ81 | SQ81, SQ83 |
| CT58S | SQ58S | SQ310 A14, SQ48CU A14, SQ58CU A14 |

## Query Guidance

Use this source to determine which internal models reuse (套用) another model's GMS certification, and the application time. This is a distinct, complementary record to the GMS+AER certification summary: that workbook lists certification status/region/window per project, while this one records certification reuse relationships.

- Preserve the exact internal project identifier, `ro.product.device` value, and application time; do not generalize a reuse relationship into a claim that the reusing model holds its own independent certification.
- The "A12" / "A14" suffixes on reusing models denote the Android version of that project (e.g., SQ58 A12 is the Android 12 CT58 base; SQ310 A14, SQ48CU A14, and SQ58CU A14 are Android 14 projects).
- A reusing model's Android version is not required to match the base certified model's; reuse is a certification-key/ro.product.device relationship, not a spec claim.

## Active Source Discrepancies

No unresolved same-context contradiction with the GMS+AER certification summary was identified. The reuse relationships are consistent with the certification summary's project-level records (e.g., SQ58 A12 corresponds to the Android 12 CT58 base, and the A14-suffixed projects correspond to the summary's Android 14 rows). Historical and project-specific rows remain qualified and must not be collapsed.
