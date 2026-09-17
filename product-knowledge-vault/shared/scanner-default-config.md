# Scanner 默认配置说明（Default Profile）

**Source type:** user-authored canonical Markdown (one-file source slot, no companion). 平台级参考（portfolio-wide，适用于所有 UROVO 条码扫描设备）。

**Paths:**
- Markdown: `_shared/operations/scanner-default-config_202608170900/Scanner默认配置说明.md`（唯一文件，未改动）

**Scope:** UROVO 扫描器 `Default` profile（源自 `Default_scanner_property.xml`）的**默认配置说明**——按功能分组逐项列出配置参数、默认值与含义，覆盖：

1. **配置基本信息**（profileName/Enable、scanwedge 总开关）
2. **码制配置**（1D / 2D / 复合码 / 邮政码的默认开启/关闭状态，含各码制的长度范围、校验位、静区、安全等级等）
3. **输出配置**（键盘模拟 / Intent 广播 / 剪贴板 / TCP/IP 网络输出 / 缓存）
4. **数据后处理**（追加回车、前后缀、正则匹配替换、编码格式、UDI 解析、高级格式化）
5. **触发与省电**（触发模式、低功耗休眠、免持移动感应）
6. **解码行为**（全读、多码同时解码、模糊处理、居中解码）
7. **成像/曝光/补光**（自动曝光、增益、Gamma、瞄准圈）
8. **图像预处理/低对比度增强**（直方图均衡、平滑、锐化、形态学）
9. **OCR**（模式/模板）
10. **引擎与其他**（引擎类型选择、成功提示音/震动、BKN 子选项）

**默认开启码制速览：**
- **1D**：Code 39、Code 128（含 GS1-128、ISBT 128）、Interleaved 2 of 5、Codabar、UPC-A、EAN-13、EAN-8
- **2D**：QR Code、Data Matrix、PDF417、Aztec、MaxiCode

## Query Guidance

回答「UROVO 扫描器默认开启哪些码制」「某参数（如触发模式、输出方式、前后缀、校验位、安全等级）的默认值是什么」「如何配置扫描结果输出到 Intent/剪贴板/网络」等扫描配置类问题。配合 [[shared/scan-settings-user-manual|Scan Settings User Manual]] 使用。

## Cross-references

- [[shared/scan-settings-user-manual|Scan Settings User Manual]] — 内置条码扫描配置 App 的用户手册（码制、输出模式、前后缀、触发）
- [[shared/scan-data-advanced-formatting|Scan Data Advanced Formatting]] — 扫描数据高级格式化与输出控制
- Scan Engine Specifications — [[shared/honeywell-ex30-scan-engine|Honeywell EX30]], [[shared/honeywell-n570x-scan-engine|Honeywell N570X]], [[shared/honeywell-n6803-scan-engine|Honeywell N6803]], [[shared/zebra-se55-scan-engine|Zebra SE55]], [[shared/zebra-se58-scan-engine|Zebra SE58]], and [[shared/urovo-se2030s-scan-engine|UROVO SE2030S]]

## Discrepancies

None recorded.
