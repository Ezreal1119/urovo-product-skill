# RT40 Service Manual v1.0

> Canonical original: `RT40S/others/service-manual_202609121547/RT40_Service_Manual.doc` (bytes and filename unchanged).
> SHA-256: `8cb512eb393baa8754141044476f8a377d64a3318689be17d705dc28826f2732`
> Companion inspection PDF was generated only for vision; it is not a canonical source.
> Visual protocol: **16/16** converted-PDF pages; **46/46** embedded `word/media` files inspected.
> Body title **RT40 Service Manual v1.0**. Record of updating: **2022-12-13** / **WuDongni** / **v1.0** / “This is a documentation of RT40 maintenance.”
> Zero **RT40S** / **SQ47S** / **SQ47SP** strings. Routed to the **RT40S** Hub by user decision; retain the source **RT40** label.
> Interior footer (CN/EN): **深圳市优博讯科技股份有限公司** / **Shenzhen Urovo Technology Co., Ltd.** / 深圳市南山区学府路63号高新区联合总部大厦36楼 / Fl. 36, United Headquarters Bldg., High-tech Zone, No. 63, Xuefu Rd., Nanshan Dist., Shenzhen, Guangdong, China / Tel: (86) 755 8618 6300 / Fax: (86) 755 8618 6290 / www.urovo.com / **第 N 页 共 16 页** / **Page N of 16**.
> Header logo: UROVO / 优博讯 and the U mark.
> Parts table names an **EX30 reader** (also present on the RT40S after-sales BOM). Not a live spec. Lead hard specs from `RT40S/specs/`.

---

## Cover / Record of updating / Content (page 1)

**RT40 Service Manual**  
**v1.0**

| Date | Author | Version | Description |
| --- | --- | --- | --- |
| 2022-12-13 | WuDongni | v1.0 | This is a documentation of RT40 maintenance. |

| Section | Printed page |
| --- | --- |
| I. Product Appearance | 2 |
| II. Accessories | 2 |
| III. Disassembly Procedure | 6 |
| 1. Remove the Back Cover | 6 |
| 2. Remove the Reader Bracket/Motherboard | 7 |
| 3. Remove the Reader | 8 |
| 4. Remove the Main Antenna and KB Board | 9 |
| IV. Parts | 11 |

## I. Product Appearance (page 2)

**Visual:** front studio shot of a black keypad handheld. Dark unlit display; physical numeric keypad with grey/white keys; function-key row above the keypad; scan-engine hood at the top; slim orange-tinted side keys. No on-screen UI text. No rear / side views on this page.

Empty accessories table header below: **Name** | **Picture**.

## II. Accessories (pages 2–6)

Three-column layout on later pages: name | photo | notes.

| Name | Notes (source text) | Photo (visible evidence) |
| --- | --- | --- |
| Power adapter | QC3.0 fast-charging adapter. Input: 100-240V~50/60Hz 0.6AMAX. Output: 5V/3A, 9V/2A, 12V/1.5A | Black USB-A wall wart, two-pin plug |
| Type-C cable | Applicable to charging and data transmission. Interface type: Type-C | Black USB-A to USB-C cable |
| Battery | Removable 3.85V 5200mAh Polymer battery | Black pack with gold pogo contacts on the top edge and a regulatory label on the face (sample photo; not a catalog SN) |
| Charging cradle (optional) | Support charging one device and one battery simultaneously. Support charging standard device and pistol grip type device. Support charging device with TPU protective case. Support LED charging status indicator. DC charging port. Type-C data interface. Charging dock adapter output: **12V/2A** | Black single-slot cradle, **urovo** wordmark on the front face |
| 4-slot battery charger (optional) | Support charging four batteries simultaneously. Support LED charging status indicator. DC charging port. Charging dock adapter output: **12V/5A** | Black 4-bay battery charger |
| 5-slot charging cradle (5 devices) (optional) | Support charging five devices simultaneously. Support charging standard device and pistol grip type device. Support charging device with TPU protective case; and support LED charging status indicator. DC charging port. Charging dock adapter output: **12V/5A** | Black 5-bay device charging gang |
| 5-slot charging dock (4 devices + 4 batteries) (optional) | Support charging four devices and four batteries simultaneously. Support charging standard device and pistol grip type device. Support charging device with TPU protective case; and support LED charging status indicator. DC charging port. Charging dock adapter output: **12V/10A** | Black combo dock: four device bays + four battery bays |
| Hand strap -1 (optional) | Applicable to standard device | Black wrist / hand strap with a clip |
| Hand strap -2 (optional) | Applicable to pistol grip type device | Black strap (pistol-grip variant) |
| TPU protective case (optional) | Applicable to standard device, pistol grip device, enhanced protection and protective device | Black TPU boot / bumper frame |

## III. Disassembly Procedure

### 1. Remove the Back Cover (page 6)

Remove **12 hexagon screws** on the case and then remove the SIM waterproof plug.

Remove the rear cover by gently prying along the gap of the rear cover.

**Visual:** rear of the keypad handheld, battery well empty; **12 red-circled hex screws** around the perimeter (including the scan-hood pair). SIM waterproof plug called out at the card-slot area.

### 2. Remove the Reader Bracket/Motherboard (pages 7–8)

First remove the **three screws** on the motherboard and the **four screws** on the reader bracket, then remove all BTB clamps from the motherboard, and remove the motherboard and bracket.

Remove the **four screws** on the motherboard and then take out the motherboard; when taking out the motherboard, remember to remove the **reader FPC** first.

**Visual:** opened chassis, green mainboard still seated; reader bracket at the top. Isolated mainboard (top and bottom faces) with a UROVO barcode sticker on the shield. Red callouts on motherboard / bracket screws and the reader FPC.

### 3. Remove the Reader (page 9)

Remove the screws fixing the reader and then directly take out the reader.

Finally, take out the camera, large capacitor, flash light and FPC in turn.

**Visual:** scan-engine / **EX30-class reader** in the bracket; then the engine removed. Separate photos of the rear camera, cylindrical large capacitor, LED/flash + MIC FPC, and reader cable laid on the bench.

### 4. Remove the Main Antenna and KB Board (pages 10–11)

First remove the **three white screws** on the main antenna bracket and **four black screws** on the KB board; remove **one screw** on the USB board, and remove the FPC that connects the USB board to the KB board, the main FPC that connects the KB board to the motherboard, and the coaxial cable in sequence.

**Visual (page 10–11):** remaining front-shell stack after the mainboard is out — KB board over the keypad, antenna bracket, USB / I/O board at the bottom. Coaxial and interconnect FPCs visible. Isolated KB board and USB board on a green backdrop.

## IV. Parts (pages 12–16)

Header: **RT40 main maintenance parts**. Columns **Part Name** | **Picture**.

| Part Name | Photo (visible evidence) |
| --- | --- |
| Back cover | Rear housing with scan-hood cutout |
| Display | Front display + keypad assembly |
| Motherboard | Green / shielded mainboard |
| KB board | Keyboard PCB |
| EX30 reader | Scan-engine module |
| Rear camera | Camera module |
| LED/MIC FPC | Flex with LED / microphone |
| Reader cable | Scan-engine FPC |
| Foam | Small foam pad |
| Large capacitor | Cylindrical capacitor |
| Reader bracket | Black scan-engine bracket |
| USB board | I/O / USB PCB |
| FPC connecting the KB board and USB | Short interconnect FPC |
| Main antenna bracket | Antenna bracket |
| FPC connecting the MB and KB | Longer interconnect FPC (row repeats on page 15) |
| NFC | NFC coil / antenna module |
| Horn | Speaker |

**RT40 maintenance parts** (screws):

| Part Name | Picture |
| --- | --- |
| Screw 1 | Longer black screws |
| Screw 2 | Medium black screws |
| Screw 3 | Short silver / black screws |
| Screw 4 | Small black screws |
