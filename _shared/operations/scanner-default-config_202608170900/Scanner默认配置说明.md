# Scanner 默认配置说明文档

> 来源：`Default_scanner_property.xml`（profile 名称：`Default`）
> 说明：本文档按功能分组，逐项列出配置参数、默认值及含义。码制（Symbology）部分标注了默认开启/关闭状态。
> 注：个别参数为厂商枚举值（如触发模式、编码格式等），具体枚举映射请以对应扫描器 SDK 文档为准。

---

## 一、配置基本信息

| 配置项 | 默认值 | 说明 |
|---|---|---|
| `profileName` | `Default` | 配置文件名 |
| `profileEnable` | `true` | 该配置是否启用 |
| `scanwedgeEnable` | `false` | 扫描楔（键盘模拟输入）总开关 |

---

## 二、码制配置（Symbology）

### 2.1 一维条码（1D）

| 参数 | 默认值 | 说明 | 默认状态 |
|---|---|---|---|
| `CODE39_ENABLE` | `1` | Code 39（工业/物流常用） | ✅ 开启 |
| `CODE39_ENABLE_CHECK` | `0` | 是否校验 Code 39 校验位 | — |
| `CODE39_SEND_CHECK` | `0` | 是否发送校验位 | — |
| `CODE39_FULL_ASCII` | `0` | 全 ASCII 模式（支持小写等） | 关闭 |
| `CODE39_LENGTH1` | `2` | 最小长度 | — |
| `CODE39_LENGTH2` | `55` | 最大长度 | — |
| `CODE39_Quiet_Zone` | `1` | 静区要求 | — |
| `CODE39_START_STOP` | `0` | 是否发送起止符（*） | — |
| `CODE39_SECURITY_LEVEL` | `0` | 安全等级 | — |
| `TRIOPTIC_ENABLE` | `0` | Trioptic Code 39 | ❌ 关闭 |
| `CODE32_ENABLE` | `0` | Code 32（意大利药品码） | ❌ 关闭 |
| `CODE32_SEND_START` | `0` | 是否发送 Code 32 起始符 | — |
| `C25_ENABLE` | `0` | Standard/Industrial 2 of 5 | ❌ 关闭 |
| `D25_ENABLE` | `0` | Discrete 2 of 5 | ❌ 关闭 |
| `D25_LENGTH1` | `2` | 最小长度 | — |
| `D25_LENGTH2` | `48` | 最大长度 | — |
| `M25_ENABLE` | `0` | Matrix 2 of 5 | ❌ 关闭 |
| `M25_ENABLE_CHECK` | `0` | 是否校验 | — |
| `M25_SEND_CHECK` | `0` | 是否发送校验位 | — |
| `M25_LENGTH1` | `4` | 最小长度 | — |
| `M25_LENGTH2` | `55` | 最大长度 | — |
| `CODE11_ENABLE` | `0` | Code 11 | ❌ 关闭 |
| `CODE11_ENABLE_CHECK` | `0` | 是否校验 | — |
| `CODE11_SEND_CHECK` | `0` | 是否发送校验位 | — |
| `CODE11_LENGTH1` | `4` | 最小长度 | — |
| `CODE11_LENGTH2` | `55` | 最大长度 | — |
| `I25_ENABLE` | `1` | Interleaved 2 of 5（ITF，物流常用） | ✅ 开启 |
| `I25_ENABLE_CHECK` | `0` | 是否校验 | — |
| `I25_SEND_CHECK` | `0` | 是否发送校验位 | — |
| `I25_LENGTH1` | `6` | 最小长度 | — |
| `I25_LENGTH2` | `55` | 最大长度 | — |
| `I25_TO_EAN13` | `0` | 是否转换为 EAN-13 | — |
| `I25_QUIET_ZONE` | `1` | 静区要求 | — |
| `I25_SECURITY_LEVEL` | `1` | 安全等级 | — |
| `IATA25_ENABLE` | `0` | IATA 2 of 5（航空货运） | ❌ 关闭 |
| `IATA25_LENGTH1` | `4` | 最小长度 | — |
| `IATA25_LENGTH2` | `80` | 最大长度 | — |
| `CODABAR_ENABLE` | `1` | Codabar（NW-7，医疗/图书/血库） | ✅ 开启 |
| `CODABAR_NOTIS` | `0` | NOTIS 变体 | — |
| `CODABAR_CLSI` | `0` | CLSI（医疗）变体 | — |
| `CODABAR_LENGTH1` | `6` | 最小长度 | — |
| `CODABAR_LENGTH2` | `55` | 最大长度 | — |
| `CODABAR_ENABLE_CHECK` | `0` | 是否校验 | — |
| `CODABAR_SEND_CHECK` | `0` | 是否发送校验位 | — |
| `CODABAR_SEND_START` | `0` | 是否发送起止符 | — |
| `CODABAR_CONCATENATE` | `0` | 是否拼接多段 | — |
| `CB_SECURITY_LEVEL` | `1` | 安全等级 | — |
| `CODE93_ENABLE` | `0` | Code 93 | ❌ 关闭 |
| `CODE93_LENGTH1` | `4` | 最小长度 | — |
| `CODE93_LENGTH2` | `55` | 最大长度 | — |
| `CODE128_ENABLE` | `1` | Code 128（通用，含 GS1-128） | ✅ 开启 |
| `CODE128_LENGTH1` | `1` | 最小长度 | — |
| `CODE128_LENGTH2` | `80` | 最大长度 | — |
| `CODE_ISBT_128` | `1` | ISBT 128（输血医学标准） | ✅ 开启 |
| `CODE128_GS1_ENABLE` | `1` | GS1-128（UCC/EAN-128） | ✅ 开启 |
| `CODE128_REDUCED_QUIET_ZONE` | `2` | 缩减静区模式 | — |
| `CODE128_CHECK_ISBT_TABLE` | `1` | 是否校验 ISBT 表 | — |
| `CODE_ISBT_Concatenation_MODE` | `0` | ISBT 拼接模式 | — |
| `CODE128_SECURITY_LEVEL` | `0` | 安全等级 | — |
| `CODE128_IGNORE_FNC4` | `0` | 是否忽略 FNC4 | — |
| `CODE128_REDUNDANCY_LEVEL` | `0` | 冗余等级 | — |
| `UPCA_ENABLE` | `1` | UPC-A（北美零售） | ✅ 开启 |
| `UPCA_SEND_CHECK` | `1` | 是否发送校验位 | — |
| `UPCA_SEND_SYS` | `1` | 是否发送系统位 | — |
| `UPCA_TO_EAN13` | `0` | 是否转换为 EAN-13 | — |
| `UPCE_ENABLE` | `0` | UPC-E | ❌ 关闭 |
| `UPCE_SEND_CHECK` | `1` | 是否发送校验位 | — |
| `UPCE_SEND_SYS` | `1` | 是否发送系统位 | — |
| `UPCE_TO_UPCA` | `0` | 是否转换为 UPC-A | — |
| `UPCE1_ENABLE` | `0` | UPC-E1 | ❌ 关闭 |
| `UPCE1_SEND_CHECK` | `1` | 是否发送校验位 | — |
| `UPCE1_SEND_SYS` | `1` | 是否发送系统位 | — |
| `UPCE1_TO_UPCA` | `0` | 是否转换为 UPC-A | — |
| `EAN13_ENABLE` | `1` | EAN-13（全球零售） | ✅ 开启 |
| `EAN13_SEND_CHECK` | `1` | 是否发送校验位 | — |
| `EAN13_BOOKLANDEAN` | `0` | Bookland（ISBN/ISSN）转换 | — |
| `EAN13_BOOKLAND_FORMAT` | `0` | Bookland 输出格式 | — |
| `EAN8_ENABLE` | `1` | EAN-8（小包装零售） | ✅ 开启 |
| `EAN8_SEND_CHECK` | `1` | 是否发送校验位 | — |
| `EAN8_TO_EAN13` | `0` | 是否转换为 EAN-13 | — |
| `EAN_EXT_ENABLE_2_5_DIGIT` | `0` | EAN/UPC 2/5 位附加码 | ❌ 关闭 |
| `UPC_EAN_SECURITY_LEVEL` | `0` | UPC/EAN 安全等级 | — |
| `UCC_COUPON_EXT_CODE` | `0` | UCC 优惠券扩展码 | ❌ 关闭 |
| `UCC_REDUCED_QUIET_ZONE` | `1` | UCC 缩减静区 | — |
| `UCC_COUPON_EXT_REPORT_MODE` | `0` | 优惠券扩展上报模式 | — |
| `UCC_EAN_ZERO_EXTEND` | `0` | 是否补零扩展 | — |
| `UCC_EAN_SUPPLEMENTAL_MODE` | `0` | 附加码模式 | — |
| `UCC_EAN_SUPP_Redundancy` | `1` | 附加码冗余 | — |
| `MSI_ENABLE` | `0` | MSI/Plessey | ❌ 关闭 |
| `MSI_REQUIRE_2_CHECK` | `0` | 是否要求双校验位 | — |
| `MSI_SEND_CHECK` | `0` | 是否发送校验位 | — |
| `MSI_CHECK_2_MOD_11` | `0` | 第二校验位是否 Mod 11 | — |
| `MSI_LENGTH1` | `4` | 最小长度 | — |
| `MSI_LENGTH2` | `55` | 最大长度 | — |
| `GS1_14_ENABLE` | `0` | GS1 DataBar-14（Omnidirectional/RSS-14） | ❌ 关闭 |
| `GS1_14_TO_UPC_EAN` | `0` | 是否转换为 UPC/EAN | — |
| `GS1_LIMIT_ENABLE` | `0` | GS1 DataBar Limited | ❌ 关闭 |
| `GS1_LIMIT_Security_Level` | `3` | 安全等级 | — |
| `GS1_EXP_ENABLE` | `0` | GS1 DataBar Expanded | ❌ 关闭 |
| `GS1_EXP_LENGTH1` | `1` | 最小长度 | — |
| `GS1_EXP_LENGTH2` | `74` | 最大长度 | — |

### 2.2 二维条码（2D）

| 参数 | 默认值 | 说明 | 默认状态 |
|---|---|---|---|
| `PDF417_ENABLE` | `1` | PDF417（运输/证件） | ✅ 开启 |
| `PDF417_LENGTH1` | `1` | 最小长度 | — |
| `PDF417_LENGTH2` | `2750` | 最大长度 | — |
| `MICROPDF417_ENABLE` | `0` | Micro PDF417 | ❌ 关闭 |
| `DATAMATRIX_ENABLE` | `1` | Data Matrix（制造/医疗追溯） | ✅ 开启 |
| `DATAMATRIX_LENGTH1` | `1` | 最小长度 | — |
| `DATAMATRIX_LENGTH2` | `3166` | 最大长度 | — |
| `DATAMATRIX_INVERSE` | `0` | 反白解码 | — |
| `DATAMATRIX_SYMBOL_SIZE` | `1` | 符号尺寸 | — |
| `DPM_DECODE_MODE` | `0` | DPM（激光点阵刻印）解码模式 | 关闭 |
| `MAXICODE_ENABLE` | `1` | MaxiCode（UPS 快递） | ✅ 开启 |
| `MAXICODE_SYMBOL_SIZE` | `1` | 符号尺寸 | — |
| `QRCODE_ENABLE` | `1` | QR Code（最常见 2D 码） | ✅ 开启 |
| `QRCODE_INVERSE` | `0` | 反白解码 | — |
| `QRCODE_LENGTH1` | `1` | 最小长度 | — |
| `QRCODE_LENGTH2` | `7089` | 最大长度 | — |
| `QRCODE_SYMBOL_SIZE` | `1` | 符号尺寸 | — |
| `QR_WITHOUT_QZ` | `0` | 无静区 QR 解码 | — |
| `QR_NON_SQUARE_MODULES` | `0` | 非方形模块解码 | — |
| `MICROQRCODE_ENABLE` | `0` | Micro QR | ❌ 关闭 |
| `AZTEC_ENABLE` | `1` | Aztec（电子票券/登机牌） | ✅ 开启 |
| `AZTEC_INVERSE` | `0` | 反白解码 | — |
| `AZTEC_LENGTH1` | `1` | 最小长度 | — |
| `AZTEC_LENGTH2` | `3832` | 最大长度 | — |
| `AZTEC_SYMBOL_SIZE` | `1` | 符号尺寸 | — |
| `HANXIN_ENABLE` | `0` | 汉信码（中国国标 GB/T 21049） | ❌ 关闭 |
| `HANXIN_INVERSE` | `0` | 反白解码 | — |
| `HANXIN_LENGTH1` | `1` | 最小长度 | — |
| `HANXIN_LENGTH2` | `6000` | 最大长度 | — |
| `DOTCODE_ENABLE` | `0` | DotCode（烟草行业） | ❌ 关闭 |
| `DOTCODE_LENGTH1` | `1` | 最小长度 | — |
| `DOTCODE_LENGTH2` | `2400` | 最大长度 | — |
| `GRIDMATRIX_ENABLED` | `0` | Grid Matrix（中国国标 GB/T 41210） | ❌ 关闭 |
| `GM_LENGTH1` | `1` | 最小长度 | — |
| `GM_LENGTH2` | `2751` | 最大长度 | — |

### 2.3 复合码（Composite）

| 参数 | 默认值 | 说明 | 默认状态 |
|---|---|---|---|
| `GS1128__UCCEAN_Composite` | `0` | GS1-128 复合码 | ❌ 关闭 |
| `COMPOSITE_UPC_MODE` | `0` | UPC 复合码模式 | ❌ 关闭 |
| `COMPOSITE_CC_AB_ENABLE` | `0` | Composite CC-A/B | ❌ 关闭 |
| `COMPOSITE_CC_C_ENABLE` | `0` | Composite CC-C | ❌ 关闭 |
| `COMPOSITE_TLC39_ENABLE` | `0` | TLC-39 | ❌ 关闭 |

### 2.4 邮政码（Postal）

| 参数 | 默认值 | 说明 | 默认状态 |
|---|---|---|---|
| `US_POSTNET_ENABLE` | `0` | 美国 Postnet | ❌ 关闭 |
| `US_PLANET_ENABLE` | `0` | 美国 Planet | ❌ 关闭 |
| `US_POSTAL_SEND_CHECK` | `1` | 是否发送校验位 | — |
| `USPS_4STATE_ENABLE` | `0` | USPS 4-State（智能邮件码） | ❌ 关闭 |
| `UPU_FICS_ENABLE` | `0` | UPU FICS（国际邮政） | ❌ 关闭 |
| `ROYAL_MAIL_ENABLE` | `0` | 英国皇家邮政码 | ❌ 关闭 |
| `ROYAL_MAIL_SEND_CHECK` | `1` | 是否发送校验位 | — |
| `AUSTRALIAN_POST_ENABLE` | `0` | 澳大利亚邮政码 | ❌ 关闭 |
| `KIX_CODE_ENABLE` | `0` | 荷兰 KIX 码 | ❌ 关闭 |
| `JAPANESE_POST_ENABLE` | `0` | 日本邮政码 | ❌ 关闭 |
| `KOREA_POST_ENABLE` | `0` | 韩国邮政码 | ❌ 关闭 |
| `Canadian_POSTAL_ENABLE` | `0` | 加拿大邮政码 | ❌ 关闭 |
| `POSTAL_GROUP_TYPE_ENABLE` | `0` | 邮政码分组类型 | ❌ 关闭 |

---

## 三、输出配置（数据往哪儿送）

| 参数 | 默认值 | 说明 |
|---|---|---|
| `WEDGE_KEYBOARD_ENABLE` | `1` | 键盘模拟输出（在光标处输入扫描结果） |
| `WEDGE_KEYBOARD_TYPE` | `0` | 键盘模拟类型 |
| `WEDGE_INTENT_ENABLE` | `1` | 广播 Intent 输出 |
| `WEDGE_INTENT_DELIVERY_MODE` | `2` | Intent 投递模式（显式/隐式等） |
| `WEDGE_INTENT_FOREGROUND_FLAG` | `0` | 是否限定前台应用 |
| `WEDGE_INTENT_CATEGORY_NAME` | 空 | Intent 分类名 |
| `WEDGE_INTENT_PACKAGE_NAME` | 空 | Intent 目标包名 |
| `WEDGE_INTENT_ACTION_NAME` | `android.intent.ACTION_DECODE_DATA` | Intent Action |
| `INTENT_LABEL_TYPE_TAG` | 空 | 标签类型字段名 |
| `INTENT_DATA_STRING_TAG` | `barcode_string` | 数据字符串字段名 |
| `INTENT_DECODE_DATA_TAG` | `barcode` | 解码数据字段名 |
| `OUT_EDITORTEXT_MODE` | `0` | 输出到编辑器文本框模式 |
| `OUT_CLIPBOARD_ENABLE` | `0` | 输出到剪贴板 |
| `OUT_CLIPBOARD_PASTE_ENABLE` | `0` | 剪贴板自动粘贴 |
| `IP_OUTPUT_WEDGE` | `0` | 网络（TCP/IP）输出 |
| `IP_OUTPUT_ADDRESS` | `0.0.0.0` | 网络输出地址 |
| `IP_OUTPUT_PORT` | `60000` | 网络输出端口 |
| `IP_OUTPUT_PROTOCOL` | `0` | 网络输出协议 |
| `CACHE_DATA_ENABLE` | `0` | 缓存扫描数据 |
| `CACHE_DATA_LIMIT_ENABLE` | `0` | 缓存条数限制 |
| `CACHE_DATA_LIMIT_TIME` | `30000` | 缓存时间限制（毫秒） |

---

## 四、数据后处理（对扫描结果做加工）

| 参数 | 默认值 | 说明 |
|---|---|---|
| `LABEL_APPEND_ENTER` | `1` | 扫描结果后自动追加回车 |
| `APPEND_ENTER_DELAY` | `0` | 追加回车延迟（毫秒） |
| `CHARACTER_DATA_DELAY` | `0` | 字符输出延迟（毫秒） |
| `LABEL_PREFIX` | 空 | 扫描结果前缀 |
| `LABEL_SUFFIX` | 空 | 扫描结果后缀 |
| `SEND_LABEL_PREFIX_SUFFIX` | `0` | 是否发送前后缀 |
| `LABEL_SEPARATOR_ENABLE` | `0` | 多码分隔符开关 |
| `LABEL_FORMAT_SEPARATOR_CHAR` | `()` | 多码分隔符字符 |
| `LABEL_MATCHER_PATTERN` | 空 | 匹配模式 |
| `LABEL_MATCHER_TARGETREGEX` | 空 | 目标正则表达式 |
| `LABEL_MATCHER_REPLACEMENT` | 空 | 正则替换文本 |
| `REMOVE_NONPRINT_CHAR` | `0` | 移除不可见字符 |
| `CODING_FORMAT` | `9` | 输出字符编码格式（枚举） |
| `CODING_FORMAT_NAME` | 空 | 编码格式名称 |
| `OUTPUT_HEX_STRING_DATA` | `0` | 以十六进制字符串输出 |
| `CONVERT_CHARACTER_CASE` | `0` | 大小写转换（0=不转换） |
| `TRANSMIT_CODE_ID` | `0` | 附加码制 ID |
| `SEND_TOKENS_OPTION` | `0` | Token 发送选项 |
| `SEND_TOKENS_FORMAT` | `0` | Token 格式 |
| `SEND_TOKENS_SEPARATOR` | `0` | Token 分隔符 |
| `SEND_CONTROL_CHAR_AS_EVENTS` | `0` | 控制字符作为事件发送 |
| `ADVANCE_FORMAT_ENABLE` | `1` | 高级格式化 |
| `FORMAT_SUBSTRING_MODE` | `0` | 子串格式化模式 |
| `FORMAT_PROCESS_SYMID` | `-1` | 格式化目标码制 ID |
| `FORMAT_SUBSTRING_INDEX` | `0` | 子串起始索引 |
| `FORMAT_SUBSTRING_MATCH_STR` | 空 | 子串匹配字符串 |
| `FORMAT_SUBSTRING_LENGTH` | `-1` | 子串长度 |
| `ENABLE_PARSER_UDICODE` | `62` | UDI（唯一设备标识）解析器开关/掩码 |
| `ENABLE_FORMAT_UDI_DATE` | `0` | UDI 日期格式化 |
| `WEBJUMP` | `0` | 网页跳转（扫描 URL 自动打开） |

---

## 五、触发与省电

| 参数 | 默认值 | 说明 |
|---|---|---|
| `SCANNER_ENABLE` | `1` | 扫描器总开关 |
| `TRIGGERING_MODES` | `8` | 触发模式（枚举：手动/自动瞄准/连续等） |
| `TRIGGERING_LOCK` | `0` | 触发锁定 |
| `TRIGGERING_SLEEP_WORK` | `0` | 休眠时触发工作 |
| `SCAN_HANDLE` | `1` | 扫描手柄（按键） |
| `SUSPENSION_BUTTON` | `0` | 挂起按钮 |
| `LOW_POWER_SLEEP_MODE` | `1` | 低功耗休眠开关 |
| `LOW_POWER_SLEEP_TIMEOUT` | `15000` | 休眠超时（毫秒，15 秒） |
| `HANDSFREE_MOTION_MODE` | `0` | 免持移动感应模式 |
| `MOTION_ILLUMINATION` | `1` | 移动补光 |
| `CONTINUOUS_SCAN_INVALID_TIMEOUT` | `60000` | 连续扫描失效超时（毫秒） |

---

## 六、解码行为（1D/2D 策略）

| 参数 | 默认值 | 说明 |
|---|---|---|
| `FULL_READ_MODE` | `1` | 全读模式 |
| `BAR_CODES_TO_READ` | `1` | 每次读取的条码数量 |
| `MULTI_DECODE_MODE` | `0` | 多码同时解码 |
| `MULTI_DECODE_GS_CHAR` | `\x0a` | 多码间分隔符（换行） |
| `DEC_MaxMultiRead_COUNT` | `3` | 多码读取最大数量 |
| `DEC_Multiple_Decode_TIMEOUT` | `5000` | 多码解码超时（毫秒） |
| `DEC_Multiple_Decode_INTERVAL` | `100` | 多码解码间隔（毫秒） |
| `DEC_Multiple_Decode_MODE` | `0` | 多码解码模式 |
| `FIXED_MultiRead_COUNT` | `0` | 固定多码读取数量 |
| `FUZZY_1D_PROCESSING` | `1` | 1D 模糊处理 |
| `LINEAR_CODE_TYPE_SECURITY_LEVEL` | `0` | 线性码安全等级 |
| `LINEAR_1D_QUIET_ZONE_LEVEL` | `1` | 1D 静区等级 |
| `VARIABLE_LENGTH_1D_LIMIT` | `0` | 变长 1D 限制 |
| `VARIABLE_1D_MIN_LENGTH` | `2` | 变长 1D 最小长度 |
| `LINEAR_BOUNDARY_CHECK` | `0` | 线性码边界检查 |
| `IMAGE_ONE_D_INVERSE` | `0` | 反白 1D 解码 |
| `TIMEOUT_BETWEEN_SAME_SYMBOL` | `10` | 同一码重复输出间隔（毫秒） |
| `LASER_ON_TIME` | `50` | 激光开启时间 |
| `IMAGE_PICKLIST_MODE` | `0` | Picklist（瞄准）模式 |
| `DEC_EachImageAttempt_TIME` | `125` | 每帧图像尝试解码时间（毫秒） |
| `DEC_DECODE_DELAY` | `0` | 解码延迟 |
| `DEC_DECODE_DEBUG_MODE` | `0` | 解码调试模式 |
| `DPM_DECODE_MODE` | `0` | DPM 解码模式 |
| `DEC_2D_LIGHTS_MODE` | `3` | 2D 补光模式 |
| `DEC_2D_CENTERING_ENABLE` | `0` | 2D 居中解码 |
| `DEC_2D_CENTERING_MODE` | `3` | 2D 居中模式 |
| `DEC_2D_WINDOW_UPPER_LX` | `632` | 居中窗口左上 X |
| `DEC_2D_WINDOW_UPPER_LY` | `392` | 居中窗口左上 Y |
| `DEC_2D_WINDOW_LOWER_RX` | `640` | 居中窗口右下 X |
| `DEC_2D_WINDOW_LOWER_RY` | `400` | 居中窗口右下 Y |
| `DEC_2D_DEBUG_WINDOW_ENABLE` | `0` | 2D 窗口调试 |
| `SEARCH_CYCLING_FINDER` | `0` | 循环查找 |
| `MULTI_THREAD_DECODER_MODE` | `0` | 多线程解码 |

---

## 七、成像 / 曝光 / 补光（硬件相关）

| 参数 | 默认值 | 说明 |
|---|---|---|
| `IMAGE_EXPOSURE_MODE` | `0` | 曝光模式（0=自动） |
| `IMAGE_FIXED_EXPOSURE` | `200` | 固定曝光值 |
| `DEC_ES_EXPOSURE_METHOD` | `2` | 解码曝光方法 |
| `DEC_ES_TARGET_VALUE` | `120` | 曝光目标值 |
| `DEC_ES_TARGET_PERCENTILE` | `97` | 曝光目标百分位 |
| `DEC_ES_TARGET_ACCEPT_GAP` | `40` | 曝光目标容差 |
| `DEC_ES_MAX_EXP` | `472` | 最大曝光 |
| `DEC_ES_MAX_GAIN` | `4` | 最大增益 |
| `DEC_ES_TARGET_CONTRAST` | `145` | 曝光目标对比度 |
| `DEC_ES_IMAGE_GAMMA` | `10` | 图像 Gamma |
| `HW_EXPOSURE_SETTING_ENABLE` | `0` | 硬件曝光设置开关 |
| `HW_ES_EXPOSURE_METHOD` | `3` | 硬件曝光方法 |
| `HW_ES_TARGET_VALUE` | `0` | 硬件曝光目标值 |
| `HW_ES_TARGET_PERCENTILE` | `0` | 硬件曝光目标百分位 |
| `HW_ES_TARGET_ACCEPT_GAP` | `0` | 硬件曝光容差 |
| `HW_ES_MAX_EXP` | `0` | 硬件最大曝光 |
| `HW_ES_MAX_GAIN` | `0` | 硬件最大增益 |
| `HW_ES_IMAGE_FIXED_GAIN` | `0` | 硬件固定增益 |
| `HW_ES_IMAGE_MAX_EXP` | `0` | 硬件图像最大曝光 |
| `HW_ES_IMAGE_MAX_GAIN` | `0` | 硬件图像最大增益 |
| `HW_ES_FRAME_RATE` | `0` | 硬件帧率 |
| `HW_ES_CONFORM_IMAGE` | `0` | 硬件图像校准 |
| `HW_ES_CONFORM_TRIES` | `0` | 硬件校准尝试次数 |
| `HW_ES_SPECULAR_EXCLUSION` | `0` | 镜面反射排除 |
| `HW_ES_SPECULAR_SAT` | `0` | 镜面反射饱和度 |
| `HW_ES_SPECULAR_LIMIT` | `0` | 镜面反射限制 |
| `HW_ES_FIXED_EXP` | `0` | 硬件固定曝光 |
| `HW_ES_FIXED_GAIN` | `0` | 硬件固定增益 |
| `HW_ES_FIXED_FRAME_RATE` | `0` | 硬件固定帧率 |
| `HW_AEC_MAX_EXP_TIME` | `500` | 硬件自动曝光最大时长 |
| `HW_AEC_MAX_EXP_TIME_FINAL` | `0` | 硬件自动曝光最终最大时长 |
| `HW_AEC_MAX_GAIN` | `0` | 硬件自动曝光最大增益 |
| `HW_AEC_LUMA_TARGET` | `0` | 硬件自动曝光亮度目标 |
| `HW_AEC_LED_POWER_LEVEL` | `0` | 硬件自动曝光 LED 功率 |
| `DEC_ILLUM_POWER_LEVEL` | `10` | 补光功率等级 |
| `DEC_PICKLIST_AIM_MODE` | `0` | 瞄准模式 |
| `DEC_PICKLIST_AIM_DELAY` | `0` | 瞄准延迟 |
| `DEC_MIN_ES_MAX_EXP` | `15` | 最小曝光上限 |
| `DEC_MAX_ES_MAX_EXP` | `30` | 最大曝光上限 |
| `DEC_MIN_ES_MAX_GAIN` | `3` | 最小增益上限 |
| `DEC_MAX_ES_MAX_GAIN` | `7` | 最大增益上限 |
| `DEC_ADJUST_ES_MAX_EXP` | `200` | 曝光上限调整 |
| `LIMIT_MAX_EXP_THRESHOLD` | `1` | 最大曝光阈值限制 |
| `LIMIT_MAX_EXP_THRESHOLD_LEVEL1` | `400` | 阈值等级 1 |
| `LIMIT_MAX_EXP_THRESHOLD_LEVEL2` | `230` | 阈值等级 2 |
| `AIMER_AROUND_CIRCLE_X` | `-1` | 瞄准圈中心 X |
| `AIMER_AROUND_CIRCLE_Y` | `-1` | 瞄准圈中心 Y |
| `AIMER_AROUND_CIRCLE_R` | `12` | 瞄准圈半径 |

---

## 八、图像预处理 / 低对比度增强

| 参数 | 默认值 | 说明 |
|---|---|---|
| `IMAGE_CONTRAST_LEVEL` | `15` | 对比度等级 |
| `LOW_CONTRAST_IMPROVED` | `5` | 低对比度增强等级 |
| `LOW_CONTRAST_IMPROVED_ALGORITHM` | `0` | 低对比度增强算法 |
| `IMG_PREPROCESSING_ENABLE` | `0` | 图像预处理开关 |
| `IMG_PREPROCESSING_MODE` | `0` | 预处理模式 |
| `IMG_EQUALIZE_SENSITIVITY` | `5` | 直方图均衡灵敏度 |
| `IMG_SMOOTH_BLOCK_SIZE_X` | `3` | 平滑核宽 |
| `IMG_SMOOTH_BLOCK_SIZE_Y` | `3` | 平滑核高 |
| `IMG_SHARPEN_BLOCK_SIZE_X` | `3` | 锐化核宽 |
| `IMG_SHARPEN_BLOCK_SIZE_Y` | `3` | 锐化核高 |
| `IMG_MORPHOLOGY_OPERATION` | `0` | 形态学操作类型 |
| `IMG_MORPHOLOGY_SHAPE` | `0` | 形态学核形状 |
| `IMG_MORPH_KERNEK_SIZE_X` | `2` | 形态学核宽 |
| `IMG_MORPH_KERNEK_SIZE_Y` | `2` | 形态学核高 |
| `IMG_PREPROCESSING_SAVE` | `0` | 是否保存预处理图像 |

---

## 九、OCR

| 参数 | 默认值 | 说明 |
|---|---|---|
| `DEC_OCR_MODE` | `0` | OCR 模式（0=关闭） |
| `DEC_OCR_TEMPLATE` | `0` | OCR 模板 |
| `DEC_OCR_USER_TEMPLATE` | `137777777777777777770` | 用户 OCR 模板 |
| `OCR_USER_TEMPLATE_CONFIG` | 空 | 用户 OCR 模板配置 |

---

## 十、引擎与其他

| 参数 | 默认值 | 说明 |
|---|---|---|
| `SCANNER_ENGINE_TYPE_SELECT` | `0` | 扫描引擎类型选择 |
| `SCANNER_INTERNAL_CAMERA_ID` | `0` | 使用的内部摄像头 ID |
| `GOOD_READ_BEEP_ENABLE` | `2` | 成功提示音模式 |
| `GOOD_READ_VIBRATE_ENABLE` | `0` | 成功震动 |
| `GOOD_READ_BEEP_AUDIO_FILE` | 空 | 自定义提示音文件 |
| `SEND_GOOD_READ_BEEP_ENABLE` | `0` | 是否发送提示音事件 |
| `SEND_GOOD_READ_VIBRATE_ENABLE` | `0` | 是否发送震动事件 |
| `SPECIFIC_CODE_GS` | `0` | 特殊 GS 字符处理 |
| `C128_OUT_OF_SPEC` | `0` | Code 128 超规格处理 |
| `C128_BKN_ENABLE` | `1` | Code 128 高级子选项（BKN） |
| `C128_BKN_WORD_MAX` | `1` | BKN 单词最大数 |
| `C128_BKN_BC_MAX` | `2` | BKN 条码最大数 |
| `C39_BKN_ENABLE` | `0` | Code 39 高级子选项（BKN） |
| `C39_BKN_WORD_MAX` | `1` | BKN 单词最大数 |
| `C39_BKN_BC_MAX` | `2` | BKN 条码最大数 |
| `DEC_USE_DISTANCE_MAP` | `52` | 解码距离图（内部算法参数） |
| `DEC_USE_MLD` | `52` | MLD 算法参数（内部） |

---

## 附：默认开启的码制速览

- **1D**：Code 39、Code 128（含 GS1-128、ISBT 128）、Interleaved 2 of 5、Codabar、UPC-A、EAN-13、EAN-8
- **2D**：QR Code、Data Matrix、PDF417、Aztec、MaxiCode
