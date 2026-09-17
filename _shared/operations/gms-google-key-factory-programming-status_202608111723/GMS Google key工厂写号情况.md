# GMS Google Key Factory Programming Status

> This Markdown is a semantically lossless cell-level transcription of the synchronized Excel workbook.
> Sheet order, cell coordinates, values, formulas, comments, and hyperlinks are preserved. Date-valued cells are normalized to ISO 8601 for unambiguous AI retrieval. The unchanged workbook remains authoritative for merged-cell layout, formatting, drawings, and status colors.

## Source

- Original file: `GMS Google key工厂写号情况.xlsx`
- SHA-256: `5a385f0883955ca1467983bd4080e12dadf16a3837f5cfb28bc9f53a0896d393`
- Sheets: 1
- Non-empty cells: 329
- Formulas: 0
- Comments: 0
- Hyperlinks: 0
- Merged ranges: 0
- Embedded drawings: 0

## Sheet Index

| # | Sheet | Data range | Non-empty cells | Formulas | Comments | Hyperlinks | Merged ranges | Drawings |
| ---: | --- | --- | ---: | ---: | ---: | ---: | ---: | ---: |
| 1 | Sheet1 | `A1:H72` | 329 | 0 | 0 | 0 | 0 | 0 |

## Sheet 1: Sheet1

- Data range: `A1:H72`
- Non-empty cells: 329
- Formulas: 0
- Comments: 0
- Hyperlinks: 0
- Merged ranges: 0
- Embedded drawings: 0

### Cell data

| Row | A | B | C | D | E | F | G | H |
| ---: | --- | --- | --- | --- | --- | --- | --- | --- |
| 1 | SPM 与项目名称 | 是否需要写入 Google Key | 是否存在海外版本 | 写 Google Key 方式 | 无法写 Google Key 的原因 | Google Key 判断属性 | 厂测预置情况 | 厂测设备信息 Google Key 判断 |
| 2 | 朱兵斌 |  |  |  |  |  |  |  |
| 3 | SQ53（友恺，高通660） | 是 | YES | 厂测 |  | 已导入 | 源码厂测 | 已完成 |
| 4 | SQ53H（麦博） | 否 | 没有合入GMS应用，没有海外版本 |  |  |  |  |  |
| 5 | SQ21（麦博） | 否 | 海外版本未合入GMS应用 |  |  |  |  |  |
| 6 | SQ47&SQ47D（高格，高通636&660） | 是 | YES | 厂测 |  | 已导入 | 行业厂测 |  |
| 7 | SQ53Z（SQ53升级A10） | 是 | YES | 厂测 |  | 已导入 | 早期com.ubx包名源码编译生成的apk<br>后续用行业厂测apk |  |
| 8 | SQ53X（鸿祥源，MTK6762） | 否 | Yes |  | 没有TEE,套用57项目 |  |  |  |
| 9 | SQ53B（豪成，MTK6833） | 是 | Yes | 豆荚加密狗 |  | 已导入 | 行业厂测 |  |
| 10 | SQ53XC | 否 | 没有海外版本 |  |  |  |  |  |
| 11 | SQ47S(高格，高通6115) | 是 | Yes | 厂测 |  | 已导入 | 行业厂测 |  |
| 12 | SQ83A(高格，高通6115) | 是 | Yes | 厂测 |  | 已导入 | 行业厂测 |  |
| 13 | XT4 | 是 | Yes | 写号工具 |  | 已导入 | 行业厂测 |  |
| 14 | SQ53BV(豪成，MTK6833) | 是 | Yes | 豆荚云/豆荚加密狗 |  | 已导入 | 行业厂测 |  |
| 15 | SQ83S（移远，高通4290） | 是 | Yes | 通过写号工具在user版本写入后联外网重启 |  | aosp13.0分支已导入 | 行业厂测 |  |
| 16 | SQ610 | 是 | Yes | 写号工具 |  | 已导入 | 行业厂测 |  |
| 17 | SQ81A(高通SM6115) | 是 | yes | 厂测 |  |  |  |  |
| 18 | SQ53Q（友恺，高通636） | 是 | Yes | 厂测 |  | 已导入 | 源码厂测 | 已完成 |
| 19 | SQ51 |  |  |  |  |  |  |  |
| 20 | SQ51C |  |  |  |  |  |  |  |
| 21 | SQ51CW |  |  |  |  |  |  |  |
| 22 | SQ53C（高格，高通435） | 是 | Yes | 厂测 |  | 已导入 | 源码厂测 | 已完成 |
| 23 | 邹琼芬 |  |  |  |  |  |  |  |
| 24 | SQ52&SQ52T（美格） | 否 | No |  |  |  |  |  |
| 25 | SQ52TGW（高格） | 是 | yes | 厂测 |  | android8项目不导入 | 源码厂测 |  |
| 26 | SQ51FW（高格，高通435） | 否 | no |  |  |  |  |  |
| 27 | SQ51S（友恺，高通660） | 是 | yes | 厂测 | 语言为海外时厂测有，语言为国内时，厂测没有 | 已导入 | 源码厂测 | 已完成 |
| 28 | SQ81（美格，高通435） | 是 | yes | 写SN号工具 |  | 已导入 | 源码厂测 | 已完成 |
| 29 | SQ83（高格，高通660） | 是 | yes | 厂测 | 套用SQ81的 | 已导入 | 行业厂测 |  |
| 30 | SQ55(基于SQ53X)&SQ55_5G（基于SQ53B） | 否 | 未出过海外版本 |  |  |  |  |  |
| 31 | SQ52M（鸿祥源，MTK6762） | 否 | yes |  | 套用SQ57的，没有TEE |  |  |  |
| 32 | SQ57（鸿祥源，MTK6762） | 是 | yes | PC工具 |  | 已导入 | 行业厂测 |  |
| 33 | SQ45S（高格，高通450） | 是 | Yes | 厂测 |  | 已导入 | 源码厂测 | 已完成 |
| 34 | SQ45T（SQ45S升级A12） | 是 | Yes | 厂测 |  | 已导入 | 行业厂测 |  |
| 35 | SQ66（移远，高通4290） | 是 | Yes |   |  | aosp13.0分支已导入 | 行业厂测 |  |
| 36 | SQ510（移远，MTK8755） | 否 |  |  |  |  |  |  |
| 37 | SQ520（MTK8781）暂停 | 否 |  |  |  |  |  |  |
| 38 | SQ310（A14，鸿祥源，MTK G81） | 是 | Yes | 豆荚云/豆荚加密狗 |  | 已导入 |  |  |
| 39 | SQ15 | 否 |  |  |  |  |  |  |
| 40 | SQ58/S（高格，MTK6762&8768）/S | 是 | Yes | 豆荚加密狗 |  | 已导入 | 行业厂测 |  |
| 41 | SQ58S-A14 | 是 | Yes | 加密狗 |  | 已导入 | 行业厂测 |  |
| 42 | SQ59（麦博，MTK8768） | 否 | NO |  | 只出国内版本 |  |  |  |
| 43 | SQ53ST（SQ53S升级A13） | 是 | yes | 工厂测试模式点击google key菜单项 |  | 已导入 | 行业厂测 |  |
| 44 | SQ53UR（共用53ST软件） | 是 | Yes |  |  |  |  |  |
| 45 | SQ58PRO | 否 | No |  |  |  |  |  |
| 46 | 宋子馨 |  |  |  |  |  |  |  |
| 47 | SQ38（高格，高通435） | 否 | 海外版本未合入GMS应用 |  |  |  |  |  |
| 48 | SQ45（高格，高通435） | 是 | Yes | 厂测 |  | 已导入 | 源码厂测 | 已完成 |
| 49 | SQ53A（美格，高通435） | 否 | 海外版本未合入GMS应用 |  |  |  |  |  |
| 50 | SQ46M（麦博，MTK8768）,SQ46W | 是 | Yes | PC工具 |  | SQ46M已导入<br>SQ46W android7项目不导入 | 早期com.ubx包名源码厂测编译生成的apk给方案商推送过来；后续同53B用行业厂测apk |  |
| 51 | SQ48（麦博，MTK8768） | 是 | Yes | 豆荚加密狗 | bash kernel_platform/qcom/proprietary/prebuilt_HY11/vendorsetup.sh && cd kernel_platform && python ./build_with_bazel.py -t pineapple ALL && cd .. | 已导入 | 行业厂测 |  |
| 52 | SQ51Q（友恺，高通6225） | 是 | Yes | 写号工具 |  | 已导入 | 行业厂测 |  |
| 53 | SQ48C(鸿祥源，MTK6768) | 是 | Yes | 豆荚加密狗 |  | 已导入 | 行业厂测 |  |
| 54 | SQ46S | 是 | Yes | 写号工具 |  | 已导入 |  |  |
| 55 | K388PRO | 是 | Yes | 写号工具 |  | 已导入 | 行业厂测 |  |
| 56 | SQ91 | 否 |  |  |  |  |  |  |
| 57 | SQ58C | 是 | Yes | 加密狗 |  | 已导入 | 行业厂测 |  |
| 58 | SQ45C（鸿祥源，MTK6762） | 否 | Yes |  | 没有TEE,套用57项目 |  |  |  |
| 59 | R70（蓝牙指环） | 否 | NO |  |  |  |  |  |
| 60 | SQ53S（移远，高通6115） | 是 | Yes | 工厂测试模式点击google key菜单项 |  | 已导入 | 行业厂测 |  |
| 61 | SQ630 | 是 | Yes |  | 尚未合入TEE |  |  |  |
| 62 | FR900 |  |  |  |  |  |  |  |
| 63 | 陈思羽 |  |  |  |  |  |  |  |
| 64 | SQ29WR（高格） | 是 | Yes | 工厂测试模式点击google key菜单项 |  | 已导入 | 行业厂测 |  |
| 65 | SQ28W（高格） | 是 | Yes | 工厂测试模式点击google key菜单项 |  | 已导入 | 行业厂测 |  |
| 66 | SQ27TGW（高格） | 是 | Yes | 工厂测试模式点击google key菜单项 |  | 已导入 | 行业厂测 |  |
| 67 | SQ27TG | 否 | no |  |  |  |  |  |
| 68 | SQ29（美格） | 否 | no |  |  |  |  |  |
| 69 | SQ29H | 否 | no |  |  |  |  |  |
| 70 | SQ65A | 否 | no |  |  |  |  |  |
| 71 | SQ29M | 是 | Yes | 加密狗 |  | 已导入 | 行业厂测 |  |
| 72 | SQ27M | 是 | Yes | 加密狗 |  | 已导入 | 行业厂测 |  |
