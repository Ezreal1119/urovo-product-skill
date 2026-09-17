# K329 service manual

> Canonical original: `K329/others/maintenance-service-manual_202609112225/K329_Maintenance_Service_Manual.pdf`
> SHA-256: `af8fba512d870057c7bc1de8553fcab77263e991a0fd70b7fd72903940d74faa`
> Language: English (TOC/body). Cover logo UROVO TECHNOLOGY.
> Visual protocol: **16/16 pages** rendered and inspected. Photo-heavy disassembly / troubleshooting manual. Not a live product spec; lead hard specs from `K329/specs/`.
> Source spelling retained (e.g. Iterms, mainrboard is not used here; "Jam holder", "Pluse" is SR5600-only).

---

## Cover / TOC (page 1)

Cover photograph: black UROVO K329 mobile printer, front-right 3/4 view, translucent silver flip cover, orange latch on the right, POWER (left) and FEED (right) buttons flanking a small OLED, chassis text **UROVO | K329 MOBILE PRINTER**. Background dark blue. Right-side TOC card:

| # | Section |
| --- | --- |
| 1 | Photos |
| 2 | Mainboard interface |
| 3 | Disassembly |
| 4 | Troubleshooting |

Header logo: **UROVO TECHNOLOGY**.

## 1. Photos (page 2)

Callout labels (source spelling):

**Figure 1 — Top view:** Translucent flip cover; Open cover button (orange); Tear-off slot; POWER; FEED; OLED; chassis **UROVO | K329 MOBILE PRINTER**.

**Figure 2 — Rear view:** Label (regulatory plate on battery well, product name / 产品型号 **K329**, UROVO TECHNOLOGY CO.,LTD, CE and related marks); POGO pin (gold charging contacts on the rear-right); battery lock; battery; yellow tag **Rear view**.

**Figure 3 — Side view:** logo **UROVO | K329 MOBILE PRINTER**; OLED cover; NFC (top of orange latch area); USB (Type-C on the right side); yellow tag **side view**.

**Figure 4 — Open cover picture:** Rubber roller; Paper stop button (orange, inside bin); warning Label (yellow, in paper bin); printer head; yellow tag **Open cover picture**.

## 2. Mainboard interface (page 3)

Two board photographs:

- **P1 Mainboard front view:** green PCB, USB Type-C on the edge, Bluetooth module (metal shield), chips and connectors.
- **P2 Motherboard back view:** green PCB reverse.

Callouts: Motor interface; Thermal film interface; Main optical coupling interface; Display interface; Rubber roller optical coupling interface; Lithium battery interface; USB; Debugging interface; WIFI expansion interface; Bluetooth Module.

**USB Pin Definition**

| Pin | Definition |
| --- | --- |
| 1 | N/C |
| 2 | D- |
| 3 | D+ |
| 4 | GND |

## 3. Disassembly — assembly map (page 4)

Left table of replaceable items / failure modes; right exploded-style photos of sub-assemblies (Printer head, mainboard, Keypad, Flip cover assembly, Jam holder assembly, Middle frame components, Base assembly).

| Items | Details |
| --- | --- |
| Jam holder assembly | 1. Paper stop bracket (); 2. Paper stop button(). |
| Middle frame components | 1. Silicone plug (falling off); 2. Opening button (falling off); 3. Opening return spring (lost); 4. Display transparent cover (scratched, burned, stained, discolored); 5. Paper bin warning label (lost); 6. Battery seal (falling off). Plus: 1. POWER power button (interference); 2. FEED paper button (interference); 3. Paper tearing blade (loose); 4. NFC logo (worn and difficult to identify); 5. Silk screen (worn); 6. NFC electronic tag (failure). |
| Flip cover assembly | 1. Opening cover shaft (deformation, rust, etc.); 2. Opening cover torsion spring (elastic force damaged, reverse installation); 3. Optocoupler pressure block (deformation, breakage); 4. Rubber roller optical coupler FPC (sensor failure, wire short circuit, breakage); 5. Roller bracket (deformation, screw hole strain); 6. Shaft side sleeve, gear side sleeve (deformation, interference); 7. Shaft side bracket, gear side bracket (deformation, rust); 8. Gear (broken teeth); 9. Rubber roller (defective, deformed). |
| Base assembly | 1. Charger probe (falling off); 2. Battery slider (man-made damage, friction loss); 3. Battery wrench (cracked, broken); 4. Battery tension spring (elasticity loss, broken); 5. Screw hole rubber plug (falling off); 6. Battery sealing gasket (falling off). |
| Keypad | 1. Display screen seat (material deformation, breakage); 2. FPC cable (breakage, short circuit). Also: 1. Display screen (not lit); 2. Keyboard (short circuit, breakage). |
| Mainboard | 1. Bluetooth module/WIFI module (replacement). |
| Printer head | 11. Motor (abnormal noise, not working); 2. Movement body (interference); 3. Rotating hook, rotating hook tension spring (deformation, interference); 4. Gear 2, gear 3, gear 4, gear cover (paper slip); 5. Thermal film, thermal film compression spring (printing effect); 6. Main body optical coupler FPC (sensor failure); |

Source numbering "11." for the first printer-head motor item is retained.

## Steps to remove the lithium battery and base (page 5)

1. Turn the back of the machine upwards, slide the [battery slide] to the right, and then turn the bottom downwards, and the lithium battery will fall out naturally;
2. On the back of the machine, use tweezers to pick out the [screw hole rubber plug], and then use an electric screwdriver to remove the screws **PB2×6** (as shown in P1);
3. On the front of the machine, press the cover opening button to open the flip cover, and use an electric screwdriver to remove the screws **PB2×6** (as shown in P2);
4. At this time, the base is separated from the main body (as shown in P3).

**Visual — P1/P2/P3:** underside with battery removed, screw-hole plugs circled, two **PB2*6** screws; P2 front with flip open and two more **PB2*6**; P3 separated black base.

### Steps to remove the flip cover

1. After the base is separated, turn the bottom of the machine upwards and use the tip of the tweezers to push the left end of the cover opening shaft (as shown in P1①) to the right end;
2. Unplug the rubber roller optical coupler FPC line (as shown in P1②) from the main board, tear off a section of double-sided tape, and pass the FPC line through the opening;
3. At this time, the flip cover is separated from the main body (as shown in P2).

**Visual:** P1 underside with ① shaft and ② FPC highlighted; P2 detached flip-cover assembly.

## Jam remover / middle frame (page 6)

### Steps to remove the paper guide

1. After the cover is separated, turn the machine face up, pull the paper guide's [paper stopper button] vertically upward to the top, and then pull the paper guide upward along the moving track in the paper bin in a 135° direction (as shown in P1);
2. At this time, the paper guide is removed from the inside of the paper bin (as shown in P2).

**Visual:** P1 paper stop button / jam holder in the bin; P2 removed paper-guide part.

### Steps to remove the middle frame

1. After the base is separated, turn the bottom of the machine upwards and use an electric screwdriver to remove the four screws **PB2×6** (as shown in P1);
2. Turn the front of the machine upwards, hold it with both hands, and press down vertically with both thumbs to remove the movement from the middle frame (as shown in P2);
3. At this time, the middle frame is separated from the main body (as shown in P3).

**Visual:** P1 four screws on underside; P2 thumbs pressing the mechanism out; P3 empty grey middle-frame shell.

## Keypad / motherboard / movement (page 7)

### Steps to remove the keypad

1. As shown in P1, use an electric screwdriver to remove the two **PB2×4** screws, gently lift them up, and then remove the FPC cable connected to the motherboard;
2. At this time, the keypad assembly is removed from the main body (as shown in P2).

**Visual:** P1 keypad board with **PB2*4** and FPC; P2 keypad lifted showing OLED module on a green FPC.

### Steps to remove the motherboard and movement components

1. As shown in P1, use an electric screwdriver to remove the two screws **PB2×4**, lift it up gently, and then pull out the main optical coupler FPC, thermal film cable, and motor cable connected to the mainboard;
2. At this time, the mainboard is separated from the main body (as shown in P2).
3. At this time, the movement assembly is separated (as shown in P2).

**Visual:** P1 green mainboard in the chassis; P2 board removed beside the remaining metal/plastic movement.

## 3.1 Disassembly — Paper Jam Holder Assembly (page 8)

Replacement table (reason / same-type overall replacement = None / single material = paper stop bracket and paper stop button / steps / tools = Tweezers). Remark: In [Replacement Steps]: black letters indicate disassembly steps, red letters indicate assembly steps. Callout: If there is a problem with any of these two items, just replace a single material.

P1 locked vs unlocked states of the paper-guide; P2/P3 paper stopper button ears; P4 separated bracket and button; P5 two paper-guide tracks in the bin; P6 installing the paper guide vertically until a click.

How to remove the paper stopper button: when unlocked, clamp the two ears of the [paper block button] with tweezers, push the foot from the inside to the outside with the index-finger nail, then lift. Install: insert until a click; pay attention to front and back.

## 3.2 Middle frame assembly (page 9)

Replacement reasons include scratched/burned/stained/discolored/deformed middle frame or blurred logo; cracked screw posts; if the same type of 6 integrated processes are damaged, replace the middle frame. Same-type overall replacement: POWER / FEED / tearing blade / NFC logo. Single material: silicone plug, opening button, return spring, display transparent cover, paper bin warning label, NFC electronic tag, battery seal.

Tools: Cross screwdriver; Tweezers; Anti-static wrist strap; Pressing machine fixture.

Notes: ① Replace the middle frame of the same type as a whole; ② Replace only individual materials for a single material; ③ Replace the tear blade, paper feed button, and power button. ④ Prevent the cover opening button from flying when in use. Tweezers are used for assembly. After assembly, check whether the elastic force is normal.

**Visual P1–P4:** grey middle-frame shell; POWER/FEED buttons and tear blade; NFC logo area; silicone plug / opening button close-ups.

## 3.3 Flip cover assembly (page 10)

Same-type overall replacement: none. Single-material list matches page 4 flip-cover items. Tools include rubber roller pressing jig.

Replacement steps include removing battery, base (4 screws), flip cover (tweezers push shaft), rubber roller assembly (8 screws), then reverse assembly; manually turn the rubber roller gear (must slide flexibly); insert cover opening shaft with tweezers (elastic force flexible).

**Visual P1–P10:** numbered ①–④ on a roller/bracket photo; exploded roller, gears, shaft, torsion spring, optocoupler FPC, sleeves and brackets.

Notes: ① Check that the rubber roller is in good rolling condition when disassembling it; ② The torque of the electric screwdriver needs to be adjusted properly.

## 3.4 Base assembly (page 11)

Same-type overall replacement: Rubber plug for the lanyard hole (broken by human factors, loss of function). Single material: charger probe, battery slider, battery wrench, battery tension spring, screw hole rubber plug, battery sealing gasket. Tool includes constant temperature soldering iron.

Notes: ① After the battery slider is installed, check whether the elastic force is normal; ② If the rubber plug of the lanyard hole is damaged, the entire base needs to be replaced; ③ The charging probe can be pushed out vertically; ④ The rubber plug of the lanyard hole needs to be ironed flat with a soldering iron.

**Visual P1–P3:** underside of base with slider/wrench/spring; charging probes; lanyard-hole rubber plug.

## 3.5 Button board / keypad assembly (page 12)

Reasons include OLED not lit (buzzer will sound); button interference; keypad not working; OLED not fixed firmly; FPC short; 10PIN-FPC socket damaged. Same-type: display / keyboard. Single: display screen seat / FPC cable.

Note: When installing the keypad, first plug in the Type-C cable to check whether the screen lights up when powered on.

**Visual:** keypad/OLED assembly photos (page is table-dominant; OLED board visible in the earlier page-7 sequence).

## 3.6 Motherboard (page 13)

Same-type overall replacement: None. Single: Bluetooth module/WIFI module (replace as needed). Tools: Cross screwdriver; Tweezers; Constant temperature soldering iron; Air gun; Anti-static wristband.

Notes: ① Wear an anti-static wristband when replacing; ② When replacing the WIFI module, the Bluetooth module needs to be removed.

**Visual P1 front / P2 back:** green PCBs with yellow boxes highlighting the Bluetooth / Wi-Fi module area.

## 3.7 Movement components (page 14)

Source heading spelling: **Iterms**. Replacement of movement components. Single-material list: Motor; Movement body; Rotating hook and tension spring; Gear 2/3/4 and gear cover; Thermal film and compression spring; Main body optical coupler FPC; Paper guide block.

Notes: ① Whether the gear is installed correctly, the gear needs to be coated with damping oil; ② The thermal sheet spring should be installed neatly.

**Visual P1–P10:** movement body, motor, gears with damping oil, thermal film, springs, FPC, paper guide block; numbered ①–④.

## 4.1 Troubleshooting (page 15)

| Question | Possible Causes | Solution |
| --- | --- | --- |
| OLED screen does not display | Batteries not inserted; Batteries are low. | Insert the battery; Charge the battery. |
| OLED screen error handling | Warning: "Please close the cover"; Warning: "Please load paper"; Warning: "Overheat protection". | Close the paper cover correctly; Replace a new paper roll; When the temperature of the thermal head drops, printing will resume automatically. |
| Do not print | Paper installation error; Mainboard damage; Thermal chip connection error; Thermal chip damage; Label size setting incorrectly; Exceeding the maximum printing width. | Install the paper roll correctly; Replace the main board; Connect the thermal head cable correctly; Replace the thermal film; Set the correct label size; Replace the paper roll with the maximum width. |
| Partially not printed | The thermal film is connected incorrectly; One side of the paper compartment cover is not fastened tightly; The thermal film is damaged. | Connect the thermal film cable correctly; Close the paper compartment cover correctly; Replace the thermal film. |
| Wrinkle problem | Uneven thermal film pressure; Incorrect label paper installation; Incorrect print density; Incorrect label paper feeding. | Please set the appropriate label printing density; Please adjust the label width adjuster to suit the label width. |
| Blurred printing | The label paper is not installed correctly; Dust or adhesive is accumulated on the thermal film; The print density is not set correctly; The thermal film is damaged; The battery voltage is low; One side of the paper compartment cover is not fastened; The rubber roller is installed incorrectly; The maximum print thickness exceeds 0.15mm. | Reinstall the printing consumables; Clean the thermal film with a cloth dipped in alcohol; Clean the rubber roller with a soft brush; Set the appropriate printing speed and printing density; Print the self-test page to check whether the thermal film is damaged. If so, please return to the factory to replace the thermal film; Choose label paper that meets the specifications; Confirm that the thermal film bracket is completely closed. |
| Paper skipping problem | The label size is set incorrectly or incompletely; The label sensor is covered by foreign matter, causing incorrect detection. | Re-adjust the specification and print; Humidity reduces the gap value and prints; Remove foreign matter between sensors. |
| Broken needle problem | There is dirt on the print head; The rubber roller is dirty. | Clean the print head; Clean the rubber roller. |

## 4.2–4.4 Calibration / self-test (page 16 / printed 17)

### 4.2 Gap Sensor Calibration

1. Long press the POWER button to turn on the printer;
2. Press the cover open button. If there is no paper in the paper bin, the OLED screen prompts **"Please load paper"**;
3. After correctly installing the label paper, check whether it is in the gap paper mode. If so, close the cover;
4. Press the FEED paper feed button for **0.2S** and release it. Wait for the printer to output paper. When a label paper is output, it stops at the gap and feeds another paper in the same way. If the paper feeding position is the same, it means that the calibration is successful. (As shown in the right picture)
5. Calibrate the black label paper in the same way.

**Visual — right photo:** printer with white gap labels feeding; OLED shows **Ready**; chassis **urovo K329 MOBILE PRINTER**.

### 4.3 Cover open sensor verification

1. Long press the POWER button to turn on the device;
2. After pressing the cover opening button, the OLED screen prompt changes from **"Ready"** to **"Please close the cover"**, indicating that the sensor performance is good. Close the cover again, and the OLED screen prompt changes from **"Please close the cover"** to **"Ready"**, indicating that the sensor performance is normal;

### 4.4 Print a self-test page

1. When the printer is turned on, press and hold the FEED button for 2 seconds to enter the setup mode;
2. Continue to short-press the FEED button to select **"Print self-test page: Off"**, then short-press the POWER button and wait for the printer to eject paper.

**Visual — self-test receipt (CONFIGURATION):**

| Field | Printed value |
| --- | --- |
| SN | U21069300061R |
| VERSION | 3.1.17 |
| DARKNESS | 8 |
| MEDIA TYPE | CONTINUE |
| POWER OFF TIME | 60MIN |
| BLUETOOTH NAME | K329_41F1 |
| BLUETOOTH ADDR | DC003BC141F1 |
| BLUETOOTH PIN | 0000 |
| DRAM FILE | 0 FILE(S) |
| FLASH FILE | 0 FILE(S) |

Also printed: `DC003BC141F1`; `GB18030 UNICODE简体中文字符集`; `B165码繁体中文宋元`; `Korean KSC5601`; `SourceHanSansCN.TTF`; a QR code on the receipt. These are values from the photographed sample printer, not catalog claims.

OLED on the lower photo: **Ready**.

Coverage check: 16/16 pages inspected.
