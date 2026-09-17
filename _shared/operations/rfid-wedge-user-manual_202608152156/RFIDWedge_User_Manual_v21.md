# RFIDWedge User Manual

> Source original retained (bytes unchanged). This Markdown companion preserves the extractable text layer of the source.

---

RFIDWedge User Manual
Version V21
Shenzhen Urovo Technology Co. , Ltd.
November 14,2023

Statement
This document is owned and interpreted by Shenzhen UROVO Technology Holdings Limited and
shall not be copied, disclosed or sold to third parties without the written permission of Shenzhen
UROVO Technology Holdings Limited.
This document is the functional operation instructions of RFIDWedge. The specific operation is
subject to the functions of the user's handheld device. Read the instruction manual in detail before use,
and make operation in accordance with standards.
Revision History

| Version  | Date  | AMD  | Revised by  | Description  |     |
| -------- | ----- | ---- | ----------- | ------------ | --- |
March 18,
| V1.0  |     | A   | Gong Yi  | First edition  |     |
| ----- | --- | --- | -------- | -------------- | --- |
2021
|       | August     |     |              | Output mode adds keyboard type  |     |
| ----- | ---------- | --- | ------------ | ------------------------------- | --- |
| V1.1  |            | A   | Qiu Yanfang  |                                 |     |
|       | 10,2021    |     |              | and operation key characters    |     |
|       | September  |     |              | Description of key setting is   |     |
| V1.2  |            | A   | Qiu Yanfang  |                                 |     |
|       | 08,2021    |     |              | added.                          |     |
1.Delete the setting of Key Setting
April 20,
| V1.3  |     | D   | Qiu Yanfang  | 2. Modify the Key Setting to  |     |
| ----- | --- | --- | ------------ | ----------------------------- | --- |
2022
RFID Normally On
|       | June 23,  |     |              | Modify the RFIDWedge global  |     |
| ----- | --------- | --- | ------------ | ---------------------------- | --- |
| V1.4  |           | M   | Qiu Yanfang  |                              |     |
|       | 2022      |     |              | switch position.             |     |
1.Added the export and import
function.
|      | August 28,  |     |              | 2.Set parameters by sending a  |     |
| ---- | ----------- | --- | ------------ | ------------------------------ | --- |
| V20  |             | A   | Qiu Yanfang  |                                |     |
|      | 2023        |     |              | broadcast.                     |     |
3.Data source Added output
format.
1.Add the range function;
2.Added ASCLL output;
3.Added "Unified Output" in
|      | November  |      |              | keyboard mode.                   |     |
| ---- | --------- | ---- | ------------ | -------------------------------- | --- |
| V21  |           | A,M  | Qiu Yanfang  |                                  |     |
|      | 14, 2023  |      |              | 4.In keyboard mode, the default  |     |
"input method output";
5.The SQ53S is compatible with
V1.3 RFID handles

(A-Add, M-Modify, D-Delete)
|     |     |     |     |     |     |
| --- | --- | --- | --- | --- | --- |

Contents
Contents ............................................................................................................................................ 1
I. Home Page .................................................................................................................................... 1
II. Global Settings ............................................................................................................................. 3
2.1 New..................................................................................................................................... 4
2.2 Import ................................................................................................................................. 4
2.3 Export ................................................................................................................................. 5
2.2 About .................................................................................................................................. 5
III. Detailed Settings ......................................................................................................................... 6
3.1 Related Apps....................................................................................................................... 6
3.2 Beep .................................................................................................................................... 7
3.3 Scan Mode .......................................................................................................................... 7
3.4 Key Setting ......................................................................................................................... 8
3.5 Data Sources ..................................................................................................................... 10
3.6 Output Mode ..................................................................................................................... 10
3.7 Filter ................................................................................................................................. 13
3.8 Tag Format ....................................................................................................................... 14
3.9 Trigger Mode .................................................................................................................... 15

I. Home Page
Tap RFIDWedge to enter the main interface.The RFIDWedge global switch button needs to be
turned on first. The app will have a Default Config.; then enter the Default Config, bind the app and set
the key value to use the RFIDWedge function.
The program supports broadcast debugging Settings.
e.g.: 1.Open RFIDWedge gglobal switch button;
2. Tap to enter the Default Config, and then enter the associated app to bind the SMS Application.
第 1 页

3.Return to the previous interface and enter the Key Setting; then press the entity button to be
scanned on the Key Setting interface. The interface will display the set key value and key value name.
3. After setting, enter the SMS Application to select Text Input, and use the scan key set in the
Key Setting function for scanning; then the RFID content can be automatically input to the text box.
第 2 页

Note:
1. It is the keyboard input mode by default, the broadcast mode modification method, see 3.5 for
details.
2. Detachable handle devices and handle-less devices need to set up RFID Scan Button first, see
3.4 for details.
II. Global Settings
Click the RFIDWedge program to enter the home page, the Wedge switch must be turned on
first,otherwise the RFIDWedge function cannot be used.
第 3 页

2.1 New
1. Tap New to create a new configuration, different configurations can be associated for different
apps.
2. Long press a particular configuration to rename and delete the configuration.
2.2 Import
2.2.1 Manual import
Place the configuration file in any local directory, click the Import button, and manually select the
target configuration file to import the configuration file.
2.2.2 Automatic import on startup
第 4 页

The configuration file into the/sdcard/RfidWedge/file/autoImport/folder, restart the equipment can
import the configuration file. (/ sdcard/RfidWedge/file/autoImport/folder first open RfidWedge
automatically generated after the procedure.)
Note: The program has fixed identification of the file name rfidwedge_config.txt, do not modify at
will, otherwise the import will fail.
2.3 Export
Click the Export button and the configuration file rfidwedge_config.txt will be generated under
local /sdcard/.
2.2 About
Check the current software version.
第 5 页

III. Detailed Settings
1. Tap a particular configuration to enter the detailed settings of the configuration, each configuration is
independent.
2. The upper right corner is the main configuration switch, which is turned on by default, and the rule
will not take effect after it is turned off.
3.1 Related Apps
1. Default rules and new rules, there is no related apps by default.
第 6 页

2. Tap the Related Apps that needs to be selected in More Apps to bind, and one rule can bind multiple
apps.
3. Swipe right on the Related Apps tab and click Delete to delete the related apps.
3.2 Beep
The beep is Sharp by default, and can be modified to None or Short.
3.3 Scan Mode
1. The default scan mode is Repeat
Deduplicate: read as many unique tags as possible
The data of the selected application is the only one that is not duplicated
第 7 页

Repeat: read as many tags as possible
Return all the stored data
Single: manual scan, only scan one tag for one trigger
Only return a piece of currently scanned data
3.4 Key Setting
1. After setting, enter the SMS Application to select Text Input, and use the scan key set in the Key
Setting function for scanning; then the RFID content can be automatically input to the text box.
第 8 页

2. The mapping function has 2 modes: RFID, RFID + Scan
RFID: RFID is enabled by default. After setting the key value, you can directly enter the
associated app to use RFID for scanning.
RFID + Scan: By enabling Scan and entering the associated app, you can simultaneously use
RFID and scanning head for scanning.
3. If the Float Button is turned on, a float button will show up on pages of related apps, and you may
switch between the modes of Scan and RFID easily. The Float Button also offers threes modes of
mapping functions same as above, including RFID, Scan and Both.
Functions Modes of Float Button
第 9 页

3.5 Data Sources
1. The EPC area is read by default, the Session is S0, and the output format is HEX.
2. You can click the following Settings to modify the read area, Session, and read format.
3.6 Output Mode
1. The default output mode is input method only. You can set Keyboard Type, Uniform Output, and
Operation Key Characters as required.
 Footed keyboard type
The default keyboard type is Input Method Only.
The output methods of the two keyboard types are different.
第 10 页

After scanning with "Input method only", all barcode data is displayed in the input box
immediately.
After the bar code is scanned by the physical keyboard, the bar code data is displayed
one by one.
 Whether to unify output
Yes: Data is displayed in the input box only after scanning stops.
No: The scan data is displayed in the input box immediately.
 Anyway operates a key character
None: no key is set. Operation key The default value is None. No operation is
performed after the scan.
Carriage return: After scanning the bar code, enter operation is attached.
Line feed: Line feed. After the barcode is scanned, a newline operation is provided.
Tab: tabs. After scanning the bar code, there is a lattice operation.
第 11 页

2. Turn off the Output Mode namely broadcast output. The intent action and tag data are as shown in
the figure below, which can be modified according to requirements.
第 12 页

3.7 Filter
1.It is Unfilter by default.
2.Filtering settings include 4 types: Partial Filtering, Fully Filtering, Partial Screening, Fully Screening
 Partial Filtering: If the input data information and tag information are partially continuously
overlapped, then filter out accordingly (for example: input 123, filter tag 123455, 645674123;
retain: 14552443)
 Fully Filtering: If the data information and tag information are identical, filter out (for example:
input 123456, filter: tag 123456, retain: 123456789, 33123456, 1233456)
 Partial Screening: If the data information and tag information are partially continuously
overlapped, weed out and display these tags
 Fully Screening: If the data information and tag information are identical, weed out and display
these tags
第 13 页

3.8 Tag Format
1. The suffix is checked in the default format type, and the suffix is special characters [LF] by default.
2. You can choose more than one format type according to your needs.
3. Check the Prefix, Suffix or Replacement, enter the required characters in the settings below, or select
special characters.
第 14 页

3.9 Trigger Mode
1. The default trigger mode is Tap;
2. Press/Tap can be modified:
 Press: scan while pressing the trigger or triggering the button. Release the button to stop
scanning
 Tap: tap the Trigger Button to start scanning, tap again to end scanning
第 15 页

|     | 第  16 页  |     |
| --- | -------- | --- |
