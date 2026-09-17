# RFID-Demo User Manual

> Source original retained (bytes unchanged). This Markdown companion preserves the extractable text layer of the source.

---

RFID-Demo User Manual
Version V25
UROVO TECHNOLOGY CO., LTD.
November 1, 2023

Statement
This document is owned and interpreted by UROVO TECHNOLOGY CO., LTD. and shall not
be copied, disclosed or sold to third parties without the written permission of UROVO
TECHNOLOGY CO., LTD.
This document is the functional operation instructions of RFID-Demo. The specific operation is
subject to the functions of the user's handheld device. Read the instruction manual in detail before use,
and make operation in accordance with standards.

| Version            | Date  | AMD  | Revised by  | Description  |     |
| ------------------ | ----- | ---- | ----------- | ------------ | --- |
| V1.0  January 29,  |       | A    | Gong Yi     |              |     |
2021
| V1.1  April 13,  |     | M   | Gong Yi  | 1.pop-up window that indicates   |     |
| ---------------- | --- | --- | -------- | -------------------------------- | --- |
| 2021             |     |     |          | unsuccessful RFID connection is  |     |
added.
2.Options of long- and
short-distance module are added.
V1.2  September  A  Qiu Yangfang  1.A handle indicator initialization
| 15, 2021  |     |     |     | button is added for products with a  |     |
| --------- | --- | --- | --- | ------------------------------------ | --- |
removable handle.
V1.3  June  M  Qiu Yangfang  Read and write label modification,
| 15,2022  |     |     |     | before can read multiple, after  |     |
| -------- | --- | --- | --- | -------------------------------- | --- |
modification, can only read one by
one.
V22  June 1,2023  M,D  Qiu Yangfang  1.Remove the mode selection;
2. Remove the settings interface
(connecting serial port, antenna
sensitivity, quick reading of TID
tags, reader status reader
identification, reader RS-485
address);
3. Add the function of setting
custom parameters in the settings
interface;
4.Two new query methods have
been added to the scanning
interface;
5.Inventory data can be returned to
|     |     |     |     |     |     |
| --- | --- | --- | --- | --- | --- |

TID;
6.Modify the data selection
methods for read/write, lock, and
destroy interfaces;
7.Added InventoryLed function;
V24 November A,M Qiu Yangfang 1.Change the scanning interface to
1,2023 manual clearing;
2.Added the function of rfid range
Settings;
3.Added EPC area ascll code
scanning, read/write;
4.The SQ53S model is compatible
with the 1.3SQ53R handle
(A-Add, M-Modify, D-Delete)

contents
contents .............................................................................................................................................. I
I. Scan .............................................................................................................................................. II
II. Tag Management ....................................................................................................................... III
2.1 Read/Write ........................................................................................................................ IV
2.2 Lock .................................................................................................................................. IV
2.3 Kill ..................................................................................................................................... V
III. Filter ......................................................................................................................................... VI
IV. Location ...................................................................................................................................VII
V. Settings ................................................................................................................................... VIII
VI. InventoryLed ...........................................................................................................................XII
I

I. Scan
Visit the main page of the App by clicking the RFID icon, and you will be required to choose a
UHF RFID module for your first visit. Choose the module appropriate to your product type as
instructed and then click the START SCANNING button to start RFID label scanning with default
settings.
The meaning of the data displayed is as follows:
V0.00-？ Module firmware version number (?=7, 5, 3, R, C, M correspond to
E710/E510/E310/R2000/C6/M100 respectively).
Unique Tags (Pcs) The count of unique tags that have been scanned in total since tapping
the Start Scanning button.
Read Rate (Pcs/sec) The rate of tag read.
Total Reads One tag EPC is recorded as one piece of tag data. Here shows the
counted total numbers of data in real time, including the data of the same
tag read repeatedly.
Read Time The total read duration since tapping the Start Scanning button.
ASCLL Convert the data in the EPC area to the corresponding Ascll code
characters.
II

The fields in the tag list have the following meanings:
DATA(??) The specific data scanned in the area (?? depending on the scan area
selected, the corresponding area is displayed)
COUNT Number of times of tag being recognized
RSSI Signal intensity at the last time of tag being recognized
Note: A pop-up window as shown below will appear when you open the App if there is no RFID
module or the RFID module is failed to be connected.
II. Tag Management
The tag management page can be accessed through the Tag Management / Sidebar at the bottom
of the home page. The main functions of the module are to read, write, lock and kill tags.
II

2.1 Read/Write
Before reading labels, scan and take inventory on the label scanning interface. After the inventory
is complete, click Label Management and select the labels to be read and written to write labels or
labels.
To read a tag, three parameters need to be entered: the tag area to be read, the starting address
and the data length.
Note that the input parameters should be in accordance with the tag specifications. Otherwise,
an error message will be prompted.
The interface for writing tag is in the same area as the reading, except that the writing
requires the access password and the data to be written.
(The default access password is 00000000)
Note: The maximum writing length at one time is 32 words (64 bytes, 512bits).
2.2 Lock
The operation interface for locking tags is as follows:
An access password must be provided to lock the tag.
1. Select the storage area that needs to be locked;
2. Fill in the access password for the label;
3. Select the locking method;
4. Select the label that needs to be locked;
Note: The original password is not valid for locking. It is recommended that the user change the
access password before locking the tag.
IV

After successful operation, the following information will be returned.
2.3 Kill
The operation interface for destroying tags is as follows:
To destroy a tag, the kill password must be provided, and the kill password cannot be 00 00 00 00. So
to destroy a tag, you must first modify the content of the kill password in the password area by the
command to write tag.
V

III. Filter
Tap sidebar Filter to enter the filter settings page, and main functions of the module is to filter and
weed out the content of the tag scanning.
Filtering settings include 4 types: Partial Filter, Fully Filter, Partial Weed out, Fully Weed out
1. Partial Filter: If the input data information and tag information are partially continuously overlapped,
then filter out accordingly (for example: input 123, filter tag 123455, 645674123; retain: 14552443)
2. Fully Filter: If the data information and tag information are identical, filter out (for example: input
123456, filter: tag 123456, retain: 123456789, 33123456, 1233456)
3. Partial Weed out: If the data information and tag information are partially continuously overlapped,
weed out and display these tags
4. Fully Weed out: If the data information and tag information are identical, weed out and display these
tags
Note: The starting address can be set for Fully Filter and Fully Weed out
V

IV. Location
The main purpose of this function is to display the relative positional relationship between the
RFID Reader and the tag.
First scan the tags, then select a particular tag.
Switch to the Location page (the tag just selected will be displayed above) and click the start button.
After starting, the page will display the Signal Intensity in real time. The larger value means the
stronger signal and closer to the tag
V

V. Settings
Tap sidebar Setting to enter the setting page, mainly for the configuration of the RFID
Reader.
Options of UHF RFID Module: Automatically select corresponding modules based on device type.
V

Connect Serial Number: It can be used by default and does not need to be modified
Export: The current tag scanning data can be exported to Excel
IX

Basic Parameter Settings:
1. Firmware Version: Display the current firmware version
2. Sounds Settings: Set whether to beep during scanning, which is enabled by default
3. RF Output Power: The default is as follows, which can be read and set
4. RF Spectrum: The default is as follows, which can be read and set
X

Note: When setting the frequency band, it is necessary to determine whether the antenna is a European
standard antenna or an American standard antenna. Setting it incorrectly may result in the tag not being
read.
5. Handle indicator: for products with a removalble handle, the second indicator on the right side of the
removalble handle will flash when you scan if it is turned on. To turn it off, click it again.
6.Profile
In the profiles supported by the E-series:
Mode 13: 160k, M8, 20us (farther distance when reading a single card)
Mode 15: 640k, M4, 7.5us (better group reading effect)
7. Tag Focus (only supports E-series)
This function only supports the use of E-series module devices;
Read more tags in a shorter time, such as 400 tags. At the same reading time, if not opened, 200 tags
may be read, but if opened, 400 tags can be read.
X

8. Custom parameter settings: Customize parameter configurations according to requirements.
The following modes have been added to the Session
Auto1: S2/S3 alternating operation
Auto2: Extreme Inventory Mode
Auto3: Fast limit inventory mode
Range：Reading distance control (short range reading control, power set between 10-15dBm, read
distance is controlled by adjusting the range, the smaller the range value, the closer the reading
distance)
VI. InventoryLed
This feature supports the manufacturer labels of Kailuwei and Yilian. Select the label that needs to
be inventoried, and the inventoried label will follow the flashing light of the disk.
To select the manufacturer who needs to read the label, first inventory the label, select and check
the checkbox to the right of the label that needs to be read, and click Inventory;
X II

The inventory label indicator light will follow the disk reading and light up.
X II
