# SR5600 Bluetooth Ring Scanner User Guide

> Canonical original: `SR5600/user_guide/default_202609112225/Urovo-SR5600-2D-Wearable-Ring-Barcode-Scanner-User-Manual.pdf`
> SHA-256: `9dc53be05100067d76605b320aa2242280174dba4ef0b3d506d2982d776e3be3`
> Cover: **SR5600 [USER GUIDE] [F.2021.07.12].2 Bluetooth Ring Scanner**
> Revision history: 2021.06.15 first version through **2021.08.08 Version 1.2** (prefix/suffix, barcode type, Bluetooth name modifying). No SR5600 V2 identification.
> Visual protocol: **49/49** pages rendered and inspected.
> First user-guide slot for this Hub. Lead hard specs from product brochure/spec sources; this is a 2021 operation / programming guide.


## Visual protocol notes (49/49 pages)

Cover (page 1): teal left panel **UROVO**; title **SR5600 Bluetooth Ring Scanner [USER GUIDE]**; line-art of the ring scanner (imager window, trigger, finger strap). Footer **UROVO [F.2021.07.12].2**. No V2 branding.

Page 2 Revision History table as in the text layer. Page 3–4 Index.

**Page 5 Figure 1 SR5600 Trigger Configuration Features** (source spelling **NFC Aera** retained): line drawings of the scanner body and imager head. Callouts: Battery; Battery buckle; Top Scan Trigger; NFC Aera; Indicator; Imager window; POGO PIN. Trigger face shows **OVOIN**.

**Page 6:** exploded battery install: Cord buckle, Strap buckle, Finger Straps, Trigger Assembly; Direct Charger with Type C; Ring buckle; POGO Pin. LED table as text.

**Page 7:** battery insert photo with **Battery buckle**; **Power button** and **Side Scan Trigger** on the imager head.

**Page 8:** Figure1 right-finger / Figure2 left-finger trigger assembly; **Sliding buckle**; finger-strap adjustment with **Finger Strap** and **Strap Buckle**.

**Page 9:** Direct Charger clip-on with **Type-C**; power button on imager (red callout). Long-press 2 second boot / 3 second off.

**Pages 10–11:** Code 128 programming barcodes. Captions: Human Interface Device(*HID MODE), Serial Port Profile(SPP MODE), Low Energy(BLE MODE); Pairing Mode; Bluetooth Name Modifying (`$BT#SETSSID=M`). HRI under the mode barcodes is of the form `%NUS-3400xxxxN%` (digits confirmed on HID as **34000282** in the page-10 render). Remaining HRI strings that were too small to resolve digit-by-digit are not guessed.

**Page 12 Android screenshot:** Settings > Connected devices path; **Bluetooth** toggle On; AVAILABLE DEVICES includes **SR5600-0128** (sample). Fast-connect notes: Android NFC tap-to-pair; QRCODE of U2 wearable Bluetooth MAC.

**Pages 13–15 Windows screenshots:** Windows 10 Bluetooth settings, **Add a device**, discovered **SR5600-0128** / Ready to go. Default PIN **0000**. Page 15 footer `<Test in text file.>` and a numeric string `37875815737188` under a sample device-ready dialog (screenshot-only; not a catalog SN).

**Pages 16–49:** programming-barcode pages. Each option in the text layer corresponds to a Code 128 symbol with a printed caption (Enable/Disable/default `*`). Some later symbology pages use HRI of the form `#-INS.%xxxxS00%#-` (e.g. MSI/PLESSEY, Dotcode, Standard 2 of 5). Captions and defaults below are from the text layer and were confirmed against the page renders. Source spellings retained: **Pluse**, **Austranlian Post**, **Hanxincode**, **postnet**, **CodaBlock_F**, **NEC 2of 5**, **MicrE-13 B**. Android HID steps also print **The RS5100 displays as SR5600 - xxxxxx**.

Page numbering in the footer is 1–45 after the front matter (PDF pages 5–49).

---

## PDF page 1

SR5600
[USER GUIDE]
[F.2021.07.12].2
Bluetooth Ring Scanner



## PDF page 2

Revision History
Change
Date
Description
Author
-2
2021.06.15
First version
Liang Wang
-1
2021.07.12
Initial Release
Nolan Luo
0
2021.07.15
Version 1.0 Revision
Nolan Luo
1
2021.07.29
Version 1.1 Revision
Nolan Luo
2
2021.08.08
Version 1.2 Revision

Add prefix/suffix setting

Barcode type

Bluetooth name modifying
Nolan Luo



## PDF page 3

Index
Revision History...................................................................................................................................2
1. Getting Started................................................................................................................................ 1
1.1 Introduction...........................................................................................................................1
1.2 Unpacking..............................................................................................................................1
1.3 Configuration Features..........................................................................................................1
1.4 LED Status Indications........................................................................................................... 2
1.5 Buzzer, vibration status......................................................................................................... 3
1.6 Battery installation instructions............................................................................................3
1.7 Trigger Assembly................................................................................................................... 4
1.7.1 Installation instructions..............................................................................................4
1.7.2 Adjust finger strap......................................................................................................4
1.8 Direct Charger installation instructions................................................................................ 5
1.8.1 Powering ON/OFF...................................................................................................... 5
1.9 Bluetooth Communications.................................................................................................. 6
1.9.1 Introduction................................................................................................................6
1.9.2 Bluetooth Connection Modes....................................................................................6
1.9.3 Pairing Mode..............................................................................................................7
1.9.4 Bluetooth Name Modifying....................................................................................... 7
2. Setup................................................................................................................................................8
2.1. HID Bluetooth Connection to iOS/iPad/iPhone...................................................................8
2.2 HID Bluetooth Connection to Android..................................................................................8
2.3 HID Bluetooth Connection to Windows................................................................................9
2.4 Power Save.......................................................................................................................... 12
2.5 Delay 01~10 ms to send (HID).............................................................................................12
2.6 Firmware Version................................................................................................................ 12
2.7 Restore Factory Setting....................................................................................................... 13
2.8. Indicators & Beeper setting................................................................................................13
2.8.1. Power on alarming..................................................................................................13
2.8.2. LED indicator........................................................................................................... 14
2.8.3. Beeper setting.........................................................................................................14
3. Scanner Setting..............................................................................................................................16
3.1. Scanning Type.....................................................................................................................16
3.2. Illumination&Aiming setting..............................................................................................16
3.3. Illumination level................................................................................................................17
3.4. Suffix&Prefix.......................................................................................................................18
4. Symbologies...................................................................................................................................21
Code 39......................................................................................................................................21
Code 39 Full ASCII..............................................................................................................22
PDF417.......................................................................................................................................22
Data Matrix................................................................................................................................23
Interleaved 2 of 5...................................................................................................................... 23
MaxiCode...................................................................................................................................24
UPC/EAN....................................................................................................................................25



## PDF page 4

Code 93......................................................................................................................................26
Code 11......................................................................................................................................26
Matrix 2 of 5..............................................................................................................................28
NEC 2of 5...................................................................................................................................28
Hanxincode................................................................................................................................29
GridMatrix................................................................................................................................. 29
Aztec Code.................................................................................................................................30
MicroPDF417.............................................................................................................................30
MSI/PLESSEY..............................................................................................................................31
Dotcode..................................................................................................................................... 31
Standard 2 of 5.......................................................................................................................... 32
CodaBlock_F..............................................................................................................................32
CodaBlock_A..............................................................................................................................33
GS1 DataBar-14......................................................................................................................... 33
Codabar..................................................................................................................................... 34
Code 2 of 5................................................................................................................................ 34
Trioptic.......................................................................................................................................35
postnet...................................................................................................................................... 35
China Post..................................................................................................................................40
OCR............................................................................................................................................41
Decoding............................................................................................................................41
OCR Pattern.......................................................................................................................42
OCR Fonts.......................................................................................................................... 43
OCR Character................................................................................................................... 44
OCR Character length : 00~FF........................................................................................... 45



## PDF page 5

1
1. Getting Started
1.1 Introduction
This chapter describes the features of the SR5600 Ring Scanner and explains
how to install and charge the battery, capture data and reset the SR5600.
1.2 Unpacking
Carefully remove all protective material from around the equipment and save
the shipping container for later storage and shipping.
After opening the shipping box, inspect the contents. You should have received
the following:

SR5600

Battery

Simple Operation Guide

USB Cable

Power adaptor

Direct Charger
Inspect the equipment for damage. If you are missing any equipment or if you
find any damaged equipment, contact Support immediately. See Website:
http://en.urovo.com or local agent.
1.3 Configuration Features
Figure 1 SR5600 Trigger Configuration Features



## PDF page 6

2
1.4 LED Status Indications
Status light
Description
Red indicator light is always on
Trigger button hold or charging
Red indicator light flashes once
Setup failure
Red indicator blinking twice
Alarming/Scanning when Bluetooth is not
connected
Green indicator light flashes once
Scan bar code successfully
Green indicator light is always on
Battery fully charged
Blue indicator light keeps flashing
Bluetooth enters pairing mode
Blue indicator solid on
Successful Bluetooth connection



## PDF page 7

3
1.5 Buzzer, vibration status
Buzzer, vibration status
Description
Start-up sound + no vibration
Startup
One long buzz + vibration
Shutdown
One short buzz + vibration
Successful decoding
Two short buzz + no vibration
The battery is set successfully, the Bluetooth is
connected successfully, and the Bluetooth is
disconnected
One long buzz + no vibration
Setup failure
Four short beeps + vibration
Alarming/Scanning
when
Bluetooth
is
not
connected
1.6 Battery installation instructions
Align the battery with the top of the SR5600 and insert it into the battery compartment.
Slide the battery all the way into the SR5600 locking slot to ensure that the battery matches
with SR5600.



## PDF page 8

4
1.7 Trigger Assembly
1.7.1 Installation instructions
Align one end of the SR5600 lock catch and push the other end down until it clicks into
place.
The trigger assembly can be installed as required. The following figure 1 is for the right finger,
and figure 2 is for the left finger.
Press the sliding buckle to remove the ring.
1.7.2 Adjust finger strap



## PDF page 9

5
1.8 Direct Charger installation instructions
Insert the bottom of the SR5600 into the charger until it clips into place. Connect the Type-C
interface at the end of the charger with the USB cable and Power adaptor. Normal charging
starts when the indicator light indicates that the red light is always on.
1.8.1 Powering ON/OFF
Long-press the power button for 2 second to boot, for 3 second to turn off.



## PDF page 10

6
1.9 Bluetooth Communications
1.9.1 Introduction
This chapter provides information about the modes of operation and features available or
Bluetooth communication between Ring Scanner and hosts. The chapter also includes the
parameters necessary to configure the SR5600.
Scan a factory barcode to return all features to default values. See page10.
Scan a version barcode to check the version number of the scanner. See page10.
1.9.2 Bluetooth Connection Modes
The SR5600 Ring Scanner can connect to a host computer using the following Bluetooth
modes, scan to switch the connection mode you need:
Human Interface Device(*HID MODE)
Serial Port Profile(SPP MODE)
Low Energy(BLE MODE)



## PDF page 11

7
1.9.3 Pairing Mode
Scan the following barcode to enter the pairing mode or release the connection.
1.9.4 Bluetooth Name Modifying
Generate the barcode to change the Bluetooth name, value = $BT#SETSSID=M
M: Bluetooth name of Ring Scanner SR5600.



## PDF page 12

8
2. Setup
HID Setup
2.1. HID Bluetooth Connection to iOS/iPad/iPhone
1. Scan the barcode ‘Pairing Mode’ into connectable status.
2. Scan the HID MODE Barcode from this chapter.
3.Select Settings > General > Bluetooth(iOS)
4. Turn the iOS Bluetooth ON.
5. Select Bluetooth Settings and choose SR5600 from the list of discovered devices. The SR5600
displays as SR5600 - xxxx, where xxxx is the The last four digits of the Mac address.
2.2 HID Bluetooth Connection to Android
1. Scan the barcode ‘Pairing Mode’ into connectable status.
2. Scan the HID MODE barcode from this chapter.
3.Select Settings > Bluetooth(Android)
4. Turn the Android Bluetooth ON.
5 Select Bluetooth Settings and choose SR5600 from the list of discovered devices. The RS5100
displays as SR5600 - xxxxxx, where xxxxxx is the serial number.
Fast-connect:
*Make sure the Android’s NFC is on and Ring Scanner is power on, Tap NFC to pair and connect.
*Scan a QRCODE(Bluetooth MAC of urovo ’s U2 wearable devices) to quick pair and connect.



## PDF page 13

9
2.3 HID Bluetooth Connection to Windows
To start the connection process aim the SR5600 at about 7" (18 cm) away from the computer
screen and scan the barcode of the Pairing Mode.
The SR5600 Scan LEDs start flashing blue indicating that the SR5600 is attempting to establish
connection with the computer. The following notifications display upon successful connection.
1. Scan the barcode ‘Pairing Mode’ into connectable status.
2. Scan the HID MODE barcode from this chapter.
3.
4.



## PDF page 14

10
5.Default PIN code is 0000.



## PDF page 15

11
<Test in text file.>



## PDF page 16

12
2.4 Power Save
If no Bluetooth connection is made within 5 minutes, the ring scanner will auto switch off.
Disable power off
*Enable power off
2.5 Delay 01~10 ms to send (HID)
*1ms
2.6 Firmware Version



## PDF page 17

13
2.7 Restore Factory Setting
2.8. Indicators & Beeper setting
2.8.1. Power on alarming
OFF
*ON



## PDF page 18

14
2.8.2. LED indicator
OFF
*ON
2.8.3. Beeper setting
OFF
*ON



## PDF page 19

15
2.8.4. Duration
*50ms
2.8.5. Volume Level
Low
Middle
*High



## PDF page 20

16
3. Scanner Setting
3.1. Scanning Type
Continuous Barcode Read
Pluse
*Normal(Manual)
3.2. Illumination&Aiming setting
Disable both



## PDF page 21

17
Laser aiming only
Illumination only
*Enable both
3.3. Illumination level
Level 1
Level 2



## PDF page 22

18
*Level 3
Level 4
3.4. Suffix&Prefix
SR5600 can add 1 prefix and 2 suffix.
‘*’represent default.
Multi-step
Single-step
Function
Description
Parameter
Description
Option
%3001M
%
Disable
00
Enable
01*
Format
%3002M
%
<data><suffix
1><suffix 2>
00*



## PDF page 23

19
<data><suffix
1>
01
<data><suffix
2>
02
<prefix><data>
03
<prefix><data>
<suffix 1>
<suffix 2>
04
<prefix><data>
<suffix 1>
05
<prefix><data>
<suffix 2>
06
Prefix
%3003M
%
Prefix value
00~FF
...
00*
Suffix 1
%3004M
%
suffix 1 value
00~FF
...
0A*



## PDF page 24

20
0D
Suffix 2
%3005M
%
suffix 2 value
00~FF
...
0D*
0A



## PDF page 25

21
4. Symbologies
Code 39
To enable or disable Code39, scan the appropriate barcode below.
*Disable Code 39
1 Check digit
2 Check digit
*Do not Transmit Code39 Check Digit(Disable)



## PDF page 26

22
*Do not Transmit Code39 2 Check Digit(Disable)
Code 39 Full ASCII
*Disable Code 39 Full ASCII
Enable Code39 Full ASCII
PDF417
Disable PDF417



## PDF page 27

23
*Enable PDF417
Data Matrix
Disable Data Matrix
*Enable Data Matrix
Interleaved 2 of 5
*Disable ITF



## PDF page 28

24
Enable ITF
MaxiCode
*Disable MaxiCode
Enable MaxiCode



## PDF page 29

25
UPC/EAN
Disable UPC/EAN
*Disable UPC/EAN
Disable 2and5 digit supplemental
Enable 2 and 5 supplemental



## PDF page 30

26
Code 93
*Disable Code 93
Enable Code 93
Code 11
*Disable Code11
Enable Code11



## PDF page 31

27
Check digit and transmit
Disable Code11
*1 check digit
2 check digit
Do not transmit 1 check digit
Do not transmit 2 check digit



## PDF page 32

28
Matrix 2 of 5
*Disable Matrix 2 of 5
Enable Matrix 2 of 5
NEC 2of 5
*Disable NEC 2 of 5
Enable NEC 2 of 5



## PDF page 33

29
Hanxincode
*Disable Hanxin Code
Enable Hanxin Code
GridMatrix
*Disable GridMatrix
Enable GridMatrix



## PDF page 34

30
Aztec Code
*Disable Aztec Code
Enable Aztec Code
MicroPDF417
*Disable Micro PDF417
Enable Micro PDF417



## PDF page 35

31
MSI/PLESSEY
Disable MSI/PLESSEY(*)
Enable MSI/PLESSEY
Dotcode
Disable Dotcode(*)
Enable Dotcode



## PDF page 36

32
Standard 2 of 5
Disable Standard 2 of 5
Disable Standard 2 of 5
CodaBlock_F
*Disable CodaBlock_F
Enable
CodaBlock_F



## PDF page 37

33
CodaBlock_A
*Disable CodaBlock_A
Enable
CodaBlock_A
GS1 DataBar-14
*Disable GS1 DataBar-14



## PDF page 38

34
Enable GS1 DataBar-14
Codabar
*Disable Codabar
Enable Codabar
Code 2 of 5
*Disable code 2 of 5



## PDF page 39

35
Enable code 2 of 5
Trioptic
*Disable Trioptic
Enable Trioptic
postnet
*Disable postnet



## PDF page 40

36
Austranlian Post
Royal Mail(BPO-4-State)
Japan Post
Dutch Post(KIX code)
US Planet



## PDF page 41

37
US Postnet
US4State FICS(UPUID-Tag)
USPS 4CB(Intelligent Mail)
Canadian Post
Planet,Postnet



## PDF page 42

38
Planet,UPU
Postnet,UPU
Planet,USPS 4CB
Postnet,USPS 4CB
UPU,USPS 4CB



## PDF page 43

39
Planet,Postnet,UPU
Planet,Postnet,USPS 4CB
Planet,UPU,USPS 4CB
Postnet,UPU,UPS 4CB
Planet,Postnet,UPU,USPS 4CB



## PDF page 44

40
China Post
*Disable China Post
Enable China Post



## PDF page 45

41
OCR
Decoding
*Disable OCR
Normal
Inverse
Both



## PDF page 46

42
OCR Pattern
User Defined
*Passport
ISBN
Price Field



## PDF page 47

43
MicrE-13 B
OCR Fonts
OCR-A
OCR-B
*OCR-A or B



## PDF page 48

44
MICR
SEMI
OCR Character
Numeric
Alpha



## PDF page 49

45
Alphanumeric
*Any (include space)
OCR Character length : 00~FF
*18

Coverage check: 49/49 pages inspected.
