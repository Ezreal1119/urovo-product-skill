# Skill Memories

## Memory mem_ebb1a2a45a93aa0e

- Kind: fact
- Created-By-Email: ai_patrick@urovo.com
- Created: 2026-08-19T11:08:05+08:00
- Updated: 2026-08-19T11:08:05+08:00

### Content

RT40 的 SQ47Pro 现已停产，不再生产。SQ47S 计划于 2027 年通过固件更新升级至 Android 16。

## Memory mem_ede6beec004cd8ee

- Kind: fact
- Created-By-Email: ai_patrick@urovo.com
- Created: 2026-08-24T19:08:40+08:00
- Updated: 2026-08-24T19:08:40+08:00

### Content

### UROVO RFID 协议代际：Gen2X 与 Gen2 的区别

- Gen2X 可以读得更快、更远、更灵敏。
- 注意：Gen2X 需要 Reader（读写器）和 RFID Tag（标签）都支持 Gen2X 才能发挥该优势。
- 产品示例：M730 为 Gen2；M830 为 Gen2X。

## Memory mem_fd4d1f4c1486405c

- Kind: fact
- Created-By-Email: ai_patrick@urovo.com
- Created: 2026-09-03T17:40:21+08:00
- Updated: 2026-09-03T17:40:21+08:00

### Content

UROVO i5300L 具有 RoHS 认证。此前本地产品资料台账未收录该型号的 RoHS 记录（资料库中 RoHS 仅见于老款 i9000S 印度版历史条目），经用户于 2026-09-03 明确确认：i5300L 具备 RoHS 认证。今后回答 i5300L 认证类问题时，可将 RoHS 列为已确认认证项。

## Memory mem_e4f0b240492247f7

- Kind: correction
- Created-By-Email: ai_patrick@urovo.com
- Created: 2026-09-04T18:06:23+08:00
- Updated: 2026-09-04T18:06:23+08:00

### Content

DT630 自 2026-03-18 起已取消正面 NFC 感应，出货版本仅保留背面 NFC 天线。此前用户手册（如 DT630-User_Guide_20251126）中「NFC 开关开启时将卡片/标签放在设备正面天线感应」的表述已不再适用于当前出货版本，引用手册表述时需以实际出货配置为准。凡涉及「设备须能在正面/顶部感应 NFC 卡」（如招投标条款 2.3(ii) 类）的选型场景，DT630 不再满足正面感应要求，不应推荐其投标正面 NFC 场景；可改用 DT610/DT610 Pro（屏内/双面 NFC）或其他确认仍支持正面 NFC 的机型。

## Memory mem_68f5649141f19167

- Kind: correction
- Created-By-Email: ai_patrick@urovo.com
- Created: 2026-09-08T16:49:15+08:00
- Updated: 2026-09-08T16:49:15+08:00

### Content

### U2S 无 GPS 定位功能

U2S 设备没有 GPS 定位功能（用户确认），对外不应承诺支持 GPS/GNSS 定位。

### 与本地资料的矛盾（记录以便溯源）

- U2S 官方规格书（SPEC 20260526）的通信栏只列 Bluetooth 与 Wi-Fi，**未列出 GPS**；
- 但 U2S 官方彩页（20260526）与产品资料曾标注 "GPS: GPS, A-GPS, BeiDou, GLONASS, Galileo"；
- 两者存在矛盾。现以"U2S 无 GPS"为准；若需对外承诺定位能力，请以实测或新版规格书核实后再定。

## Memory mem_f16b38cba1a24c5a

- Kind: field_note
- Created-By-Email: ai_patrick@urovo.com
- Created: 2026-09-09T11:08:27+08:00
- Updated: 2026-09-09T11:43:49+08:00

### Content

i9600正在开发 Android 15 版本，该版本主控芯片采用联发科 MediaTek MT8786，内部型号为SQ69BX（金融版本，不含GMS）。现有在售 Android 13 版本（SQ69D/SQ69K）为 MTK MT8766（规格书可选四核/八核 A53 2.0GHz）。此条为用户提供的研发进度信息：Android 15 + MT8786 属新平台配置，与现售 A13/MT8766 平台不同，对外口径以规格书为准。

## Memory mem_d8914edf6900b797

- Kind: field_note
- Created-By-Email: ai_patrick@urovo.com
- Created: 2026-09-09T12:12:59+08:00
- Updated: 2026-09-09T12:12:59+08:00

### Content

UPad（内部型号 SQ92P）Type-C/USB 接口分工与充电实测（工程档口径）
数据来源：用户 2026-09 提供的 UPad 接口/充电实测工程档（附 4 张图：Type-C 口侧视特写、整机、扫描头、商超/柜台场景，无额外文字规格）。该档比对外规格书更细，回答 UPad 接口/充电问题以此为准。

- USB 版本：底部 Type-C = USB 3.1（高速口）；顶部、右侧 Type-C = USB 2.0。与规格书（2×USB-C 2.0 + 1×USB 3.1 Gen 1）一致。
- PC 数据传输：仅底部 Type-C 支持（USB3.1，priority 最高）；顶部/右侧 Type-C 与 POGO 触点均为 "no PC data transfer"，只支持 OTG 外设（U盘/键鼠等 host 应用），不能连 PC 传数据。注意：不能把规格书 "All interface support OTG" 等同于"三个口都能连电脑传数据"。
- 快充：三个 Type-C 全部支持 PD + QC 快充；POGO 触点仅支持 QC。标配适配器 18W = 9V/2A。
- 充电规则：关机也可充电，任意口皆可；同一时间仅允许一个口在充电，先插入者优先；慢充中插入快充源会自动切换为快充；快充中再插入其它口不切换。
- 并发规则：最多 4 个 OTG 外设同时工作；底部口连 PC 时，其它口的 OTG 全部禁用。
- 实测充电时长（1%→100%）：5V2A ≈ 4h09m；9V2A ≈ 2h31m。
- 续航实测口径：WiFi + 320nit 常亮 + 最大音量 + 3 秒扫一次 ≈ 9.68h。

## Memory mem_141aefa5dc9d8e4c

- Kind: correction
- Created-By-Email: ai_patrick@urovo.com
- Created: 2026-09-10T11:20:40+08:00
- Updated: 2026-09-10T11:20:40+08:00

### Content

### CT58C（SQ58C）南美频段状态更新：已基本研发完成，可以下单

- **原口径**（CT58 系列出货状态表 2026-08-10 版）：CT58C（SQ58C）标注"北美、南美不适用"，并注明"南美频段正在研发中，目前只能出不带 SIM 的"；CT58S 不出南美。
- **用户最新确认口径（本次会话提供，晚于上述 2026-08-10 版资料）**：南美频段**基本研发完了，目前可以下单**（即可接南美订单，含带 SIM 版本）。
- 回答 CT58C 在南美（如哥伦比亚等拉美市场）能否出货/使用时，**以本口径为准**，不要再引用"南美频段正在研发中、只能出不带 SIM"的旧表述。
- 注意事项：若需对外承诺具体频段覆盖范围（拉美口径为 LTE B1/B2/B3/B4/B5/B7/B28/B38/B40/B41/B55）或当地入网/运营商认证、GMS 认证状态，仍应以 CT58C 南美版本的最终频段清单与认证资料核实后再承诺。

## Memory mem_cf1a370e6ca46f5a

- Kind: fact
- Created-By-Email: ai_patrick@urovo.com
- Created: 2026-09-10T11:49:04+08:00
- Updated: 2026-09-10T11:49:04+08:00

### Content

### Understanding NFC（NFC 卡种类、用途，及我们设备的 NFC 支持范围）

#### 1. 不同的 NFC 卡种类

- MIFARE Ultralight：最轻量的纯信息卡，最普通的 NFC 标签，用来快速识别身份或者其他信息。
- MIFARE Classic：经典 NFC 卡，可读可写有身份。可以用来做简单的门禁卡、储值卡。
- MIFARE DESFire：最智能的芯片卡，可读可写有身份。可以用来做高安全的门禁卡、储值卡。
- EMV Contactless：支付芯片卡。

#### 2. 不同的 NFC 卡用途

- TYPE_2：最简单的 NFC 标签，如 NTAG → MIFARE Ultralight；TYPE_A 通信方式。
- TYPE_4：MIFARE DESFire 卡，如高级门禁卡、会员卡，需要用 APDU 进行交互使用 → MIFARE DESFire；TYPE_A（通常的 NFC 智能卡）；TYPE_B（政府相关的证件）。
- TYPE_1 也是 NFC 标签，但是现在很少见了；TYPE_3 是指日本专用；TYPE_5 是远距离 NFC 标签。

#### Note：我们设备的 NFC 支持能力

- 我们的设备 NFC 一般支持读取 TYPE_2 和 TYPE_4；TYPE_3 和 TYPE_5 新项目支持；TYPE_1 不支持。

## Memory mem_4e96f152003b373c

- Kind: fact
- Created-By-Email: ai_patrick@urovo.com
- Created: 2026-09-11T16:19:20+08:00
- Updated: 2026-09-11T16:19:20+08:00

### Content

### UROVO P8100P 5G（SQ83S）补充确认参数（用户技术反馈，2026-09-11）

本条为用户提供的真实技术反馈，用于补齐本地资料缺失项；与本地资料冲突处以此为准，涉及对外承诺时仍建议核对正式规格书/研发口径。

- **显示屏**：带 **LED 背光的 LCD** 显示屏；采用 **康宁（Corning）FHD 高清屏**（对应规格书 10.1"、1200×1920 FHD / 欧洲手册写作 1920×1200，超高灵敏度电容触摸、多点触控、支持手套与湿手）。原规格书与彩页均未标注面板类型、背光方式与康宁信息。
- **网络制式**：**明确支持 HSPA / HSPA+**（此前本地资料只有 WCDMA B1/B2/B4/B5/B8，全库无 HSPA 字样）。
- **后置摄像头**：**1300 万像素，带自动对焦（AF）**；前置 5MP 定焦。（与规格书 Camera 栏一致。）
- **Android 更新支持期限**：**可更新支持到 Android 16**；**产品计划（生命周期）到 2028 年**。原规格书仅写 Android 13 且无 Upgradable 字段，产品路线图不含平板，故此为用户口径补充。
- **标配充电器**：最大功率 **18W**，输出档位 **5V/3A、9V/2A、12V/1.5A（最大 18W）**；品牌 **华錦电子**。该充电器即为平板所支持的最高快充功率（18W）。原规格书仅写「Type-C 数据线 + QC 适配器」，无品牌/型号/输出参数。

## Memory mem_e71b6ac2deb2b649

- Kind: fact
- Created-By-Email: ai_patrick@urovo.com
- Created: 2026-09-14T10:10:59+08:00
- Updated: 2026-09-14T10:10:59+08:00

### Content

### K388 Pro 存储颗粒为 UFS（用户确认）

- K388 Pro（项目名 K388PRO，高通 SM6225，4+64，Android 14）的存储颗粒为 **UFS**。
- 该口径由用户在本会话中明确确认。本地官方资料（规格书 2025-09-25、彩页、报价表）与内部型号·内存表**只记录容量 4+64，未标注存储类型**；全库检索 UFS / eMMC / uMCP / eMCP 均无 K388 Pro 命中，故此前无法判定，现以用户确认口径为准。
- 今后回答 K388 Pro（或 K388PRO）存储类型问题时，按 **UFS** 回答；如需对外书面承诺仍建议以研发/BOM 复核为准。
- 相关已知口径：**uMCP = RAM + UFS，eMCP = RAM + eMMC**，两者封装不同、刷机包不可混用。按本条，K388 Pro 对应 uMCP 类固件包。

## Memory mem_bfaf2a98f8cbb794

- Kind: fact
- Created-By-Email: ai_patrick@urovo.com
- Created: 2026-09-17T12:07:00+08:00
- Updated: 2026-09-17T12:07:00+08:00

### Content

### 各 PDA 项目安兔兔（AnTuTu）跑分（用户提供口径，2026-09）

| 内部型号       | 对应产品                                    | AnTuTu 跑分 |
| -------------- | ------------------------------------------- | ----------- |
| SQ47S          | RT40S                                       | 24 万       |
| SQ53S / SQ53ST | DT50S（4G 血统，Product Hub 按 DT50S 路由） | 33 万       |
| SQ66           | DT66（Android 13 版本）                     | 56 万       |
| SQ83           | P8100 系列                                  | 24 万       |
| SQ83A          | P8100 系列                                  | 25 万       |
| SQ83S          | P8100P 5G                                   | 45 万       |
| SQ83S          | P8100P 5G                                   | 62 万       |

#### 使用与冲突说明

- 本条为用户明确提供的跑分口径，回答上述型号的 AnTuTu 跑分问题时以此为准。
- **填补了此前的资料空缺**：此前 Vault 中 DT66（SQ66）、RT40S（SQ47S）全库无 AnTuTu 记录，无法做跑分对比；现可回答。
- **修正/印证了此前的口径冲突**：
  - SQ53ST 此前存在冲突值（内部型号表与配件指南写 19W+，对战卡写 330K）。本条的 **33 万 = 330K**，与对战卡一致，应以 33 万为准。
  - SQ47S（RT40S）此前无记录，现为 **24 万**。
- **仍存在的相关冲突（本条未覆盖）**：DT610 / DT610 Pro（SQ610 / SQ610Pro）规格书为 1,114,080，配件指南与内部型号表按 FP1（2.0GHz）460K+ / FP4（2.9GHz）850K+ 两档给出；CT48C 存在 250K / 200K+ / 20W+ 三个来源值。这些型号本条未涉及，仍按原冲突提示处理。
- 跑分对比时需注意 AnTuTu 版本与内存配置差异，不同版本/配置不可直接横比。

## Memory mem_3156b1e47c0d4736

- Kind: fact
- Created-By-Email: ai_patrick@urovo.com
- Created: 2026-09-17T12:09:22+08:00
- Updated: 2026-09-17T12:09:22+08:00

### Content

### SQ47S（RT40S）AnTuTu PVT1 跑分测试报告

- **产品/项目**：SQ47S（Product Hub 按 RT40S 系列路由）
- **测试机版本**：SQ47S_WE**DS**R01_U_240227_02；样机数量 1；设备 ID 47202312151810；测试人 何德鑫；完成时间 **2024-02-28**
- **测试工具与方法**：安兔兔 **V10.2.1**（"安兔兔评测" + "安兔兔评测3D"）；两台设备开启 WLAN 并连接同一 AP 后运行跑分
- **测试机 SQ47S 平均总分：243,491.6（≈24 万）** —— 5 次有效值：242,216 / 243,457 / 243,266 / 243,976 / 244,543
  - CPU 88,360.2 ｜ GPU 34,996.4 ｜ UX 55,501.6 ｜ MEM 64,633.4
- **对比机 斑马 MC3300（版本 02-13-15.00-ON-U13-STD）平均总分：180,462.4** —— 5 次：189,454 / 181,054 / 173,454 / 178,205 / 180,145
- **测试结论**：SQ47S 优于斑马 MC3300，两者相差 **25.8%**

#### 使用说明与数据质量提示

- 本条与《各 PDA 项目安兔兔跑分》中 "SQ47S = 24 万" 互为印证：24 万即来自本次 PVT1 测试的平均分 243,491.6。
- **本次使用 AnTuTu V10.2.1**，而 DT630（950,707）、DT50 Pro（418,013）、SR5750（308,016）等标注的是 **V11**；跨版本分值不可直接横比。
- 原表存在录入/公式问题：L22–L25 均引用 L21（本应各自取 AVERAGE(B22:F22) 等）；L21 的 AVERAGE(B21:K21) 实际只覆盖 B:F。对比机 D22 的 CPU 值 640,481 疑似多一位，其余 4 次约 63,000–64,848。引用分项时应以原始 5 次数值为准。
- 来源：SQ47S项目PVT1安兔兔跑分结果模板.xlsx（PVT1 阶段测试报告）。

## Memory mem_a90f6cbe0600f5a2

- Kind: correction
- Created-By-Email: jk@urovo.com
- Created: 2026-08-12T11:26:30+08:00
- Updated: 2026-08-12T11:26:30+08:00

### Content

### DT50 Pro 最高可升级到 Android 21

DT50 Pro（DT50-Pro Edition，内部代号 SQ53Pro）实际最高可升级到 Android 21。尽管 2026-06-30 版产品规格书标注为 Upgradable to Android 20，用户实测/官方确认为 Android 21。回答相关问题时以 Android 21 为准，并注明与规格书（Android 20）的差异。

## Memory mem_515aeff58d5f2b4a

- Kind: fact
- Created-By-Email: patrick@urovo.com
- Created: 2026-08-12T20:01:21+08:00
- Updated: 2026-08-12T20:01:21+08:00

### Content

### 4G LTE 频段（按地区）

| 地区                             | 4G LTE 频段                                                                |
| -------------------------------- | -------------------------------------------------------------------------- |
| Europe（欧洲）                   | B1, B3, B7, B8, B20, B28, B32, B38, B46                                    |
| Russia（俄罗斯）                 | B1, B3, B7, B20, B38                                                       |
| Japan（日本）                    | B1, B3, B8, B11, B18, B19, B21, B26, B28, B41, B42                         |
| North America（北美）            | B2, B4, B5, B7, B12, B13, B14, B25, B26, B29, B30, B41, B46, B48, B66, B71 |
| China（中国）                    | B1, B3, B5, B8, B34, B39, B40, B41                                         |
| South Korea（韩国）              | B1, B3, B5, B7, B8                                                         |
| MEA（中东及非洲）                | B1, B3, B8, B20, B28, B41                                                  |
| Australia/SEA（澳大利亚/东南亚） | B1, B3, B5, B7, B28, B40                                                   |
| Latin America（拉丁美洲）        | B1, B2, B3, B4, B5, B7, B28, B38, B40, B41, B55                            |

### Note: 如何判断某个产品的频段配置是否支持某地区？

- 需要判断该产品的频段配置是否覆盖了特定地区所有的频段。（不同地区的频段上面有显示）
  (详细的各个国家的频段信息，可以在这个网站查看`https://www.kimovil.com/en/frequency-checker/CA`)

## Memory mem_c3bc7aa5f1944eca

- Kind: field_note
- Created-By-Email: patrick@urovo.com
- Created: 2026-08-12T20:58:09+08:00
- Updated: 2026-08-12T20:58:09+08:00

### Content

### 为POS客户开发支付应用App需提前确认的技术问题

为 POS 客户开发交易App前，需提前与客户确认以下技术问题：

1. **网络通讯协议**：socket/http/https？是否需要 SSL 通讯认证（如需请提供相关证书文件）——描述交易 App 与支付后台之间的网络通信方式。
2. **通讯报文规范**：如 ISO8583 规范——描述交易 App 与支付后台通信时的协议报文规范。
3. **功能清单与示例报文**：需要实现哪些功能（如交易、取款、退款等），每种功能都应有对应示例报文，用于开发调试。
4. **测试环境**：是否有测试环境，供开发过程中及时调试。
5. **应用 UI 要求**：交易 App 的 UI 是否有具体要求或参考样式。

## Memory mem_b19b3798e1a929b9

- Kind: field_note
- Created-By-Email: patrick@urovo.com
- Created: 2026-08-12T22:17:06+08:00
- Updated: 2026-08-12T22:17:06+08:00

### Content

### POS机五种写密钥的情况

1. **客户生产前把密钥给到我们 [DUKPT / MK/SK]**：我们利用我们的 KMS 在产线上，利用 SNTool 触发设备进行密钥下载（通过内网下载），然后通过 SE 的 API 写入安全芯片中。
2. **客户生产后把密钥给到我们 [DUKPT / MK/SK]**：客户的 APP 用 Intent 触发我们内置的 KMS 相关 APP，通过公网进行密钥下载，然后通过 SE 的 API 写入安全芯片中。
3. **私有化部署我们的 KMS 系统**：客户的 APP 用 Intent 触发密钥通过公网下载，然后通过 SE 的 API 写入安全芯片中。
4. **卖 KLD 给客户**：客户自行在 KLD 在当地 PCI 认证的安全房自己注入密钥。【注：我们的 KLD 主要是 i2000，通过了 PCI 安全认证】
5. **完全是自己的 KMS 系统以及自己的密钥通信协议**：完全不需要我们的参与，我们只提供底层的 SE 接口【如 OPAY】。

## Memory mem_83e35257aa5412b0

- Kind: field_note
- Created-By-Email: patrick@urovo.com
- Created: 2026-08-12T22:48:08+08:00
- Updated: 2026-08-12T22:48:08+08:00

### Content

### POS 小票打印和标签打印的区别

- 标签打印需要打印机带**间隙传感器**，小票打印则不需要。
- 目前只有 **i9200 行业版（SQ68P）**支持标签打印。

## Memory mem_daa4a36444b30cf6

- Kind: field_note
- Created-By-Email: patrick@urovo.com
- Created: 2026-08-12T22:54:01+08:00
- Updated: 2026-09-07T09:40:46+08:00

### Content

### Mifare/智能NFC卡 与 金融非接触卡（PICC/Contactless Payment）的区别及开发方式

#### MIFARE DESFire（智能NFC，如会员卡、门禁卡、交通卡等）

- Mifare 卡（俗称 NFC 卡 / 智能非接触卡）：通常用于门禁卡等场景；智能 NFC 卡（如 MIFARE DESFire）多用于会员卡、门禁卡、交通卡等。
- 对于智能 NFC 卡，利用 Android Standard SDK 里面的 NfcAdapter 即可（即安卓通用 SDK 的 NFC 模块，android.nfc.NfcManager），**不需要**集成 Urovo 的私有 SDK 进行二次开发。第三方应用通常可以用安卓通用 SDK 的 NFC 模块去调用（android.nfc.NfcManager）；softPOS 一般就是这样调用 NFC 模块去读取非接触金融卡。即第三方应用**不需要**根据厂商 SDK 对设备 NFC 模块进行功能二次开发。
- 所以第三方软件使用 NFC 的时候都可以直接使用。

#### Contactless Payment Card（非接触金融银行卡）

- 金融非接触卡（俗称 PICC / Contactless）：应用需要继承厂商的 SDK 进行设备 NFC 模块的功能调用。相比安卓通用 SDK 的 NFC framework，我们 SDK 的 **PiccManager** 的金融支付更加规范，可支持各种金融认证。支付应用开发一般都使用我们 SDK 的 PiccManager。
- 对于非基础的金融银行卡，必须要用私有 SDK 里面的 PiccManager 去做集成和二次开发，因为标准的 NFC 是没有 EMV 认证的，没法用于金融支付，我们做 EMV 认证都是基于 PiccManager 去做的。

**Note**：原则上我们的产品都支持读取 Mifare 卡，可通过标准 NFC Framework 开发，也可通过我们 SDK 的 PiccManager 模块开发；但世界上的 Mifare 卡种类太多，实际是否支持需要我方或用户实测。

## Memory mem_c756e55fac0a2794

- Kind: fact
- Created-By-Email: patrick@urovo.com
- Created: 2026-08-14T19:37:43+08:00
- Updated: 2026-08-14T19:37:43+08:00

### Content

### CT58S 停产，后续出货改为 CT58C

CT58S 型号以后都不再出货（已停产/停止供货），后续出货型号为 **CT58C**。回答 CT58S 相关问题时，需说明该型号已不出货，并以 CT58C 作为当前出货型号。

## Memory mem_a3958cc314e1b69c

- Kind: fact
- Created-By-Email: patrick@urovo.com
- Created: 2026-08-14T20:04:14+08:00
- Updated: 2026-08-14T20:04:14+08:00

### Content

### DT66 的 Android 13 / Android 15 版本（SQ66 / SQ66V）硬件相同，仅固件升级

- **DT66 的 Android 13 版本** 即 **SQ66**。
- **DT66 的 Android 15 版本** 即 **SQ66V**。
- SQ66 与 SQ66V 两个版本的**硬件完全一样**，只是**固件上有升级**（Android 13 → Android 15）。
- 回答 DT66、SQ66、SQ66V 相关问题时，需说明二者硬件一致、SQ66V 为 SQ66 的 Android 15 固件升级版。

## Memory mem_5038d16c6162eaac

- Kind: field_note
- Created-By-Email: patrick@urovo.com
- Created: 2026-08-14T22:06:24+08:00
- Updated: 2026-09-07T09:23:01+08:00

### Content

### MDM 管理设备的方式:三种架构类型 + 四种 Provisioning / 集成方式

#### 一、MDM 的三种架构类型(2026-09 补充)

1. **私有协议型(如 UROVO UMS)**
   - 用自己的 Server 和 DPC,使用自己的协议。
   - 能力来源于 Private SDK 或 System Signature。
   - 不经过 Google(对应下文"其他 MDM 集成方式"的第 3、4 种)。
2. **DO(Device Owner)型**
   - 仍基于 Android Enterprise(AE)的标准化模型,但是自己实现 Server 和 DPC。
   - 底层还是 Device Owner(DevicePolicyManager)。
   - 可以不经过 Google;但如果需要接入 Managed Play Store(托管 Google Play),仍要接入 Google。
3. **AE(Android Enterprise)型**
   - 完全接入 Google,利用 Google 的 Restful API 与 Google 进行通信。
   - Server 和 DPC 都用 Google 的。
   - 底层能力也是 Device Owner(DevicePolicyManager)。

Note(理解用对应关系):三种类型是对 MDM 架构的顶层归纳;下文的"四种方式"是更具体的 Provisioning / 集成路径。第 1 类(私有协议型)通过"其他 MDM 集成方式"的第 3/4 种落地,完全不经过 Google;第 2、3 类(DO / AE)通过 Android Enterprise Provisioning(QR / Zero-touch)落地,差异在于 Server 与 DPC 是自建还是用 Google 的、以及是否接入 Managed Google Play。

#### 二、两种主要的 Android Enterprise Provisioning 方式

1. **QR Code Provisioning**
   - Provisioning 方式:MDM 的 Admin 在 Console 中生成 Provision QR Code;设备开机 Wizard 的第一个页面 Tap 7 下触发二维码扫描。
   - QR Code 包括 DPC 的下载地址,以及相关的配置信息(可能包括 GroupID 或其他系统配置)。
   - DPC 下载好之后,会被系统设置为 DO(Device Owner)。
   - 下载 DPC 方式有两种:
     - MDM 自己的 CDN 服务器下载,不需要经过 Google(如 SOTI 的 `http://soti.net/apk/ae2`)。
     - MDM 先上传 DPC 到 Managed Google Play Store,然后下载地址用 Google 提供的(如 AirWatch/Workspace ONE 的 `https://play.google.com/managed/downloadManagingApp?identifier=hub`)。

2. **Zero-touch Provisioning**
   - Provisioning 方式:Reseller 提前在 Google Zero-touch Platform 给客户企业注册;Reseller 需要和 MDM 进行配置确认,以及和用户确认设备 SN;最后把 MDM 的配置和设备 SN List 绑定在用户企业下。
   - 效果:设备开机向导一联网,则自动下载 DPC 并完成配置(类似 QR Code Provisioning 但不需要 QR Code 扫描步骤);DPC 之后会被系统设置为 DO(Device Owner)。
   - Note:
     - 只有 Reseller 才能申请 Google Zero-touch Platform;UROVO 有自己的 Zero-touch 账号,可以给客户创建 Customer 账号进行设备绑定,帮助用户使用 Zero-touch 做 Provisioning。
     - 关键:UROVO PDA 设备硬件上支持 Zero-touch(AER 认证会测这个)。

#### 三、Note:Device Owner 能力

Device Owner 可以拥有调用 Android Enterprise(DevicePolicyManager)API 的权限(如 setCameraDisabled()、wipeData()、DISALLOW_FACTORY_RESET 等),这些都是 Google 定义的 Device Owner 标准能力。

#### 四、其他 MDM 集成方式(完全不需要经过 Google)

3. **Platform signed + Pre-installed**:可以获得读写 Settings 的能力(不需要具备 DO 的能力)。
4. **SDK + Pre-installed**:可以获得所有 SDK 提供的能力——要么 MDM 根据厂商 SDK 进行二次开发,要么厂商根据 MDM 的接口需求进行 SDK 开发。

## Memory mem_448961a223dfb350

- Kind: field_note
- Created-By-Email: patrick@urovo.com
- Created: 2026-08-15T17:09:31+08:00
- Updated: 2026-08-15T17:09:31+08:00

### Content

### Urovo OEMConfig 概览与 MDM 集成逻辑

#### OEM 职责

- OEM 按 Google OEMConfig 标准开发 OEMConfig 应用，并通过 Google 生态发布。
- OEMConfig 应用集成 OEM 私有 SDK，因此可访问 OEM 专属的设备管理能力，包括标准 Android Enterprise API 之外可能无法获得的硬件与系统级控制。
- Urovo OEMConfig 应用包名：**com.urovo.oemconfigs**；也可在 Managed Google Play 中搜索 "Urovo OEMConfig" 找到。
- Urovo 将 OEMConfig 应用发布到 Managed Google Play，应用的包名与 Managed Configuration Schema 通过 Google 的 Android Enterprise / Managed Google Play 基础设施提供给受支持的 MDM 平台，使其能暴露并使用 OEM 定义的配置项。

#### MDM 管理员工作流（部署 Urovo OEMConfig 的典型流程）

1. 从 MDM 平台打开 Managed Google Play。
2. 搜索并选择 Urovo OEMConfig 应用。
3. 按 MDM 要求审批/添加应用到企业环境。
4. 为 OEMConfig 应用启用 Managed App Configuration。
5. MDM 通过 Android Enterprise / Managed Google Play 集成获取应用的包名与 OEM 定义的 Managed Configuration Schema。
6. MDM 在其管理控制台中展示可用的 OEMConfig 选项。
7. 管理员配置所需设备设置。
8. 管理员将应用与配置分配部署到目标设备。

#### 设备侧配置流

MDM Server → Android Enterprise 管理基础设施 → 设备上的 Device Policy Controller (DPC) → Android Managed Configurations 机制 → Urovo OEMConfig 应用 → Urovo 私有 SDK / 系统接口 → 设备硬件与系统设置

- DPC 接收与 Urovo OEMConfig 包关联的 managed application configuration，并通过 Android 标准 Managed Configurations 机制下发。
- Urovo OEMConfig 应用读取为其包提供的 managed configuration，解析 OEM 定义的配置值，转换为对 Urovo 私有 SDK 或系统接口的调用。
- 这些 SDK/系统接口调用执行实际设备配置：扫描器设置、Wi-Fi 参数、NFC 状态、系统限制、应用控制、电池设置等 Urovo 专属功能。

简化形式：管理员在 MDM 中配置 OEMConfig → MDM 部署 managed configuration → DPC 接收并应用配置 → Android 将 managed configuration 暴露给 Urovo OEMConfig → Urovo OEMConfig 解析配置 → Urovo OEMConfig 调用 Urovo 私有 SDK / 系统接口 → 设备配置生效

#### 核心概念（重要）

MDM 本身无需为每个 OEM 专属功能直接集成 Urovo 私有 SDK，职责分离：

- MDM / DPC：使用标准 Android Enterprise 管理机制下发 managed application configuration。
- Urovo OEMConfig：理解 Urovo 配置 schema，将收到的配置转换为 Urovo SDK / 系统接口调用。
- Urovo 设备软件 / SDK：在设备上执行实际的硬件或系统级操作。

该架构允许不同的 Android Enterprise 兼容 MDM 平台通过同一个 OEMConfig 应用管理 Urovo 专属功能，无需每家 MDM 厂商自行实现 Urovo 私有设备 API。

### Urovo OEMConfig 配置功能清单（26 大类）

1. **WLAN / Wi-Fi**
   - Wi-Fi 网络配置：SSID、密码、安全模式、DHCP/静态 IP、IP 地址、前缀长度、网关、DNS 1、DNS 2、隐藏 SSID、代理模式、PAC 代理、代理主机、代理端口、代理排除列表
   - Wi-Fi 白名单管理、白名单 SSID
   - Wi-Fi 诊断：5 GHz 优先模式
   - 附加 Wi-Fi 设置：Captive portal 配置、网络可用通知、网络已监测通知、Wi-Fi 频段选择、Wi-Fi 信道选择、私有 DNS 模式、私有 DNS 服务器、设备主机名、设备型号名

2. **时钟 / 日期与时间**：自动/手动时间模式、手动日期、手动时间、自动/手动时区、手动时区、时间格式、NTP 服务器、时间服务器同步间隔

3. **声音**：闹钟/媒体/铃声/通话音量；通知音、拨号音、锁屏音、触摸音、触摸振动、充电声音与振动；音量限制（锁定音量、锁定最大音量）

4. **显示**：屏幕超时、保持唤醒、字体大小、背光/亮度级别、自动亮度、自动旋转、屏幕方向、屏幕方向建议、主屏/锁屏壁纸、锁屏通知、屏保启用/禁用、屏保启动条件、屏保类型

5. **安全**：Google Play Protect、锁屏类型、锁屏密码、锁屏超时

6. **扫描器 Profile / 配置文件**：配置文件管理、配置文件下载、扫描器设置文件路径、下载目标路径；FTP 配置（用户名、密码、端口、匿名登录）

7. **高级 Wi-Fi**：Wi-Fi 省电模式、漫游阈值、漫游差值、随机 MAC 配置

8. **NFC**：启用/禁用

9. **电源**：电源动作配置

10. **通用 UI**：系统语言、禁用指定输入法、当前键盘/IME、拼写检查、指针速度

11. **无线通用**：定位启用/禁用、Wi-Fi 扫描始终可用

12. **FOTA / 系统更新**：系统更新服务、系统更新检查时间、Wi-Fi 系统更新、本地系统更新、系统更新文件

13. **可编程按键 / 按键映射**：按键映射动作、导出按键映射、导入按键映射、屏幕左键、屏幕右键、屏幕 PTT 键

14. **扫描器（详细）**
    - 通用：扫描器启用/禁用、悬浮扫描按钮、触发模式
    - 连续扫描：连续扫描模式、连续扫描超时、扫描时间间隔、多次解码、固定解码次数
    - 多码扫描：启用/禁用、每次操作扫描条码数、每次固定条码数
    - 输出模式：键盘输出、广播输出、剪贴板输出、文本框输入模式、网址识别与跳转
    - 键盘输出：键盘类型、解码音、振动、操作/结束键字符
    - 广播输出：广播 Action、字符串数据标签、字节数据标签、广播音、广播振动
    - 阅读器参数：中文编码类型、自定义编码类型、最小 1D 条码长度控制、最小 1D 条码长度、激光时长、多重校验
    - 1D 条码特性：启用/禁用、反色解码、边界检查、单图解码时间、触发瞄准模式、触发瞄准延迟
    - 补光/成像参数：补光配置、补光亮度、曝光模式、曝光增益、图像对比度
    - 取景解码：启用/禁用、取景模式、左上 X/Y 坐标、右下 X/Y 坐标
    - UDI 数据格式：启用/禁用、Token 格式、Token 分隔符、UDI 日期、UDI 类型选择
    - 基础数据格式化：条码标识符、应用标识符、应用 ID 分隔符、GS 特殊字符配置、附加格式化、前缀特殊字符、自定义前缀、后缀特殊字符、自定义后缀、自定义格式、字符替换、十六进制输出、控制字符
    - 码制设置：Aztec、Chinese 2 of 5、Codabar、Code 11、Code 128、Code 39、Code 93、Composite、Discrete 2 of 5、Data Matrix、DotCode、EAN-13、EAN-8、GS1 DataBar Family、Grid Matrix、Han Xin、Interleaved 2 of 5、Matrix 2 of 5、MaxiCode、MicroPDF417、Micro QR Code、MSI、PDF417、QR Code、Trioptic、UPC-A、UPC-E、UPC-E1、Postal Codes、UPC/EAN Extensions、DPM 解码
    - Data Matrix 高级：启用/禁用、反色模式、高级解码设置
    - QR Code 高级：启用/禁用、反色模式、高级解码设置、QR 模块、QR 区域
    - OCR：解码模式、OCR 模板、OCR 字型、OCR 字符类型、OCR 条码长度、自定义 OCR 模板
    - 扫描器特性设置：字符间延迟、回车键延迟

15. **系统功能 / 设备限制**
    - System UI 控件：状态栏下拉、左导航键、中导航键、右导航键、导航栏
    - 输入法控制：输入法控制、永久禁止 IME 激活、悬浮按钮控制、物理按键控制
    - 系统功能：Passcode 应用、自动通话录音、三指截屏、屏幕固定
    - Launcher：默认 Launcher 选择、自定义默认 Launcher
    - 硬件/接口限制：摄像头、GPS、蓝牙、音量键、锁屏、外部挂载存储、飞行模式、剪贴板、OTG 的启用/禁用
    - USB：USB 启用/禁用、USB 模式、ADB 启用/禁用

16. **APN**
    - 新增/配置 APN：APN 名称、代理、端口、用户名、密码、服务器、MMSC、MMS 代理、MMS 端口、MCC、MNC、认证类型、APN 类型、APN 协议、APN 漫游协议、Bearer、设为当前 APN
    - 按名称删除 APN

17. **应用管理**
    - 应用安装：远程 APK 下载/安装、APK 下载 URL、APK 文件名
    - 应用控制：卸载应用、设置默认 Launcher 应用、未知来源安装控制、USB 安装应用、应用初始化状态、禁用应用列表、启用应用列表

18. **应用权限管理**：按应用包名配置权限、应用签名配置、批量应用权限配置、权限状态配置、Feature 差异配置

19. **文件管理**：远程文件下载、文件名、文件 URL、目标/存储路径

20. **Kiosk**：Kiosk 模式配置、Kiosk 应用包名、Kiosk 退出密码

21. **麦克风**：禁用麦克风、通话中禁用麦克风、指定应用启用麦克风、通话中禁用麦克风传感器

22. **日志**：日志启用/禁用、主日志、内核日志、无线日志、事件日志

23. **以太网**：启用/禁用

24. **电池**
    - 电池显示与保护：电池百分比显示、高温阈值
    - 电池优化：应用包名、电池优化启用/禁用
    - 电源与充电：省电模式、智能充电模式、充电限制百分比

25. **无障碍**：手套模式启用/禁用

26. **本地网络 OTA**：本地网络 OTA 配置、本地网络 OTA 服务、主/客户端角色、系统包路径、服务器端口、自动安装

#### 高层能力归纳（产品与 MDM 视角，18 大类）

1. Wi-Fi 与网络
2. 日期与时间
3. 声音
4. 显示
5. 安全
6. NFC
7. 电源
8. 扫描器
9. 设备限制
10. APN 与蜂窝
11. 应用管理
12. 应用权限管理
13. 文件管理
14. Kiosk
15. 电池与充电
16. OTA / FOTA
17. 硬件与接口控制
18. 系统 UI 与输入控制

#### 关键 OEM 专属能力（超出标准 Android Enterprise 管理控制的重点能力）

- 高级扫描器配置与条码码制管理
- 高级 Wi-Fi 配置
- 设备硬件与系统功能限制
- 应用安装与应用控制
- 应用权限管理
- Kiosk 配置
- APN 配置
- 可编程按键 / 按键映射配置
- 高级电池与充电控制
- FOTA 与本地网络 OTA
- 日志控制
- USB、ADB、OTG、摄像头、GPS、蓝牙、NFC 等硬件控制

## Memory mem_cd7e4cb8d876e51b

- Kind: field_note
- Created-By-Email: patrick@urovo.com
- Created: 2026-08-15T17:54:43+08:00
- Updated: 2026-08-15T17:54:43+08:00

### Content

### Google Key (Attestation Key)

Google Key 也叫 Attestation Key，是 Google 为 GMS 认证设备提供的一种 Attestation 的 Key。

- Google Play Integrity 是 Google 提供的一种验证设备是否合法、运行环境是否安全的服务(API)。
- Google Play Integrity 会使用到 Google Key。很多 App（如 softPOS）会调用 Google Play Integrity API 来判断设备的运行环境是否安全。（Google 主要检查证书链是否合法；RootCert 是否为 Google DB 里面的；设备的信息是否合法，如是否 root 了）

### Google Key 注入方法：RKP 和 SNTool 注入

- POS：都是直接写入 AttestationKey 到 TEE，无 GoogleKey（重置不会消失，且 lifetime 不变）
  - Cloud 写（从云端拉取 AttestationKey 后写入 TEE）
  - UKEY 写（从云端拉取 AttestationKey 后写入 TEE）
- PDA (SQ53S/ST)：installKeyBox 是 AttestationKey 写入 TEE，不需要联网拉取 AttestationKey（重置不会消失，且 lifetime 不变）
  - installKeybox（厂测点击 GoogleKey 会把 /vendor/bin/test_keybox.xml 写进 TEE）
- PDA (K388Pro, SQ92P, SQ610, ...)：RKP（存在 rkp 包）installKeyBox 十八罗汉 GoogleKey 写入 TEE；如果使用的时候没有 AttestationKey 的话会自动 rkp 拉取 AttestationKey（GoogleKey 重置不会消失，AttestationKey 重置会消失）
  - installKeybox（adb 去进行安装）+ register（python 程序上送设备信息给 Google）

### 如何判断 Google Key 是否被注入成功

- 在 Factory Test 里面的 Device Info 里面查看
- 利用 adb shell getprop | grep google 查看
- 在 Google Play Store 里面查看设备是否为 certified

### 如何查看某个设备是否复用别的型号

- ro.build.fingerprint: Tells the actual Info that was used to register during Google Certificate

### 为什么 Google Key 有成本

- 只要做了一次 GMS 认证之后，就会从 Google 获得十万左右的 Google Key（用完需重新申请 GoogleKey）。目前我们 POS 的 Google Key 要么是 SQ57 的要么是 i9100_A13 的，也就是 20 万的量。Google Key 是越用越少的（虽然重新和 Google 申请就可以获得多的，但是如果这样 Google 就会查看出货情况，容易被发现我们套用），所以我们会进行收费来管控。

## Memory mem_db046059d720ed5c

- Kind: fact
- Created-By-Email: patrick@urovo.com
- Created: 2026-08-15T17:59:22+08:00
- Updated: 2026-08-15T17:59:22+08:00

### Content

POS机GMS认证套用情况（2025年后口径，已修正型号写法）：

目前的POS机的GMS认证基本都是套用SQ57或者i9100_A13的（POS目前我们只有SQ57和i9100_A13过了Google认证），详细套用情况如下：

- SQ57: i9100_A12, i9000S, i5300, i5300L
- i9100_A13: i9200, U100, i9600
  Note:
- 所谓套用，即是这些设备在软件层面上都伪装成实际通过了GMS认证的设备（如SQ57和i9100_A13)，这样Google Play就在软件上认为这些设备通过了GMS认证，就可以在Google Play Store中看到Google Certified。
- 之前Google查的不严可以这样套用，但是在Android 15之后Google就会严查。所以正在研发的i9600_A15就已经自己做Google认证了。

## Memory mem_bcb3805195d498e6

- Kind: field_note
- Created-By-Email: patrick@urovo.com
- Created: 2026-08-15T22:07:16+08:00
- Updated: 2026-08-15T22:07:16+08:00

### Content

### Urovo RFID 芯片（E710 / E310）配置与差异

1. Urovo 的 RFID 芯片：

- 外挂 E710：DT50P(Lite)；RFG91；FR1000；FR2000；FR7000（最高可读 15 米；FR2000 一般只读半米以内的）
- 外挂 E310：除上面外的其他设备（最高可读 1.5 米；FR2000 一般只读半米以内的）

2. E710 / E510 / E310 的主要区别：

- Signal Sensitivity：E710 是 E510 的十倍，E510 是 E310 的十倍。芯片越强，越能提高 SNR，从而读取到更微弱的有效数据，也就是读距更远。
- Tag Read Speed：E710 能读 1000 tags/second；E310 只能读 300 tags/second

## Memory mem_af62a939755f5a2f

- Kind: field_note
- Created-By-Email: patrick@urovo.com
- Created: 2026-08-16T17:52:14+08:00
- Updated: 2026-08-21T09:24:48+08:00

### Content

### 扫描头选配指南

Standard Range Scanner（标距）: 60cm for 13 mil UPC-A

- SE2030S (Urovo): Cross-Only（十字线瞄准）
- HS7 (aka. 5703; Honeywell): 包含 Cross 与 Frame 两种瞄准图案

Middle Range Scanner（中距）: 2m for 13 mil UPC-A; 10m for 100 mil UPC-A 为最远距离

- SE2030FR (Urovo)
- N6803FR (Honeywell): Aiming Dot（点状瞄准）
- SE55(00) (Zebra): Aiming Dot（点状瞄准）

Long Range Scanner（长距）: 4m for 13 mil UPC-A; 30m for 100 mil UPC-A 为最远距离

- EX30 (Honeywell): Aiming Dot（点状瞄准）
- SE5800 (Zebra): Cross（十字线瞄准）

注：

- mil 即条码中 unit 的宽度，通常用 mil + distance 描述 scanner 读距。
- DT610Pro、DT66、DT50S 支持 Middle Range Scanner；只有 RT40S 支持 Long Range Scanner (SE5800)。
- 现在主推 Urovo 自研的 SE2030S（标距）和 SE2030FR（中距）；也可支持 Honeywell 的 HS7（标距）与 N6803FR（中距）。
- 所有扫描头都基于同一个 SDK 开发，不论是否 Urovo 自研。
- DT630 使用 Urovo 自研的特殊扫描头 SE630：位于设备背面，不含激光，纯绿色 LED，对人眼友好。
- Urovo 对 DPM 读取有专门的 Urovo 自研 DPM 扫描头。
- 扫DPM的话一般需要开反白，3 \* 3mm以下的DPM需要用DPM高密扫描头进行扫描。

## Memory mem_c8c63169a50e0427

- Kind: field_note
- Created-By-Email: patrick@urovo.com
- Created: 2026-08-16T17:54:51+08:00
- Updated: 2026-08-16T17:54:51+08:00

### Content

### SCANNING 相关参数（扫码原理与参数速记）

1. Code-related:

- CODE的信息密度(Code Resolution)用mil表示: 单位条码（二维码块）的长度
- Contrast: Contrast between Dark & Light. 对比度越高越容易解码

2. Scanner-related:

- Resolution: 2D帧中的像素数
- Field of View(FoV): Horizontal / Vertical
- (Resolution, FoV, Distance) 决定 "? px/mm" (Sampling frequency)
- Frame rate(FPS): 每秒解码次数，决定扫码成功率 (e.g., FPS=60 表示每秒60次解码尝试)

3. FAQ:

- 扫码成功的前提：清晰图像
  - FPS要平衡：太高图像容易不清晰/暗，太低成功概率会下降
  - 曝光时间要平衡：太高容易模糊，太低成像不清晰/暗
  - CODE本身的对比度要高
  - 补光要适度：太强容易Overexposure降低对比度，太低条码不清晰
- 扫码成功的本质：
  - 当扫描系统的空间分辨率足以对条码的最小模块进行有效采样（通常≥3px/module）时，即可实现识别
  - 即，scanner的采样频率(Resolution, FoV, Distance)大于code的信息密度(Code Resolution)，即可实现解码
- 为什么扫码有距离下限：
  - FoV极限：太近了整个条码不完整
  - scanner本身的对焦距离下限：太近了会模糊

## Memory mem_58340650ca832651

- Kind: fact
- Created-By-Email: patrick@urovo.com
- Created: 2026-08-16T18:02:56+08:00
- Updated: 2026-08-16T18:02:56+08:00

### Content

### Google相关的概念：SMR / GMS认证 / AER认证

#### 1. SMR (Security Maintenance Release / 安全维护)

- 拿到谷歌当前发布的最新的 Security Patch（优先相同安卓版本，如果没有就用更高版本的），然后给 Google 送测。
- 谷歌每个月都会针对不同安卓版本发布 Security Patch。
- 每个安卓版本谷歌会维护三年的 Security Patch 更新，三年之后要进行 SMR 只能用更高的 Android 版本的 Security Patch 进行合入。
- 为什么要做 SMR：
  - GMS 的 EDLA 认证路径要求每三个月进行一次安全维护，至少维护 2 年。
  - AER 要求每 3 个月做一次 SMR，至少维护 5 年。
  - 如果用户有需求（如要求更新 Security Patch），那么就需要去做 SMR。

#### 2. GMS (Google认证)

- 两条认证路径，互相独立。（POS 一般被认为是行业设备，要走 EDLA；PDA 两条都可以。）
  - MADA：主要面向 C 端设备，价格相对便宜。每个安卓版本的认证截止日期为版本发布之后一年。
  - EDLA：主要面向 B 端设备。每个安卓版本的认证截止日期为版本发布之后两年。很多时候如果某个 Android 版本的 PDA 赶不上 MADA 的 GMS 认证，就需要走 EDLA 路径的 GMS 认证。（如果连 EDLA 都错过，则该产品无法通过 GMS 认证了）
  - Note: 目前只有 i9100, U2S, DT610, K388Pro, DT630 走的是 EDLA 认证，其他的都是 MADA，详细可参考 "GMS+AER认证" 表格。
- 认证地区：
  - EEA：主要是欧洲地区。
  - ROW：除欧洲之外的大多数地区。
- GMS 认证后最直接的效果（MADA/EDLA 路径都行）：
  - 能够向客户证明该设备能够适配 Google 生态系的 App。
  - 能够在 Google Play Store 里看到设备是 Google Certified（需要 Google Key；即使是套用，也能看到 certified）。
  - 能够在 https://storage.googleapis.com/play_public/supported_devices.html 看到该型号。

#### 3. AER (Android Enterprise Recommended)：谷歌 Android Enterprise 能力认证

- 此认证建立在 GMS 之上，过了 GMS 认证才能过这个。
- 认证含义：
  - Android Enterprise Provisioning: 设备满足 Google 定义的 Android Enterprise Provision 的 workflow。
  - Android Enterprise Management: 设备满足 Google 定义的 Android Enterprise 所需要支持的管理能力，如 DevicePolicyManager。
  - OEMConfig: 设备支持 Google 定义的标准的 OEMConfig 的配置下发。
- AER 认证后最直接的效果：
  - 能够向客户证明该设备能够适配 Google 定义的 Android Enterprise 的能力。
  - 能够在 https://androidenterprisepartners.withgoogle.com/devices/ 看到该型号。

## Memory mem_2e262b6736694e8b

- Kind: fact
- Created-By-Email: patrick@urovo.com
- Created: 2026-08-16T18:21:12+08:00
- Updated: 2026-08-16T18:21:12+08:00

### Content

### K388 Pro 海外版本策略

- K388 Pro 海外市场仅推 WiFi Only（无 LTE）版本。
- 也就是说，K388 Pro 的 4G（仅国内频段）版本只面向中国大陆市场；海外销售一律使用不带蜂窝的 WiFi Only 版本。
- 与本地资料交叉印证：Device & Accessories Guide 中 K388 Pro 标注为 "支持4G(仅国内频段)"，海外无具体频段清单，因此海外无 LTE 版本。

## Memory mem_0e4c93e0b077e765

- Kind: terminology
- Created-By-Email: patrick@urovo.com
- Created: 2026-08-16T18:33:36+08:00
- Updated: 2026-08-16T18:33:36+08:00

### Content

PCI-PTS（PIN Transaction Security）认证的含义（简略版）：

1. 安全防拆（Tamper）：防止 Key 受到**物理**攻击。
2. Key 和安全运算都存在于 SE（安全元件）中，不可明文暴露出去：防止 Key 受到**系统**底层漏洞的攻击。
3. APP 签名验证：只有设备内置证书验签通过的 APK 可以安装：防止 Key 受到**App** 侧的攻击。

## Memory mem_cdcfbeab8674135a

- Kind: field_note
- Created-By-Email: patrick@urovo.com
- Created: 2026-08-16T18:34:35+08:00
- Updated: 2026-08-16T18:34:35+08:00

### Content

为什么接触式交易的 Kernel 是所有的卡组织都用同一套 EMV L2 Contact，但是非接触各家都有自己的逻辑和认证。

### 结论：历史原因

- Contact（接触式）：统一都是 EMV L2 Contact 流程，各家卡组织只是参数上有所不同。因为最开始接触式发展的时候，各家卡组织竞争还没这么激烈，大家有闲心静下来，听 EuroPay / MasterCard / Visa 先统一一下流程再发展。
- Contactless（非接触式）：PICC 支付出来之后，大家都认知到这个是下一个支付时代最重要的东西，都快马加鞭的在做，没时间遵循一个统一的流程。

### 关键点

- 并非 Contact 和 Contactless 有什么技术上的区别导致一个统一、一个没统一。
- 纯粹是商业上的考量。

## Memory mem_fa237a923a501024

- Kind: fact
- Created-By-Email: patrick@urovo.com
- Created: 2026-08-16T18:52:54+08:00
- Updated: 2026-08-16T18:52:54+08:00

### Content

POS认证可以这么理解：

- 硬件认证：
  - ICC读卡模块：EMV L1 Contact
  - PICC读卡模块：EMV L1 Contactless
- 支付安全认证：PCI-PTS认证
- 交易能力认证：
  - Contact: EMV L2 Contact
  - Contactless:
    - America: Visa; MasterCard; Discover; American Express
    - China: UnionPay
    - Japan: JCB
    - India: Rupay
    - Russia: MIR
    - Europe: PURE / Bancomat
- 其他：
  - Google认证
  - TQM(Terminal Quality Management)认证

注：softPOS理论上不需要设备做任何的硬件认证，一般来说有个NFC模块，有GMS/GoogleKey，关闭开发者模式基本就可以直接用了。但是唯一确定softPOS能否使用的标准就是实测。

我们所有的POS的Kernel都是同一套，因为Kernel的逻辑是在SDK里面的，我们所有POS都用的是同一个SDK。

## Memory mem_92ed9d6f5c598f09

- Kind: fact
- Created-By-Email: patrick@urovo.com
- Created: 2026-08-17T16:09:06+08:00
- Updated: 2026-08-17T16:09:06+08:00

### Content

因为芯片的硬件限制，UROVO设备的USB只能走POGOPIN或者USB-C Port其中一个。

HOST Mode（USB主机模式设置）：

- 不开启（默认）：根据POGOPIN和USB-C哪个优先走USB就先把USB给到谁，之后另外一个入口就无法进行USB连接了。并且不会自动切换，连接的那个入口只要不断开就不会断连。
- 开启：用来锁定USB只走POGOPIN，不走USB-C Port。所以此时USB-C Port：
  - 只能：用于充电。
  - 不能：用OTG（HOST模式）；不能用来连接外设（如鼠标）（HOST模式）；不能通过adb连接电脑（DEVICE模式）；不能用USB来连接Ethernet。

## Memory mem_2d60c194d2c0f069

- Kind: field_note
- Created-By-Email: patrick@urovo.com
- Created: 2026-08-17T21:52:23+08:00
- Updated: 2026-08-17T21:52:23+08:00

### Content

### RFID 相关参数

- UHF 频段：860 - 960 MHz（HF 可以用 NFC 模块来读取，其他频段的 RFID 读取我们没做）
- 读取距离：1.5m（E310）- 15m（DT50P - E710）
- 功率：1W（30dBm）/ 2W（33dBm）/ 4W（36dBm）【不同国家是对 RFID 读写器的功率有限制的；RFIDDemo 最高只能设置 30dBm，天线的方向增益可以增加 6dBm】
  - 增加3dbm为功率增加一倍，减少3dbm为功率减少一倍。
  - 所以能设置到最高的功率为36dbm(4W)[30dbm + 6dbm]，这个也是FCC的标准，RFID功率不能超过36dbm(4W)
- 读取 RFID 效果好的几个要点：（RFID Reader 的天线正态曲线 + 工作频段截断）与（RFID TAG 的天线正态曲线）重合度越高越好
  - RFID Reader 的天线正态曲线主要分为美标天线（约 902 - 928 MHz）和欧标天线（约 865 - 868 MHz）【此时下降到 70%】
  - 工作频段截断可以在软件里面设置，通常是要和当地法规对齐的（即使软件支持全频段，因为芯片支持全频段），截断区间就是下频点到上频点之间
  - RFID TAG 的天线正态曲线也主要分为美标天线（约 902 - 928 MHz）和欧标天线（约 865 - 868 MHz）【此时下降到 70%】
  - 注：RFID 周围的环境会对 RFID TAG 产生频偏，最高可以频偏 30MHz，所以要根据实际使用场景选择合适的标签种类（如抗金属、抗液体等）

### 为什么 RFID 出货的时候会有频段之分

- 因为每个国家规定了 RFID 产品只能在某个频段用，避免占用别的频段；每个国家的规定不一样，所以出货的时候需要注意

### Urovo 的 RFID 产品的 RFID 相关配置

- 芯片：我们的 RFID 产品的 RFID 芯片上都支持全频段（860 - 960 MHz）
- 天线：出货的时候天线会有配置差异。RFID 天线可能是美标（约 902 - 928 MHz）也可能是欧标（约 865 - 868 MHz），不同版本的天线增益曲线的顶峰所在的频率不一致（正态曲线）。注：我们的 RFID 天线都是圆极化，也就是对 TAG 的摆放角度没有要求
- 工作频段（软件层面控制，矩形）：可以通过 RFIDDemo 去设置 RFID 设备的工作频段，一般是设置当地国家要求的工作频段。注意：
  - 设置的工作频段可以理解为在 RFID 天线的正态曲线上做滤波（截断）
  - 如果工作频段和天线的频段差别很大的话，那么天线的增益就可能就很低，也就是体现在读不到标签
  - 之所以是一个工作频段而不是一个频点，是因为 RFID 读取是跳频的，所以会在一个频段内随机找一个频点读取

### RFID 产品出货的时候要注意什么

- 比如美标 RFID 天线可能频率的增益顶峰是在 920 MHz，那么离这个频率越远，天线增益就越小；欧标 RFID 天线可能频率的增益顶峰是在 880 MHz，那么离这个频率越远，天线增益就越小
- 所以出货的时候，如果是美标的国家出了欧标的天线，那么因为法律规定这个产品的 RFID 的工作频段只能在美洲的 RFID 频段（如 902 - 928 MHz），但是欧标的天线在这个频段增益又特别差，用户感受就是很难读到 RFID TAG；反之在欧洲频段的国家使用美标的天线也是如此
- 出货的时候，可以通过 UFS 定制去锁定设备 RFID 的工作频段，来满足当地的合规性要求（默认就是对应的频段；并且用户无法修改）
- 注：如果出了与当地 RFID 规定频段不一致的 RFID 设备，导致正常当地的工作频段读不到标签。这种情况即使法规上不允许，但是可以通过 RFIDWedge 去调整设备的 RFID 工作频率，来让设备正常工作，但是仅限于 DEMO 使用，大批量出货是要负法律责任的

### RFID 工作流程

- 设备 RFID 模块工作：RFID 由外接 RFID 芯片（E310/E710）和 RFID 天线组成。工作时会发送 CW（连续波）给 RFID TAG 持续供电
- 设备 RFID 广播激活并给 Q：RFID TAGs 收到 CW 之后被激活（通过 CW 的波获取能量），然后读取里面的 Q，并从 [1, 2^Q] 里面随机选择一个值作为 time slot。这个是 Anti-collision 的核心
- 设备 RFID 逐渐推进 Time Slot：每个 TimeSlot 可能会 SUCCESS / PASS / AGAIN 三种。如果发现 Collision 就进行下一轮，直到读完所有的（所以 RFID 读取是一个一个数据出来的，不是同时出来的）
- RFID TAG：
  - 先是利用不间断的 CW 波进行激活并保持唤醒，持续监听 Time Slot 的推进
  - 轮到自己的 Time Slot 之后，就会和 RFID Reader 进行命令交互
  - RFID 标签通过改变负载阻抗来使得反射回去的信号发生变化，RFID Reader 可以检测到这个反射的信号变化才解析数据
  - 注：读取速度极快，所以即使有很多 Time Slot 并且有很多命令交互，但是读取还是感觉极快
- 数据层：
  - 数据处理（比如说做过滤去重复，因为 RFID 一定是一直读的，不会只读一轮就停下来，所以重复的数据要在软件层处理）
  - 对接后台

## Memory mem_e425cb6b472b89be

- Kind: terminology
- Created-By-Email: patrick@urovo.com
- Created: 2026-08-18T10:38:51+08:00
- Updated: 2026-08-18T10:38:51+08:00

### Content

### eMCP / uMCP 存储封装

- eMCP = RAM + eMMC
- uMCP = RAM + UFS
- eMCP 比 uMCP 便宜，uMCP 性能更好（主要是因为 UFS > eMMC）
- MCP 的含义：RAM 和 ROM 封装到同一个芯片之中
- 注：刷机的时候要注意是 uMCP 还是 eMCP 的包，要根据实际情况选择

## Memory mem_7cd2db0b4acefa23

- Kind: roadmap
- Created-By-Email: patrick@urovo.com
- Created: 2026-08-18T12:20:12+08:00
- Updated: 2026-08-20T14:42:23+08:00

### Content

UROVO 产品路线图（UROVO Products Roadmap 2026-05-07）

一、Android 版本发布时间表
（发布顺序：Google 发布 → 芯片厂商集成 → 厂商采用）

| Android 版本 | 发布    | GMS(MADA) 新设备截止 | LR 截止(N+2 发布) | GMS(EDLA) 截止 |
| ------------ | ------- | -------------------- | ----------------- | -------------- |
| A15          | 2024 Q3 | 2026 Q1              | 2026 Q3           | 2027 Q1        |
| A16          | 2025 Q3 | 2027 Q1              | 2027 Q3           | 2028 Q1        |

二、各产品更新计划

【DT50S】（2022 年上市，首发 Android 11）

- 系统升级路线：
  2023 H1 首发 MVP A11
  2024 H2 升级 Android 13（A13）
  2026 H2 升级 Android 16（A16）
- 停售：2028 Q4（End of Sale）
- 停止服务：2030 Q4（End of Service，设备与备件同）

【DT50 Pro】（2026 年上市，首发 Android 16）

- 系统升级路线：
  2026 H2 首发 MVP A16
  2028 H1 升级 Android 18（A18）
  2029 H1 升级 Android 19（A19）
- 停售：2031 Q4（End of Sale）
- 停止服务：2033 Q4（End of Service，设备与备件同）

【DT66】（2024 年上市，首发 Android 13）

- 系统升级路线：
  2024 H1 首发 MVP A13
  2026 H2 升级 Android 15（A15）
  2027 H1 升级 Android 17（A17）
- 停售：2029 Q4（End of Sale）
- 停止服务：2031 Q4（End of Service，设备与备件同）

【DT610】（2025 年上市，首发 Android 15）

- 系统升级路线：
  2025 H2 首发 MVP A15
  2027 H2 升级 Android 17（A17）
  2029 H1 升级 Android 19（A19）
- 停售：2031 Q4（End of Sale）
- 停止服务：2033 Q4（End of Service，设备与备件同）

【DT610 Pro】（2026 年上市，首发 Android 15）

- 系统升级路线：
  2026 H2 首发 MVP A15
  2028 H1 升级 Android 17（A17）
  2029 H2 升级 Android 19（A19）
- 停售：2032 Q4（End of Sale）
- 停止服务：2034 Q4（End of Service，设备与备件同）

【DT630】（2026 年上市，首发 Android 15）

- 系统升级路线：
  2026 H2 首发 MVP A15
  2028 H1 升级 Android 17（A17）
  2029 H2 升级 Android 19（A19）
- 停售：2032 Q2（End of Sale）
- 停止服务：2034 Q2（End of Service，设备与备件同）

三、产品规划 Q&A（原文档问答）

1. DT610 / DT610 Pro / DT630 如何定位？推广注意事项？
   不同场景、不同竞争对手：
   - DT610：零售门店，对标 Z 公司 EM45、BB 公司 X40
   - DT610 Pro：仓储/物流，对标 Z 公司 TC58、TC501，H 公司 CT47、CT70
   - DT630：工业手机，对标 S 公司 X Cover7 / 7Pro

2. DT50S 与 DT50 Pro 如何定位？
   - DT50 Pro 提供更高的 CPU 性能、更先进的 Wi-Fi 性能，
     对标 MT8781 / SM6225 平台的竞品。
   - 两个产品均为长生命周期产品，Android 可升级。
   - 由于内存供应影响，8+128 配置只能推 DT50S。

3. UROVO 扫描头引擎如何规划？
   - 全面推广 SE2030 Series
   - HS7 / SE2030W --> SE2030S
   - N6803 --> SE2030FR

## Memory mem_a165e97d3fe80740

- Kind: field_note
- Created-By-Email: patrick@urovo.com
- Created: 2026-08-18T19:05:15+08:00
- Updated: 2026-08-18T19:05:15+08:00

### Content

### KLD 密钥注入方式

#### (1) DUKPT

- **客户**购买 KLD，并且在当地安全房进行密钥注入操作。
- 客户在 KLD 中注入 BDK 分量 和 KSN_Prefix 【KSN = KSN_Prefix + SN】
- KLD 和设备双向认证，协商 KBPK，并且加密 IPEK 封装成 TR31。（不同设备不同的 IPEK）【IPEK = KSN + BDK】
- IPEK 注入。

#### (2) MK/SK

- **客户**购买 KLD，并且在当地安全房进行密钥注入操作。
- 客户在 KLD 中注入 KEK 分量。
- 客户导入 xlsx 表格到 KLD 中。（表格包括 MK_Encryted 和 SN 的对应）
- KLD 会把加密的 MK 进行解密处理，存放在 SE 中。
- KLD 和设备双向认证，协商 KBPK，并且加密 MK 封装成 TR31。（不同的设备不同的 MK）
- MK 注入。

#### KLD 注意事项

- i2000 需要刷入专门的 KLD OS，才能用作 KLD。
- 子 POS 需要装 SubPOS 才能。
- 初始的管理员密码是 8 个 1 和 8 个 2。修改密码之后一定要记住！因为无法 Reset，并且后续要告诉客户。

### RKI / KMS 密钥下发方式

#### (1) DUKPT

- **客户**利用 Different physical sealed packages 把 BDK（Base Derivation Key）的 components 给到 Urovo。
- Urovo 在 KMS 后台（HSM）把 BDK 的分量注入，后台系统合成 BDK 并进行 KCV 校验。（KCV 用来校验正确性）
  【另一种方式为把 KEK 的分量给到 Urovo，然后 Urovo 后台合并 KEK，然后再把 KEK 加密封装的 BDK（TR31）传过来，Urovo 进行解封装后注入 KMS 后台（HSM）。】
- **客户**需要提供 KSN Format（KSN = Prefix + SN + Counter，客户定义的关键是 Prefix）
- 在后台给该 BDK 绑定 SN List。每个 SN 在下载的时候会自动根据 BDK 以及 KSN Format 去派生 IPEK。
- 客户 APP 触发 / 我们的产线上 SNTool 触发 密钥下载服务（com.ubx.dukpt），设备主动轮询后台是否有密钥需要下载。
- KDH 服务器和设备利用预置的设备证书以及 CA 证书进行双向认证，认证成功后协商形成 KBPK。
- 利用 KBPK 在网络中传输 TR31 封装的 IPEK_PlainText。
- 设备下载完 IPEK_PlainText 后，利用 KBPK 解封 TR31 拿到 IPEK_PlainText 的明文，并调用 SE 的 API 进行密钥的注入。
- 每台设备一个独有的 IPEK。
  【客户需要提供 BDK 的分量 + KSN Format + 其他 DUKPT 参数】

#### (2) MK/SK

- **客户**利用 Different physical sealed packages 把 KEK（Key Encryption Key）的 components 给到 Urovo。
- Urovo 在 KMS 后台（HSM）把 KEK 的分量注入，后台系统合成 KEK 并进行 KCV 校验。（KCV 用来校验正确性）
- **客户**提供 KEK 加密的 MK List（每个 MK 对应一个 SN），然后再把 KEK 加密封装的 MK（TR31）传过来给 Urovo。（TR31 = Header + Encrypted_MK + MAC，其中 MAC 用来防篡改）
- Urovo 在 KMS 后台（HSM）把 MK_TR31 的注入，然后利用 TEK 去解密获得 MK 的明文，存放在 HSM 里面。
- Urovo 在后台给该 MK List 绑定 SN。
- 客户 APP 触发 / 我们的产线上 SNTool 触发 密钥下载服务（com.ubx.dukpt），设备主动轮询后台是否有密钥需要下载。
- KDH 服务器和设备利用预置的设备证书以及 CA 证书进行双向认证，认证成功后协商形成 KBPK。
- 利用 KBPK 在网络中传输 TR31 封装的 MK_PlainText。
- 设备下载完 MK 后，利用 KBPK 解封 TR31 拿到 MK 的明文，并调用 SE 的 API 进行密钥的注入。
- 如果要一密多机的话，只需要一个 MK，但是很不安全。
  【客户需要提供 KEK 的分量 + KEK 加密的 MK（List） + 其他 MK/SK 参数】

#### RKI/KMS 注意事项

- KLD 和 KMS 都需要 PCI 安全认证的，因为都存放着密钥。
- 设备在出厂的时候必须要用 SNTool 去预先下载 KMS_CA 证书以及设备证书（PED），KMS_CA 证书用来核验 KDH 服务器的身份，PED 证书用来给 KDH 展示身份。
- 一般来说是一个 DATA 加密的 DUKPT，一个 PIN 加密的 DUKPT。

## Memory mem_559f40ff9b85240c

- Kind: field_note
- Created-By-Email: patrick@urovo.com
- Created: 2026-08-18T20:30:37+08:00
- Updated: 2026-08-18T20:30:37+08:00

### Content

### 电子价签（ESL）的一些信息 - 20260818

- 基站目前支持 POE 连接，也支持 WiFi 连接。
- 基站控制范围：空旷半径为 30 米左右，有阻挡的话 20 米左右，面积也就是 1500 平米左右，实际情况以实测为准。（规格书内写 100 米为基站信号最远可达，但是控制价签需要稳定的数据交换）
- ESL 支持 NFC，但是这个 NFC 一般是用来给 PDA 快速读取价签的信息，暂时不支持存入信息。

## Memory mem_3d37b7a30c9f558f

- Kind: field_note
- Created-By-Email: patrick@urovo.com
- Created: 2026-08-21T10:24:48+08:00
- Updated: 2026-08-21T10:24:48+08:00

### Content

DT50S 电池测试状态说明（指示灯 / 振动 / 显示）：

1. No Battery（无电池）：一颗红灯常亮；设备振动；无显示
2. Locked Mode / Protect Mode（锁定保护模式，0V）：一颗红灯常亮 + 一颗红灯闪烁；无显示
3. Over-discharge State（过放状态，3.2V – 3.5V）：两颗红灯常亮；充电器显示（无电池百分比）
4. Normal State（正常状态，3.5V=0% – 3.85V=50% – 4.2V=100%）：一颗红灯常亮；显示电池百分比

## Memory mem_31999bcafac8459e

- Kind: fact
- Created-By-Email: patrick@urovo.com
- Created: 2026-08-24T19:28:20+08:00
- Updated: 2026-08-24T19:28:20+08:00

### Content

### Understanding RFID Tags（RFID 标签基础知识：构成、关键参数、类型与主要应用）

#### Composition（构成）

- RFID Inlay (Chip & Antenna)
- Face material（面材）
- Adhesive（背胶）

#### Three most important parameters of an RFID Tag（标签三个最重要的参数）

- Type: Normal, Anti-metal, or On-Liquid（类型：普通 / 抗金属 / 抗液体）
- Dimension（尺寸）
- User Memory: No Memory (M730/M830); or more（用户存储区：无存储（M730/M830）；或有更多存储）

#### Three types（三种类型）

1. **Normal RFID Tag**（普通标签，Clothing-related mostly 多用于服装相关）
   - RFID Sticker Tag（RFID 不干胶标签，Any regular product 适用于任何普通产品）
   - RFID Woven Tag（RFID 织唛标签；Apparel / Shoes / Bags 服装、鞋、包）
   - RFID Hang Tag（RFID 吊牌标签；Apparel / Shoes / Bags 服装、鞋、包）
   - Plastic Card Tag（塑料卡标签；Logistics Industry 物流行业）
   - RFID Laundry Tag (抗水洗烘干标签；Hotel Industry 酒店行业)

2. **Anti-Metal Tag**（抗金属标签，Assets-related mostly 多用于资产相关）
   - Flexible anti-metal tag（柔性抗金属标签；Any on-metal environment, e.g. Assets 任何金属表面环境，如资产）
   - PCB anti-metal tag（PCB 抗金属标签；PCB RFID Inlay）
   - ABS anti-metal tag（ABS 抗金属标签；安装方式：screw mounting 螺丝固定 / rivet mounting 铆钉固定 / cable tie 扎带固定 / adhesive mounting 背胶粘贴；应用：Pallet 托盘、turnover basket 周转筐、Industrial equipment 工业设备、Assets 资产）
   - Note: Anti-metal Tag uses frequency offset to counter detuning of the metal. Thus, it's not optimal to be used in non-metal scenario.（抗金属标签通过频率偏移来抵消金属的失谐/频偏，因此不适合用于非金属场景）

3. **On-Liquid Tag**（抗液体标签）
   - RFID Flag Tag（RFID 旗帜标签；天线不贴合表面 Antenna is not attached to the surface；应用：Food Industry 食品、Healthcare Industry 医疗、Electronics Industry 电子）
   - RFID On-Liquid Tag（RFID 抗液体标签；可直接贴附于液体表面；应用：Food Industry 食品、Healthcare Industry 医疗）

#### Three main use cases（三大主要应用场景）

- Asset Management（资产管理）：Anti-counterfeit 防伪、Anti-theft 防盗、Self-checkout 自助结账
- Inventory（库存盘点）：In-store inventory 门店盘点、Warehouse Inventory 仓库盘点
- Logistics（物流）：Goods tracing 货物追踪

## Memory mem_94ddb1c6f01962bc

- Kind: fact
- Created-By-Email: patrick@urovo.com
- Created: 2026-08-27T20:08:52+08:00
- Updated: 2026-08-27T20:08:52+08:00

### Content

DT50P和DT50D使用的OS与DT50S的固件，可以随着DT50S安卓版本的升级（安卓16）同步升级到安卓16。

## Memory mem_66df431b83b1ca2c

- Kind: field_note
- Created-By-Email: patrick@urovo.com
- Created: 2026-08-27T20:18:49+08:00
- Updated: 2026-08-27T20:18:49+08:00

### Content

关于体积测量：DT66已经不出ToF版本了。目前只有DT610和DT610Pro支持体积测量，具体方式是设备背后安装一个带3D结构光摄像头的背夹，背夹与设备通过POGOPIN连接。

## Memory mem_2294343d62f55988

- Kind: fact
- Created-By-Email: patrick@urovo.com
- Created: 2026-08-27T21:38:14+08:00
- Updated: 2026-08-27T21:38:14+08:00

### Content

DT50P Lite 与 DT50P 的简洁区别：Lite 电池容量更小（续航约5小时 vs 7小时）；Lite 天线功率更小（约15米 vs 20米）。因此 Lite 更轻便（约500克 vs 700克）。DT50P 本体在用户（尤其是女性用户）手中长时间使用容易造成疲劳，所以推出了 Lite 版本。

## Memory mem_d19620cc58bab544

- Kind: fact
- Created-By-Email: patrick@urovo.com
- Created: 2026-08-27T22:25:54+08:00
- Updated: 2026-08-27T22:25:54+08:00

### Content

1. CT58C是MTK芯片，DT50S是高通芯片。
2. CT58C只能支持Android 12(SQ58C)和Android 14(SQ58CU)。DT50S可以支持Android 11(SQ53S)，Android 13(SQ53ST)，和Android 16。
   【各安卓版本均为同一套硬件，只是固件不同】
3. CT58C配置为国内场景而简化过，所以更便宜。DT50S为全球通用版，更贵。
4. CT58C主要出国内，DT50S主要出国外。

## Memory mem_a16451595dc313f9

- Kind: field_note
- Created-By-Email: patrick@urovo.com
- Created: 2026-08-29T14:14:15+08:00
- Updated: 2026-08-29T14:14:15+08:00

### Content

RFID DEMO快速手册：

1. Inventory Page：用于做RFID Reading / Inventory的DEMO

- Single / Auto: Single为读到一个就停止；Auto为一直读。
- Filter: 可以用于筛选指定标签去读 (Note: EPC = 检验位\_16-bit + Metadata_16-bit + 96-bit = 128 bits)
  - Addr: 筛选起始位置，一般填写32，跳过校验位和Metadata。（如果需要对后面的bits做筛选，则可以增大）
  - Len: 一般填写96 bits （一般EPC的Data bit是96 bits，很少有例外）
  - Data：填入需要筛选的EPC Data（也可以填入TID或者USER_Memory)【小tips：要快速进行筛选某个标签进行读取测试的时候，可以先在Config中把Power调整成1（或者Range Control调整成100），然后近距离读取标签确定标签具体的EPC值，然后长按对应的EPC，选择READ/WRITE，这样就可以快速COPY并且在后续PASTE到Filter Data中来。
- FastTID：勾选后可以同时读取TID和EPC（不勾选只有EPC读取）
  - 这个和Config里面的FastTID一样的
  - FastTID和EPC+TID模式的区别为：如果RFID TAG是IMPINJ的话，FastTID比EPC+TID读取的要更快。但是不如只读EPC。

2. Access Page：可以用来读，写，锁，杀标签。

- 如何DEMO写标签（EPC）：
  - 先选定EPC（一般写TAG都是一个一个写的，因为TAG代表的是单个物体，而不是一类物体，和批量读的意义不同）
  - Access Pwd：一般是八个0（00000000）
  - Bank：选择EPC（这种场景Ptr和Len不需要选择）
  - 写之前先读取，确保标签在RFID读取范围内。然后可以复制读到的EPC内容。
  - 粘贴到WriteData中，进行修改，然后点击WriteEPC

3. Gen2X：必须要选择指定的Gen2X Profile才能使用。（Gen2X的优点为速度更快，灵敏度更高，抗干扰更强。要注意必须TAG和READER同时支持Gen2X才能走这个协议，否则会被fallback到Gen2）

4. Config：

- Frequency Settings: 必须要根据设备实际的天线的标准去设定！
  - RFID天线是有美标(FCC)和欧标(EU)之分的，所以RFID软件也必须要选择对应的频段（FCC或者EU）。天线的功率曲线类似于正态曲线，RFID软件的设定相当于一个频段滤波器。只有两者匹配上了，才能正常做RFID读写。
  - 不同国家的频段还需要更加细化，这个是根据各个国家关于RFID频段的法规来的。
  - 正常的天线都是全频段的，抗金属/抗液体的标签才分美标或者欧标。对于抗金属/抗液体，则需要标签的频段也和读写器的频段一致才能工作。
- Power Settings: RFID芯片的增益（E310 / E710）。（不包含非天线的定向增益）
  - 正常的情况下可以设置最大值，最大值会根据实际设备的不同在28 - 30 - 33之间波动。
  - 如果想要只读一个标签，那么可以设置1，然后把那个标签拿进来只读它。
  - 读写器的功率 = RFID芯片的功率 + RFID天线的定向增益（一般是6，所以6 + 30 = 36。而一般国家会要求总功率最大值不超过36）（RFID天线的定向增益就是相当于把球状的信号集中在一个方位，所以会产生增益）
- Memory Bank Settings: 可以自由选择读什么内容（Note：RFID TAG四大区域为TID，EPC，USER_MEMORY，RESERVED）
  - 一般选择EPC就行了，如果是要同时读EPC和TID的话，也可以直接在Inventory中选择FastTID。
- Other Parameters：
  - Full Inventory: 正常盘点就选择这个（包括DEMO）
  - Rapid Repeat: 想要测试极限读取速度就用这个（E310一般是300 TAG/s，E710一般是1000 TAG/s）
  - Max Range: 想要测试极限距离就用这个
  - Custom Mode：
    - Target: A/B为A B面READER都会去读，A为只读TAG的A面，B为只读TAG的B面。（Note: TAG会在和READER进行交互之后被翻转，并且在指定时间之后翻转回来）【正常设置A/B】
    - Q: 用于RFID防碰撞，Q表示Initial Round是2^Q个SLOTs。Q应该设置的和实际TAG数量越接近越好，同时这个是Dynamic Q，后续会根据实际情况调整，只有第一次受到Q设置的影响。【正常设置6】
    - Session: 只有当Target设置为A或者B的时候才生效（A/B时不生效）。S0表示瞬时翻转回来，即同一个标签会被反复读，好处是不会漏读，坏处是单体重复导致总体读取速度变慢。S1表示五秒翻转回来，属于Inventory的Sweet Spot。S2和S3表示一分钟后才翻转回来，好处是总体读取速度快，坏处是容易漏读（因为Reader可能没收到反射回来的数据，但是TAG已经翻转了，并且长时间休眠）。【A/B的时候无所谓 设置个S1正常值就行】
    - Profile(Reader Mode)：
      - Gen2: K越大，读取速度越快。M越大，灵敏度越高。
      - Gen2X：K越大，读取速度越快。B越大，灵敏度越高。
      - BOTH：如果同时存在Gen2的TAG以及Gen2X的TAG。那么就必须要选择M+B的Gen2X Profile，否则只能读其中一种TAG。
  - Range Control: 自动过滤掉信号强度不够的，Value越大则读的越少。
    - 主要用于需要把读取距离限定在某个范围的场景（Control Range越大，读取的距离越短）
    - 以及快速读取某一个标签的数据，避免其他标签的干扰。（Control Range设置为100，然后拿标签去读）
  - 实际DEMO怎么设置Custom Mode？
    - 如果想要最佳灵敏度：A/B(Session无所谓 两面都读）; Q=6; Profile选择M最大的（选择B最大的如果是Gen2X标签的话）。Range Control确保是0.
    - 如果是想要最快的读取速度：A + S0; Q=6; Profile选择K最大的（Gen2X的话记得选择Gen2X的Profile）。Range Control确保是0.
    - 正常盘点：A + S1(同一个标签五秒内不会被重复读到）; Q要根据实际情况来Log2()。Profile可以在灵敏度和速度中间选一个Balance Point。

5. Find Page: 用于快速找到某个EPC的位置，通过RSSI的数字。

6. LED Page: 用于快速找到某个EPC的位置，通过LED亮灯。（有一些RFID TAG是自带LED灯的，可以通过CW的能量来点亮。主要用于快速定位某个TAG）

## Memory mem_77337abc9879d143

- Kind: fact
- Created-By-Email: patrick@urovo.com
- Created: 2026-08-29T14:28:08+08:00
- Updated: 2026-08-29T14:28:08+08:00

### Content

RFID标签频段：一般的标签都是全频段的（840MHz - 960MHz）；抗金属和抗液体的标签才会有美标（FCC: [902, 928]）或欧标（EU: [865, 868]）之分。这种情况下，Reader的天线频段必须要和TAG的频段匹配，才能正常工作。

## Memory mem_fcec2472aa7d42b6

- Kind: field_note
- Created-By-Email: patrick@urovo.com
- Created: 2026-08-29T15:25:17+08:00
- Updated: 2026-08-29T15:25:17+08:00

### Content

### RKI方案之TR31密钥传输介绍：KBPK（KEK）协商 -> TR31密钥传输

1. TR34: KBPK（KEK）的协商一种方式

- 双向认证之后（互相利用CAPK验证对方证书以及调整成功），利用一方随机一个KBPK，然后利用对方的Public Key加密后（确保传输安全） 以及 自己的Private Key签名后（确保防篡改 以及 来源认证）。把KBPK同步给到另一方，完成KBPK的协商。后续可以用该KBPK进行TR31（加密密钥封装包）的传输。

2. mTLS：KBPK（KEK）的协商方式

- 经典双向TLS认证(ClientHello(R1+C_Cert) -> ServerHello(R2_Encrypted+S_Cert) -> Transcript_Generate_R3 => R1+R2+R3 = KBPK)完成KBPK的协商。后续可以用该KBPK进行TR31（机密密钥封装包）的传输

3. KBPK（KEK）分量保密的物理传输：把KBPK的分量利用保密的物理路径进行传输，到目的地后KCV验证Components无误后XOR组装成KBPK后，再次KCV验证。后续可以用该KBPK进行TR31（加密密钥封装包）的传输。

Note:

- 什么是TR31？TR31是一个用KBPK加密封装的密钥。和普通密钥相比就是多了两点：1. 加密性 - 利用KBPK进行加密安全传输以及签名放篡改 2. 封装性 - 比纯密钥了多了具体使用的metadata

## Memory mem_9997e27fc3c223c9

- Kind: fact
- Created-By-Email: patrick@urovo.com
- Created: 2026-08-31T20:01:33+08:00
- Updated: 2026-08-31T20:01:33+08:00

### Content

CT48C和CT58C都可以直接从Android 12升级到Android 14，因为硬件是一样的。

## Memory mem_f4d805388e0b69c3

- Kind: field_note
- Created-By-Email: patrick@urovo.com
- Created: 2026-08-31T20:26:38+08:00
- Updated: 2026-08-31T20:26:38+08:00

### Content

DT610的芯片Q-6690分为FP1和FP4两个性能档位（硬件完全相同），默认是FP1(2.0GHz)，FP4(2.9GHz)是选配。FP是Feature Pack的意思，用的是License进行管控。

## Memory mem_323bb158d4e122ad

- Kind: product_knowledge
- Created-By-Email: patrick@urovo.com
- Created: 2026-09-01T13:59:45+08:00
- Updated: 2026-09-01T13:59:45+08:00

### Content

### ESL产品相关FAQ：

### Q: 这个方案是你们自己的吗？包括什么？

- 整套方案包括我们的ESL，对应的基站（不可外采），以及我们自己开发的后台。对外可以说完全是我们自己做的。（实际上我们只负责产品定义，物料采购，以及平台开发）

### Q: ESL支持几种颜色？（客户：你们ESL产品可以支持各种颜色吗？）

- 因为是墨水屏，不像LCD那样可以自由组合RGB颜色，目前只支持黑白红黄四色（老款为黑白，现在通常为黑白红/黑白黄三色，四色是一个卖点，在模版制作上更加艳丽）

### Q: ESL的产品尺寸有哪些？

- 现在我们在做的有1.6寸（已经有香港客户在小批量试点了 很适合cosmetics这样很小的商品），2.1寸，2.6寸（正常我们见到的尺寸 两根手指的尺寸），4.2寸（一个手掌这么大）。5.8寸和10寸正在做。（常用来做促销广告之类的了）

### Q: ESL产品的续航怎么样？需要频繁换电池或者充电吗？

- 用的是是墨水屏，不是液晶显示屏。正常使用是基本不会耗电的。用的是纽扣电池 每天都刷新 可以使用至少五年。用户可以在我们的平台上实时监控ESL的电量。

### Q: ESL的通信协议是什么？我们用我们的WiFi路由器(AP - Access Point)就行了是吗？

- 基站和ESL之间用的是2.4GHz私有协议，可以简单理解为为了ESL这种产品的定制版本的BT协议（参考BLE的心跳唤醒通信机制），不是WiFi，需要配套购买我们的基站才能使用。

### Q: 是否支持NFC，能否用NFC进行刷价格？

- 支持NFC，但是NFC主要适用于快速获取价签的信息（如消费者用商户APP去获得贴ESL可以快速在手机上查看相关产品的情况 可以没货的时候快速下订单之类的）。NFC刷图的场景基本只存在于DEMO。实际使用还是用基站去修改价签。

### Q: 如果我想要快速找到某类商品，能做吗？

- 支持红黄蓝绿青紫六个颜色，该功能一般用于快速找货物。但是ESL的产品定位和声光标签不一样，连续只能亮48小时，同时亮度一般。能做，但是不属于通用应用。

### 基站相关FAQ：

### Q: 基站(Access Point / Base Station)是否支持PoE(Power over Ethernet)？是否支持WiFi？

- 可以支持WiFi(此时用电源充电） 和 PoE(此时不需要额外充电线，需注意PoE必须要客户的路由器也支持PoE），满足各种场景的部署。

### 方案相关FAQ：

### Q: 我的门店面积很大，基站的控制距离有多远？

A: ESL距离基站最多30米还可以控制，覆盖范围为2000平方米左右。正常实施的话 30米就要放一个基站了（注意：规格书上说的100米为基站单体信号的最远可达距离，非该方案的有效距离）【注意：ESL和RFID一样属于方案类产品，和实际的使用场景情况高度绑定，无法和客户承诺说一个店面放几个基站就够了，需要实际测试】

### 平台相关FAQ：

### Q: 能不能能否现场DEMO刷图？

A: 无法现场DEMO，因为需要提前搭建基站。可以放视频 或者到展厅相关负责人进行DEMO。

### Q: 刷新的时间有多长？

- 刷新时间：可以按照20秒去说。如果客户问批量的话就是一个基站同时给1000个ESL刷新的话 需要10分钟。

### Q: 客户：我们是阿拉伯文字 / 韩文 / 日文，你们ESL能否支持正常显示？特殊字符能否显示？

A: 理论上任何字体都能显示，因为字体的渲染和计算是在平台上的，平台计算完之后把图片发给ESL去显示。

### Q: 你们平台上的字体没有我们想要的，能否用我们自己的字体？

A: 如果有需求的话，可以把字体给到我们，我们集成到平台上。

### Q: 怎么和我们的后台集成（WMS / ERP）？

- 1. 客户的后台利用我们的提供的RESTFUL API进行开发。即客户后台商品价钱发生变化的时候，主动把信息推送到我们的后台上。2. 客户开发数据库的访问权限，我们开发middleware定时轮询客户的数据库。即我们开发软件，每隔一段时间看看客户后台商品的价格有没有变化，如果有变化的话，就更新ESL。

### Q: 我们想给冷藏食品 / 高温视频 使用ESL 你们能支持吗？

- 默认是0-40度；如果有冷藏或者高温的需求可以做。

### Q: 用久了，进灰进水导致ESL故障怎么办？

- 我们ESL默认是绝对防尘的（IP65），如果在经常会接触到水的环境中，可以选配IP68（可以防长时间浸水）

### 平台相关：

### Q: 如果我ESL刷新失败怎么办？我怎么知道？

- 1. 首先这个产品在失败后会自己重试10次。并且平台上有刷新的日志信息，可以查看到ESL刷新是否成功，对于失败的任务，我们也有一键重新推送的功能。2. 对于实际的效果，店员也可以利用我们的NFC信息查询，逐个核对ESL的实际画面效果。

### Q: 在ESL出现异常的时候，是否能主动通知我，还是说必须要IT人员去实时监控才行？

- 我们平台已经支持异常情况邮件推送的功能了，在基站下线，刷新失败，或者是ESL低电量的时候，每天会形成实时报告发送邮件到指定邮箱。降低IT运维的成本。

### Q: 客户在看平台的时候，问能否支持XXX功能？

- 可以回复我们可以进行开发。（硬件的变化设计成本需要和万波确定，软件层面我们是极其灵活的。别家可能不太好改动，我们的更新迭代速度是很快的。基本都可以先答应下来。）

### Q: 你们的服务器在哪？如果我不想把我的商品数据给你可以吗？

- 我们的服务器在深圳。我们的后台也支持私有化部署到客户的服务器上，满足客户对于隐私安全的需求，我们会提供技术上的支持。（服务器的内存16G/32G就足够了，容量的话1000个ESL，需要10G去存储。e.g., 如果买10000个，那么服务器至少要有100G）

## Memory mem_8604d87a6089b08d

- Kind: fact
- Created-By-Email: patrick@urovo.com
- Created: 2026-09-07T12:34:19+08:00
- Updated: 2026-09-07T12:34:19+08:00

### Content

原则上，只要支持相关卡组织的非接触支付（Contactless Card Payment），那么就支持 Apple Pay / Samsung Pay / Google Pay，不需要做额外的认证或者开发。因为这三个都是把自己伪装成卡片，在 POS 眼中他们和银行卡没有区别，直接走对应卡组织的 Contactless 的 EMV 流程就行了。

## Memory mem_d7a18fd673c40291

- Kind: fact
- Created-By-Email: patrick@urovo.com
- Created: 2026-09-07T15:58:57+08:00
- Updated: 2026-09-07T15:58:57+08:00

### Content

跌落与滚筒测试规格（同 DT50S 标准）：DT66、CT58 与 DT50S 一致。

- DT50S / DT66 / CT58：跌落 1.5 米，6 面 4 角，2 循环，共 20 次；滚筒 1 米 400 次。
- RT40s：跌落 1.8 米，6 面 4 角，2 循环，共 20 次；滚筒：产品规格书标准 1 米 1000 次，实测 1 米 500 次。
- 29M / 29MB：跌落 1 米，6 面 4 角，2 循环，共 20 次；滚筒 0.5 米 200 次。
- 68 / 69 / 65B / 65F：跌落 1 米，6 面 4 角，2 循环，共 20 次；滚筒 0.5 米 300 次。

## Memory mem_e50287a59b2e3d3d

- Kind: fact
- Created-By-Email: patrick@urovo.com
- Created: 2026-09-09T11:44:20+08:00
- Updated: 2026-09-09T11:44:20+08:00

### Content

i9600 Mini 的内部型号是 SQ69DM。

## Memory mem_4f652e914de8fec5

- Kind: field_note
- Created-By-Email: patrick@urovo.com
- Created: 2026-09-10T14:38:08+08:00
- Updated: 2026-09-10T14:38:08+08:00

### Content

### 不同设备的NFC读取

- DT66：可以支持正面和背面读取。但是一次性只能读一面，需要软件上去切换（Enterprise Settings -> NFC Switch）。
- DT610：只能支持正面 NFC，无法在 Enterprise 里面进行 switch。因为这个设备主要用于 SoftPOS（已经做了 EMV 的 L1 的非接触认证）。
- DT610Pro：支持正面，背面，顶部三个地方的NFC，不需要在Enterprise Settings里面切换。
- DT630：只有正面NFC。
- K388Pro：NFC在屏下。
- DT50P：没有NFC。
- DT50P Lite：NFC在扫描头那里。

## Memory mem_b7b725bdd64b88aa

- Kind: field_note
- Created-By-Email: patrick@urovo.com
- Created: 2026-09-10T18:30:57+08:00
- Updated: 2026-09-10T18:30:57+08:00

### Content

### DT50Pro, DT610, K388Pro 写入 Google Key 的方法

#### 1. 写入 KeyBox

```
adb shell LD_LIBRARY_PATH=/vendor/lib64/hw KmInstallKeybox keybox.xml 1 true rkp
```

#### 2. 提取设备 CSR

```
adb shell rkp_factory_extraction_tool --output_format build+csr > /Users/patrickxu/Downloads/csr_device123.json
```

#### 3. 上报设备 CSR 给到 Google 后台（需要外网）

```
python3 /Users/patrickxu/google-key/device_info_uploader.py --credentials-keyfile /Users/patrickxu/google-key/xt40-390507-f8f446767902.json --company-id 8201164 --json /Users/patrickxu/Downloads/csr_device123.json --update
```

(Note: 脚本需要根据实际情况做一下本地化处理。)

## Memory mem_2218e350ac1c66b1

- Kind: field_note
- Created-By-Email: patrick@urovo.com
- Created: 2026-09-11T15:58:04+08:00
- Updated: 2026-09-11T15:58:04+08:00

### Content

### DT50P / DT50P Lite 的 NFC 支持差异

- **DT50P**：不支持 NFC。
- **DT50P Lite**：支持 NFC，NFC 的位置在**扫描头那里**（即 NFC 天线位于扫描头区域）。

## Memory mem_fad7b311f82a222c

- Kind: fact
- Created-By-Email: patrick@urovo.com
- Created: 2026-09-11T20:42:32+08:00
- Updated: 2026-09-11T20:42:32+08:00

### Content

### 不同产品 NFC 方案对比

1. **NXP PN7220 挂载 AP**：支持安卓 NFC 原生全套协议。

- SQ27M：因为这个设备定位是带打印机的 PDA，所以拥有和 PDA 一样的 NFC 能力。
- SQ68PN：因为保加利亚项目需要 APPLE ECP 认证。
- SQ69 系列：因为要支持屏下 NFC，对性能有要求。

2. **国产芯片挂载 SP**：NFC 主要用来支持非基础支付银行卡。NFC 智能卡功能都是我们自己实现的，可能会有很多 bug，比如不支持卡模拟。

- 其他的 POS 机型。

**Note**：PDA 都支持安卓 NFC 原生全套协议。

## Memory mem_670b34deb1ec940b

- Kind: field_note
- Created-By-Email: patrick@urovo.com
- Created: 2026-09-11T20:43:18+08:00
- Updated: 2026-09-11T20:43:18+08:00

### Content

### Android Enterprise 利用 Zero-touch 做 Provisioning 的操作流程

与 mem_5038d16c6162eaac（《MDM 管理设备的方式：三种架构类型 + 四种 Provisioning / 集成方式》）中的 Zero-touch 概述互为补充：该条讲 Zero-touch 的原理与定位，本条讲具体落地操作步骤。

#### 操作步骤

1. 先把所有的设备绑定在自己的 Reseller 账号（可以通过 IMEI 或者 SN），然后给客户创建账号，并且把对应的设备加到客户下面。（Urovo 是有自己的 Reseller 账号的，可以给客户做 Zero-touch Provisioning）
2. 然后客户就可以在 Zero-touch Portal（https://partner.android.com/zerotouch），利用 Reseller 给创建的账号去登录，此时客户可以看到自己账号里面有被添加的设备。
3. 客户此时需要到自己支持 AE Zero-touch 的 MDM 账号里面生成对应的 Configuration，然后复制其中的内容。在 Zero-touch Portal 里面创建 Configuration，并把 MDM 生成的信息粘贴过去。
4. 最后只需要给设备绑定对应的 MDM Configuration 就行了，设备在开机向导联网后通过 AE 的方式（Device Owner）就会自动连接上 MDM。（如果当时没有联网的话，后续任何时候联网检测到有 Zero-touch 配置就会自动重置设备）

## Memory mem_3be181a4ddd73ba8

- Kind: fact
- Created-By-Email: patrick@urovo.com
- Created: 2026-09-11T21:11:54+08:00
- Updated: 2026-09-11T21:11:54+08:00

### Content

### KLD 与从设备认证 / 注钥流程

#### 1. 预置

- KLD：CAKRD → 验证从设备 CredKRD
- Slave：CAKDH → 验证 KLD CredKDH

#### 2. Check Binding（双向认证）

- Slave → KLD：SN + CredKRD
  KLD：CAKRD 验证 CredKRD + Certificate SN = Device SN → 保存 CredKRD
- KLD → Slave：CredKDH + CRL
  Slave：CAKDH 验证 CredKDH + CRL → 保存 CredKDH
  → 双方互信后才允许注钥

#### 3. TR-34 注钥

Query Key List
→ Key Exchange：KLD 用 Slave 凭证保护 Key + KLD 私钥签名
→ Slave 验签、解包、装载 Key
→ Key Verify：KCV 校验
→ Status Update：Slave 上报结果
→ 多把 Key 则重复 Exchange → Verify → Status

核心流程：
Check Binding → Query Key List → Key Exchange → Key Verify → Status Update

## Memory mem_084d553d7ef1e8e6

- Kind: fact
- Created-By-Email: patrick@urovo.com
- Created: 2026-09-11T21:29:15+08:00
- Updated: 2026-09-11T21:29:15+08:00

### Content

### eFuse（电子熔丝）

芯片内部中写死只读的数据，通过物理手段强行确保无法篡改。用途如下：

- **Secure Boot**：通过把 Root Key Hash 写入 eFuse 中，确保只有正确的 Bootloader 才能启动。（Bootloader 证书验证失败则无法启动）
- **防止物料替换**：SoC 和 RAM 和 ROM 在做数据交互的时候会验证对方的 eFuse，如果 eFuse 数据不对，则说明物料替换过了，则数据传输会被阻断。

## Memory mem_767c607a21da1b85

- Kind: fact
- Created-By-Email: patrick@urovo.com
- Created: 2026-09-11T21:47:57+08:00
- Updated: 2026-09-11T21:47:57+08:00

### Content

### 加密SN（Encrypted SN）

**目的**：防止代理非法篡改 SN（不使用 SNTool，而用其他手段）去出货，因此需要用加密 SN 进行管控。

**原理**：SN 加密后无法轻易篡改，确保 SN 号的 Integrity。

**对自己人的影响**：只有拥有权限的 SNTool 账号才能写入加密 SN，没有权限的 SNTool 账号无法写入加密 SN。

**如何获得加密 SNTool 账号**：需要在 OA 申请时勾选"写加密 SN"（也就是之前的 UKEY，原则上不重新走流程就没有这个权限）。

**目前支持加密 SN 的设备**（截止 2026 年 3 月）：SQ58PRO、SQ310、SQ610、SQ630、SR5750、SQ53PRO、SQ68P、SQ610PRO。

## Memory mem_19ef01a38b8cdac8

- Kind: terminology
- Created-By-Email: patrick@urovo.com
- Created: 2026-09-11T22:10:09+08:00
- Updated: 2026-09-11T22:10:09+08:00

### Content

### 手板类型（外观手板 / 结构手板 / 功能手板）

- **外观手板**：内部什么样无所谓，只要外观保持一致就行了。纯模型。
- **结构手板**：除了外观之外，内部的结构也是按照图纸来设计的。纯模型。
- **功能手板**：支持完整功能，材质可能不一样（可靠性测试可能会有问题）。

Note: 通常说的"手板"就是功能手板，不然会指明"外观手板"或"结构手板"。做手办等于打样。

## Memory mem_a91e8f0b3bab493b

- Kind: fact
- Created-By-Email: patrick@urovo.com
- Created: 2026-09-12T16:33:45+08:00
- Updated: 2026-09-12T16:33:45+08:00

### Content

### SE2030S 扫描头补充参数（Urovo 自研标距扫描头）

SE2030S 是 Urovo 自研的 Standard Range（标距）扫描头（十字线瞄准），用于替代 Honeywell HS7。本条为其详细规格参数，与《扫描头选配指南》互为补充。

- 分辨率：1280 × 1080；像素：128 万
- 最小解析度：> 3 mil (1D)；> 6.7 mil (2D)
- 解析速度：20 times/s (1D)；10 times/s (2D)
- 准确率：理论上 100%
- 运动容差：2 m/s
- 光照：0 – 100,000 LUX

注：标距扫描头的读距口径为 60 cm for 13 mil UPC-A。

## Memory mem_0bc02931eb25ae9f

- Kind: fact
- Created-By-Email: patrick@urovo.com
- Created: 2026-09-12T16:35:04+08:00
- Updated: 2026-09-12T16:35:04+08:00

### Content

### 1D Laser Scanner vs. 2D Imager Scanner

#### 原理

- **1D Laser Scanner**：发出一束横向跳动的激光，通过感知返回光的强度差异（黑色吸收、白色反射）来解码。
- **2D Imager Scanner**：先拍照，再由扫码引擎芯片解码。

#### 2D Imager Scanner 相比 1D Laser Scanner 的优势

- 2D 可以扫二维码（QRCode、DataMatrix 等），1D 不行。
- 2D 可以扫描屏幕上的二维码，1D 不行。

#### Note

- UROVO 目前所有的扫码产品都是 2D Imager Scanner。
- 2D scanner 会有 Laser Aimer 和 Illumination，但这两者都只是外设，并非解码原理的一部分；没有它们也不影响 Decode 本身的能力。
- 普通摄像头虽然也是"拍照 + 软件解码"，但效率很低；2D scanner 是专门为该场景优化过的。

#### Summary

2D Imager Scanner 基本可以理解为完爆 1D Laser Scanner。1D Laser Scanner 是以前的扫码技术，除非客户有极其特殊的要求必须使用 1D Laser Scanner，否则 2D Imager Scanner 都能满足。

## Memory mem_f5db2b5d68e45026

- Kind: fact
- Created-By-Email: patrick@urovo.com
- Created: 2026-09-12T17:42:09+08:00
- Updated: 2026-09-12T17:42:09+08:00

### Content

### POS 激活卡更新（新激活卡 / 明华澳汉）

**通知要点**：为优化成本与安全性，导入新的 POS 激活卡。

- 新激活卡料号：`4.04.000.00029`
- 供应商：明华澳汉
- 目的：优化成本与安全性

### 兼容规则

- SQ28W / SQ29G、SQ27M / 29M / 65A：可**同时支持**明华卡 + 旧紫光国微激活卡。
- 新项目 65B / 65E / 68 / 68K / 69 / 69K：**仅支持明华卡**（不再兼容旧紫光国微激活卡）。

### 申领方式

通过 **RD14 - 安全维护工具及账号申请流程**办理领卡、制卡。

## Memory mem_22d11bc1e04d2ead

- Kind: fact
- Created-By-Email: patrick@urovo.com
- Created: 2026-09-12T18:37:46+08:00
- Updated: 2026-09-12T18:37:46+08:00

### Content

### RFID 自助结账方案的防损手段

RFID Self-Checkout 方案的防损一般包括以下四类措施：

- **Reading 调试优化**：通过 RFID 天线或读写器的不断调试，尽可能达到最好的 RFID 识读率。
- **RFID TAG 优化**：对于液体或者金属，尽量使用专门的 RFID TAG；对于经常漏读的商品，可以使用反射功率更大的标签。
- **人工检查**：一般多台 Self-Checkout Machine 会配一个人专门负责快速最终校验；对于 Self-Checkout Machine 没有读取到的商品，店员可以通过手持的 RFID 短距设备进行读取结账（DT50D）。
- **RFID 防盗门**：门口可以设置 RFID 防盗门，当检测到有商品没有结账成功的时候，就报警提醒店员。

### Note

- RFID 方案的优势是能够极大降低人工管理成本，以及提升客户的购物体验。
- RFID 本身不保证百分百的识别率，实际中基本要考虑"损失金额"这个指标。
- 对于客户相关的漏读顾虑，可以用"RFID 带来的降本远大于小概率漏读所造成的损失"来进行推广。

## Memory mem_2b1e50d6cbab731e

- Kind: fact
- Created-By-Email: patrick@urovo.com
- Created: 2026-09-12T18:39:45+08:00
- Updated: 2026-09-12T18:39:45+08:00

### Content

### D81R 接口配置（标配/选配）

- **标配**：USB
- **选配**：
  - 蓝牙 + WiFi
  - 网口（以太网）

即 D81R 出厂默认只带 USB 接口，蓝牙/WiFi 与网口均需按选配项下单。

## Memory mem_6c75655fc423131f

- Kind: fact
- Created-By-Email: patrick@urovo.com
- Created: 2026-09-12T18:43:03+08:00
- Updated: 2026-09-12T18:43:03+08:00

### Content

### K389 vs. K329（简易对比）

- **跌落/耐造程度**：K329 仅支持 **1.5 米**跌落，不耐造；K389 支持 **2.0 米**跌落，耐造。
- **适用场景**：K329 适合**零售门店**或**户外**场景（如快递）；K389 适合**仓储和制造**环境。
- **成本与寿命**：K329 **很便宜**，用个一年左右就可以换了；K389 更贵一些，但可以用更久。

### Note

- 一句话口径：K329 = 便宜轻量、零售/户外、1.5 米跌落；K389 = 更耐造、仓储/制造、2.0 米跌落、寿命更长。

## Memory mem_607c3b9203e1e4d4

- Kind: fact
- Created-By-Email: patrick@urovo.com
- Created: 2026-09-14T12:16:18+08:00
- Updated: 2026-09-14T12:16:18+08:00

### Content

### CE认证（欧盟市场准入认证）

1. RED（Radio Equipment Directive）相关

- 安规测试（Safety）：EN IEC 62368-1。电气/火灾/机械等安全测试，可以理解为"机器会不会伤人/出危险"。
- 电磁兼容测试（EMC）：EN 301 489。可以理解为"设备别干扰别人，也别轻易被干扰死"。
- RF合规性测试：NFC / RFID / 2G&3G&4G / GPS / BT / WiFi（2.4/5/6GHz）。
- 射频人体吸收测试（SAR）：发射无线电的时候，人体吸收了多少 RF 能量？

2. RoHS

### FCC认证（美国市场准入认证）

基本只包括 RF 合规性测试。

## Memory mem_7f5f7d621e830c99

- Kind: fact
- Created-By-Email: patrick@urovo.com
- Created: 2026-09-15T10:26:19+08:00
- Updated: 2026-09-15T10:26:19+08:00

### Content

### i2000 (SQ28W) 母POS 与密钥注入

- i2000（对应型号 **SQ28W**）是 UROVO 的**母 POS**，可用于给 POS 机**注入密钥**。
- 注入前需要先刷入**特定的 KLD 版本 OS**（**UFS 不需要**刷 KLD 版本）。
- KLD OS 版本号（Build Number）：
  `SQ28W_EN_KLD_WE__DS_FI_S01_U_251030_01_sq28w_kld.zip`

## Memory mem_379e7334f5cb8f31

- Kind: fact
- Created-By-Email: patrick@urovo.com
- Created: 2026-09-15T11:41:34+08:00
- Updated: 2026-09-15T11:41:34+08:00

### Content

### K388Pro_RFID 打印相关逻辑

- 只能写入标签（Tag Writer），不能当作 RFID Reader 使用。
- 支持带密码的 EPC 写入。
- 支持往 Reserved 区域写入 Access 密码。
- 支持锁住指定区域的数据（上锁后再次写入该区域需要密码）。
- 支持 EPC 写完后重新读回 EPC 进行校验，或失败重试。
- 支持 TID 回读后上传 Backend，用于 SKU-EPC-TID 的记录绑定。

### 打印流程逻辑

1. 先静止写入 EPC（或 User / Reserved 区域）。
2. 然后读回进行校验或其他业务逻辑（如 TID 回读等）。
3. 最后视情况对特定区域上锁。

## Memory mem_d6c459645126f316

- Kind: fact
- Created-By-Email: patrick@urovo.com
- Created: 2026-09-15T11:45:17+08:00
- Updated: 2026-09-15T11:45:17+08:00

### Content

### 售后物料料号的确定方法

确定售后物料的料号，有两种方式：

1. **根据设备 SN 查询（最精准）**：拿设备 SN 在系统上查该设备当时出货所用的物料。
2. **根据客户所需物料 + 当时出货的配置信息**：在售后 BOM 里面进行查找。

### 要点

- 优先使用按 SN 反查出货物料的方式，结果最准确。
- 当无法取得 SN 或客户只报了物料名称/配置时，才走售后 BOM 对照方式，需要同时掌握客户所需物料和当时的出货配置信息。

## Memory mem_903b6590941f665a

- Kind: fact
- Created-By-Email: patrick@urovo.com
- Created: 2026-09-15T12:04:57+08:00
- Updated: 2026-09-15T12:04:57+08:00

### Content

### Urovo 产品可靠性数据（寿命指标）

- POS 刷卡（磁条卡刷卡）：40 万次
- POS 插卡（IC 卡插拔）：20 万次
- PDA 一般按键寿命：100 万次
- PDA 扫描键寿命：300 万次
- USB 插拔次数：1 万次

用途：答复客户关于整机可靠性 / 寿命 / 耐久性测试指标的问题时使用。

## Memory mem_cc7b2bac6acd7de3

- Kind: fact
- Created-By-Email: patrick@urovo.com
- Created: 2026-09-15T21:56:07+08:00
- Updated: 2026-09-15T21:56:07+08:00

### Content

### Urovo 设备续航与充电时长的简易估算方法

1. 充电时长估算

- 普通充电 (5V/2A)：按 1250mAh/小时 计算
- 快充 (9V/2A)：按 2000mAh/小时 计算

2. 待机时长估算

- 常规：容量 / 20（小时）
- 极限：容量 / 10（小时）

3. 工作时长估算

- POS：仅亮屏约 16 小时；连续交易约 3 小时；正常使用约 12 小时
- PDA：仅亮屏约 16 小时；正常使用约 12 小时

## Memory mem_df97d8d7805921c7

- Kind: fact
- Created-By-Email: patrick@urovo.com
- Created: 2026-09-15T23:03:53+08:00
- Updated: 2026-09-15T23:07:17+08:00

### Content

### 无线蓝牙扫描器的连接/输出模式

#### K220: Multi-function Industrial Bluetooth Scanner（多功能工业蓝牙扫描器）

配对模式：

1. 蓝牙HID键盘模式：可直接与终端或电脑配对，随后作为HID键盘使用。
2. 底座模式（Docker Mode）：通过BT连接底座，底座再通过USB连接电脑。底座模式下的USB输出有三种：

- USB HID键盘模式：给电脑当作HID键盘使用。
- USB HID-POS模式：给电脑当作扫码设备输出，需要WMS软件在软件层面接收HID-POS数据（单纯输入框不会有文字输出）。
- USB CDC：用USB模拟串口；在Windows电脑上体现为一个COM虚拟串口，软件可通过对应COM口与扫码枪进行串口数据交互。

#### K180: SLIM; FASHIONABLE; Bluetooth Scanner（轻薄时尚蓝牙扫描器）

- 主要用于蓝牙HID键盘模式，其他模式都不常用。

Note: 底座只用来充电。

### Note（无线蓝牙扫描器通用）

- 常见设置项：Scan Mode（Trigger Mode；Pulse Mode；Continuous Mode）；Beeper；Illumination；Vibration。
- 重要条码：Factory Reset；Query Firmware version；Query Battery。
