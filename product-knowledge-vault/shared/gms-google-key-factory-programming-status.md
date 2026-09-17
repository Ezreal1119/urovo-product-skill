# GMS Google Key Factory Programming Status

Multi-product internal workbook tracking whether each hardware/software project requires a Google Key, whether an overseas build exists, the factory programming method, key-property import status, and factory-test provisioning status.

## Synchronized Source

- Original: `_shared/operations/gms-google-key-factory-programming-status_202608111723/GMS Google key工厂写号情况.xlsx`
- Markdown: `_shared/operations/gms-google-key-factory-programming-status_202608111723/GMS Google key工厂写号情况.md`
- Workbook metadata modified: 2026-08-11; no explicit internal publication or revision date is stated
- Workbook coverage: 1 sheet, 329 non-empty cells, no formulas, comments, hyperlinks, merged ranges, or embedded drawings

## Covered Product Hubs

- [[products/DT40|DT40]], [[products/DT50S|DT50S]], and [[products/RT40S|RT40S]]
- [[products/CT48|CT48]], [[products/CT48C|CT48C]], [[products/CT58|CT58]], [[products/CT58C|CT58C]], and [[products/CT58S|CT58S]]
- [[products/DT66|DT66]], [[products/DT610|DT610]], and [[products/DT630|DT630]]
- [[products/P8100-4G|P8100 4G]], [[products/P8100P-4G|P8100P 4G]], and [[products/P8100P-5G|P8100P 5G]]
- [[products/U2S|U2S]] and [[products/K388-Pro|K388 Pro]]
- [[products/i9000S|i9000S]] and [[products/i9100|i9100]]

## Additional Projects Present

The workbook is organized primarily by internal SPM/project identifiers rather than market model names. It also contains projects without a canonical Product Hub, including SQ21, SQ38, SQ45, SQ46M/S/W, SQ47/D, SQ51 variants, SQ52 variants, SQ53 variants, SQ55 variants, SQ57, SQ58 Pro, SQ59, SQ65A, SQ83S, SQ91, SQ310, SQ510, SQ520, XT4, R70, and FR900. Retain the exact project identifier and supplier/platform qualifier when answering.

## Content Scope

- Whether Google Key writing is required and whether an overseas/GMS build exists.
- Factory, PC-tool, serial-number-tool, encrypted-dongle, or cloud-based writing methods.
- Reasons that a project cannot write a Google Key, TEE limitations, and branch-specific exceptions.
- Google Key property-import status and factory-test application/provisioning status.

## Query Guidance

Use this source for factory provisioning and Google Key operational questions, not as a general product specification or as proof of GMS certification. Many rows identify only an internal project; map a row to a market product only when another synchronized source or the row itself establishes that relationship. Preserve supplier, chipset, Android branch, package-name, TEE, and domestic-versus-overseas qualifiers.

## Active Source Discrepancies

No unresolved same-context contradiction was identified during this sync. Blank status cells mean the workbook does not state a result; they must not be interpreted as `No`, incomplete, or unsupported.
