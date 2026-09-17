# 电子价签规格书 — 4.2英寸系列（ET0420）

> Canonical original retained (bytes unchanged). Text layer plus visual inspection of all 8 rendered pages.
>
> - Original: `ESL/others/spec-4.2inch_202608182031/ESL-4.2inch-Specs.docx`
> - Header: 4.2英寸系列 / ET0420 系列
> - Version: 3.0，2026/2/2，编写者唐存社（描述：增加4色标签产品）
> - Pages: 8/8 inspected
> - Website in footer: https://www.urovo.com

---

## Cover (page 1)

Same cover family as the 2.1-inch spec: **电子价签 规格书** / **ELECTRONIC SHELF LABEL SPECIFICATIONS**, blue digital-city background, four ESL mockups (Organic Green Tea $8.50; Salmon €3.99; BIG SALE $15.99 with barcode/QR; 55" TV $399).

## Revision (page 2)

Header: **4.2 英寸系列**. Page 2 / 8.

| 版本号 | 描述 | 发布日期 | 编写者 |
| --- | --- | --- | --- |
| 3.0 | 增加4色标签产品 | 2026/2/2 | 唐存社 |
|  |  |  |  |
|  |  |  |  |

## 目录 (page 3)

1. 简要描述 — 4
2. 产品优势 — 4
3. 产品规格 — 5
4. 图纸 — 7
5. 网络结构 — 7

## 1. 简要描述 (page 4)

优博讯一直致力于推动电子纸技术的应用，利用其低功耗和可重复使用的特点，减少对环境的破坏，并提升工作效率。

电子货架标签（ESL）解决方案通过自动更新价格，简化了运营流程，提供了比纸张更具成本效益的替代方案。它通过提供精准、一致的定价，提升了顾客的购物体验，通过其ESL平台和API集成，帮助零售商实现最佳的业绩。加速了店内数字化转型，支持无缝的价格管理、运营优化、个性化服务和预测分析。

4.2系列ESL标签配备400×300高分辨率显示屏，可适应各种销售场景。它支持文本、促销信息、二维码或条形码显示，并且可以重复使用，无需纸张。该电子标签除零售外还可应用于其他场景，如各种物流、仓储、智能家居等。

## 2. 产品优势 (page 4)

- 提供多种颜色模式（双色，三色和四色）可选。
- 支持客户端ESL管理系统的云服务器（MQTT）和本地服务器的部署。
- 通过手机应用程序直接使用蓝牙管理价格标签，无需基站。
- 基站内置ESL管理系统，能够独立运行，无需服务器。(可选)

## 3. 产品规格 (pages 5–6)

### 3.1 产品分类（ET0420-84）

Front photo: ~square 4.2-inch e-paper sample with **400x300**, black/white/red content, price **$ 35.98 / kg**, “100% local” badge, barcode. Back: mounting clips, CE/FCC/RoHS marks, model sticker.

Source table header is **基站版本型号** (wording as printed):

| 基站版本型号 | 显示颜色 | 特点 | 手机APP版本型号 |
| --- | --- | --- | --- |
| ET0420-84 | 红色，黄色，黑色和白色 | 4色 | 价签管理1.0.1 |
| ET0420-42 | 黑白双色 | 快刷 | NFCDemo1.0.1 |

### 3.2 技术规格

|  |  |
| --- | --- |
| 外形尺寸 | 99.16mm(H)×89.16mm(V)×12.3mm(D) |
| 工作温度 | 0℃~40℃（3色，4色）；0℃~50℃ (黑白双色) |
| 操作湿度 | 45%~70%RH |
| 保护等级 | IP65(默认） IP68（可选） |
| LED灯 | 红、绿、蓝三原色，支持7种颜色 |
| 无线通信 | 蓝牙5.0私有协议 |
| 图片更新 | 超过30000个/小时（500个/分钟） |
| 通信频率 | 2.400-2.480 GHz，最大 EIRP ≤ 10mW |
| 通信距离 | 30米以内（空旷地区50米） |
| 通讯方式 | 基站或者手机APP |
| 重量 | 82 g |
| 包装标准 | 180个/箱，15.76 Kg, 390mm×350mm×240mm |

### 3.3 电子纸屏幕

|  |  |
| --- | --- |
| 尺寸 | 4.2 寸 |
| 分辨率 | 400(H)×300(V) |
| DPI | 119 |
| 有效区域 | 84.8mm(H)×63.6mm(V) |
| 视角 | >170° |
| 屏幕显示颜色 | 黑白红黄4色 / 黑白红3色 |

### 3.4 电池

|  |  |
| --- | --- |
| 内置电池 | CR2450 x 3 |
| 电池续航时间 | 不低于7年（行业领先） |

### 3.5 特性

|  |  |
| --- | --- |
| NFC功能 | 支持(可选) |
| 无线固件更新 | 支持 |
| 可用的页面 | 8页 |
| 外壳颜色 | 白色/黑色 (可选) |
| 符合认证 | CE, RoHS, FCC, MIC, SRRC |

### 3.6 功能

| 编号 | 分类 | 描述 |
| --- | --- | --- |
| 1 | 数据显示 | 支持任何语言文字、图片、符号等其他内容的传输和显示。 |
| 2 | NFC | 支持NFC通信。(可选) |
| 3 | 温度检测 | 每个标签都支持温度采样，并且系统可读取。 |
| 4 | 电量检测 | 每个标签都支持功率采样功能，其中可以被系统读取。 |
| 5 | LED灯闪烁设置 | 支持LED 3色独立控制灯。每盏灯闪烁频率为1次/秒。每盏灯的闪烁次数可由用户设定。 |

## 4. 图纸（单位：mm）(page 7)

- Front: **99.16 mm** × **89.16 mm**
- Side: rear protrusion **3.54 mm** deep × **3.79 mm** high
- Thickness: total **12.3 mm**; main body **6.5 mm**

## 5. 网络构架 (page 7)

Same family diagram as the 2.1-inch spec: LAN + Internet/cloud, Network users, WMS server, ESL server, Controllers; mobile user via **TCP/IP**; one gateway **2.4G** to light tower and ESL; another path **Bluetooth** to a handheld then ESL.

## 6. 为什么选择我们 (page 8)

| Topic | Text | Visual |
| --- | --- | --- |
| **本地云服务器** | 我们为客户提供专用云服务器的设置，它最大限度地减少了对外部云提供商的依赖，确保您的ESL系统更可靠和更具成本效益的管理。 | Cloud-infrastructure diagram (Data Storage, Tools & Services, Data Protection, Local Servers/Nodes, User / User Cloud Instance) |
| **API管理** | 我们将提供一个强大的API接口，将我们的ESL系统无缝集成到他们的平台中，为最终客户提供一个更强大、更灵活、更有竞争力的解决方案。 | Circular infographic: 01 API Design, 02 API Gateway, 03 Developer Portal, 04 API Lifecycle Manager, 05 API Dashboard |
| **强大的基站** | 低错误率；可与企业管理系统对接；适合零售、仓储、物流管理；支持云服务器或本地服务器. | Photo of a white square base station with LED display **8.8.8.8.** |
| **多功能性** | ESL有各种尺寸和规格，以满足任何应用环境的不同需求。可以定制多种功能，以增强客户体验。 | Supermarket-aisle lifestyle photo |

## Visual coverage

8/8 pages inspected.
