# KLD Operation manual

> Canonical original retained (bytes unchanged). This Markdown companion preserves the extractable text layer and transcribes every embedded screenshot in document order.
>
> - Original: `_shared/operations/kld-operation-manual_202608181911/KLD_Operation_20250707.docx`
> - Cover date: 2025.07.07
> - Core created: 2023-12-26; last modified 2025-07-07; revision 47; lastModifiedBy 康雄涛
> - Visual coverage: 35 embedded images inspected (image1–image35); 14 pages per DOCX app properties.
> - Source spelling is preserved (for example Manual-Inputed, selete, WARNMING, sure).

---

## Cover

|  |
| --- |
|  |
| KLD Operation manual |
|  |
|  |
|  |
| 2025.07.07 |

Administrator or operator authentication is required to access the KLD function, as shown below:

**Visual — image1.png (KLD Menu):** Android status bar time **8:45 PM**, with a stylized **P** icon, a square-in-square icon, signal, and a charging battery. Red header **KLD Menu**. Light-gray body with two stacked red rounded buttons: **Administrator Login** (upper) and **Operator Login** (lower).

---

## 1 Administrator Login

Start the KLD application, click the Administrator login button, and enter the administrator password as prompted (by default, the password of administrator A is all 1, and the password of administrator B is all 2, you must change the initial password at the first login).

**Visual — image2.png (Administrator Login):** Red header **Administrator Login**. Light-gray body. A single wide red **Login** button; no username/password fields on this screen.

**Visual — image3.png (Security Keyboard):** Black header **Security Keyboard**. Prompt **Please input Admin A password** above a blank white password field. Randomized numeric keypad:

- Row 1: **1**, **3**, **0**
- Row 2: **5**, **4**, **6**
- Row 3: **7**, **2**, **9**
- Row 4: **8** centered, empty cells on either side
- Right column: red **CANCEL**, yellow **DELETE**, tall green **OK**

Translucent footer watermark: **Device for development**.

**Visual — image4.png (Administrator Menu):** Red header **Administrator Menu**. Three top icons on a light gray-blue body:

1. **Key Import** — yellow circular arrow
2. **Management** — two interlocking blue gears
3. **Exit** — red hand pressing a button with a checkmark

Lower two-thirds of the screen is empty. Photograph of a physical display (glare/banding visible).

After the administrator passes the authentication, the administrator can access the Administrator menu.

### 1.1 Key Import

#### 1.1.1 Manual-Inputed BDK

The steps are as follows:

1. Enter into the "Import Key" page and click "Manual-Inputed BDK(TDES)".；

**Visual — image5.png (Import Menu, BDK TDES highlighted):** Red header **Import Menu**. Four yellow circular-arrow tiles:

- Top-left: **Manual-Inputted BDK Key(TDES)** — a red arrow points at this tile
- Top-middle: **Manual-Inputted BDK Key(AES)**
- Top-right: **Import Master Key(ciphered)**
- Bottom-left: **Manual-Inputted KEK Key**

Dark translucent footer: **Device for development**.

2. Enter the key component of BDK in plaintext (. After input component, check KCV in check popup; If KCV is correct, click the "Confirm" button to proceed to the next step.

**Visual — image6.png (BDK Key, component 1):** Red header **BDK Key**. Prompt **Please input Key component 1:**. Orange-bordered field containing `D5F4629EDF7C0E0ECDFE2607857F4AF1`. Character counter **(32)**. Red button **sure**.

**Visual — image7.png (KCV, component 1):** Red header **KCV**.

- **component 1 KCV(CMAC):** `2CB42D`
- **component 1 KCV(ECB):** `0BB04B`

Two red buttons: **sure** (left), **cancel** (right). Photograph of a physical display (reflections/smudges).

**Visual — image8.png (BDK Key, component 2):** Red header **BDK Key**. Prompt **Please input Key component 2:**. Orange-bordered field containing `088051439191BC2A762CCB898C97793B`. Character counter **(32)**. Red button **sure**.

**Visual — image9.png (KCV, component 2):** Red header **KCV**.

- **component 2 KCV(CMAC):** `CC0B6B`
- **component 2 KCV(ECB):** `0B9232`

Two red buttons: **sure** (left), **cancel** (right).

3. Input two BDK components in clear text and check KCV after xor; If KCV is correct, scroll down on the screen, click "sure" to save the BDK in the master pos.

(If the BDK only has one component, the 2nd component will be all zeros.)

The KSN Prefix is KSN,maximum length is 10 byte.

The randomDigits should be 0 or 2.

The key index of dukpt key should be 1-4.

**Visual — image10.png (combined KCV / import confirm):** Red header **KCV**. Fields:

| Field | Visible value |
| --- | --- |
| KSN Prefix | `22` |
| randomDigits | dropdown showing `0` |
| KeySetNum | `1` |
| key KCV(CMAC) | `FAD195` |
| KCV(ECB) | `586E92` |

Blue footer prompt: **Is or not import key?**

**Visual — image11.png (Import Key Finished):** Purple header **KLD**. Status-bar time **9:04 PM**. Background text and a centered dialog with a blue checkmark:

- **Import Key Finished**
- **Success: 1,**
- **Failed: 0.**

Dialog close **X** at top-right. Watermark **Device for development**.

#### 1.1.2 Import TMK

1. Enter into the ”Manual-Inputed KEK Key” option: the KEK key is used to decrypt the ciphertext master key.

Attention: Usually, KEK is obtained by XORing two components. If there are no component, KEK plaintext is directly input, and the second component is all zeros.

**Visual — image12.png (Import Menu, KEK highlighted):** Red header **Import Menu**. Same four tiles as image5. A thick red rectangle highlights **Manual-Inputed KEK Key**. Black footer **Device for development**.

**Visual — image13.png (KEK Component 2 + KCV popup):** Header **Component**. Status-bar time **10:29 AM**. Label **Component 2**, counter **(32)**, field filled with thirty-two `2` characters (`22222222222222222222222222222222`). Blue **Confirm** button. Overlay dialog:

- **KCV(Component 2):** `00962B`
- Buttons **Cancel** and **Confirm**

A numeric keypad is visible at the bottom (includes a Google **G** key).

**Visual — image14.png (KEK Component 1 + KCV popup):** Header **Component**. Status-bar time **10:29 AM**. Label **Component 1**, counter **(32)**, field filled with thirty-two `1` characters (`11111111111111111111111111111111`). Overlay dialog:

- **KCV(Component 1):** `82E136`
- Buttons **Cancel** and **Confirm**

2. Enter into the ”Import MasterKey” option: import the ciphertext master key into the master pos from the key file.

**Visual — image15.png (Import Menu, Import Master Key highlighted):** Orange/red header **Import Menu**. Same four tiles. A red box highlights **Import Master Key(ciphered)**. Photograph of a physical device; a small square QR sticker is on the top-left bezel (outside the UI).

**Visual — image16.png (Import TMK xls):** Red header **Import TMK xls**. White **File Path** placeholder field. Below it, a white control with red text **Please selete tmk file path**.

**Visual — image17.png (Pick a file):** Android file-picker, Recent directory. Status-bar time **11:13 AM**. Highlighted file (red rectangle):

| Name | Type / notes | Modified | Permissions | Size |
| --- | --- | --- | --- | --- |
| `tmk_cipher_28kld.xls` | Excel spreadsheet | 6/18/25, 11:27 AM | `-rw-rw----` | 18.0 kB |

Other visible entries: folder **storage** (6/18/25, 11:23 AM); **CALIBRI.ttf** 344.47 kB (4/29/25); **signed.crt** 1.14 kB (5/28/25); **test.csr** 1015.0 B (5/28/25); **uUACTIsCA.crt** 4.19 kB (11/20/23); **uUACTIsCA.key** 1.64 kB (11/20/23). Bottom-right **CANCEL**. Path/search bar shows a lock icon and **0**.

**Visual — image18.png (Import Key Finished after TMK file):** Photograph of a handheld. Purple header read as **KLD** (one inspection pass also produced **KED**; chrome matches the other KLD Import Key Finished dialog). Background log:

- `Initializing Key`
- `Importing:1/1`
- `Import Key Finished,`
- `Success: 1,`
- `Failed: 0.`

Foreground dialog: blue checkmark, **Import Key Finished**, **Success: 1, Failed: 0.**, close **X**. A QR sticker is on the top-left bezel.

3. Attention: the key file format need to be as below:
   SN, KEK index, master key index, ciphertext key, kcv, key algorithm.

Key algorithm: TDES/AES128/AES192/AES256.

**Visual — image19.png (example key file row):** Spreadsheet-like grid, columns A–F, only row 1 populated:

| A | B | C | D | E | F |
| --- | --- | --- | --- | --- | --- |
| `20240816151701` | `10` | `1` | `40BAEF32B505F86F40BAEF32B505F86F` | `00962B` | `TDES` |

This matches the stated column order: SN, KEK index, master key index, ciphertext key, kcv, key algorithm.

### 1.2 Management

Management is the KLD management menu, Member Management, Record Management, and Delete Key. After the administrator login for the first time, you need to add two operators to perform key related operations.Member Management

**Visual — image20.png (Manage Menu):** Red header **Manage Menu**. Three tiles:

1. **Member Management** — two interlocking blue gears
2. **Record Management** — blue clipboard with a magnifying glass
3. **Delete Key** — three overlapping orange rectangular cards

Watermark **Device for development**.

#### 1.2.1 Member managment

**Add Operator**

Add Operator Detailed steps, Enter accounts, pure numbers are recommended，Enter the password and confirm it

**Visual — image21.png (Member Management):** Red header **Member Management**. Three list rows with right chevrons:

1. **Add Operator**
2. **Delete Operator**
3. **Modify Operator Password**

Watermark **Device for development**.

**Visual — image22.png (Add Operator accounts):** Red header **Add Operator accounts**. Three fields:

- **accounts :** placeholder **Please input accounts**
- **new password :** placeholder **Please input new password**
- **new password :** placeholder **Please input new password** (second field is the confirmation field)

Red button **sure**. Bottom-right watermark in Chinese: **开发样机禁止商用**.

**Delete Operator**

Confirm the deletion by entering accounts and password.

**Visual — image23.png (Delete Operator accounts):** Red header **Delete Operator accounts**. Fields:

- **accounts :** placeholder **Please input accounts**
- **password :** placeholder **Please input the password!**

Red button **sure**. Watermark **Device for development**.

**Modify Operator**

Enter accounts, old password, new password, confirm the change

**Visual — image24.png (Update Operator password):** Red header **Update Operator password**. Four fields:

- **accounts:** placeholder **Please input accounts**
- **original password :** placeholder **Please input original password**
- **new password :** placeholder **Please input new password**
- **new password :** placeholder **Please input new password ang...** (text is cut off on the screenshot; likely “again”)

Red button **sure**. Watermark **Device for development**.

---

## 2 Operator Login

**Visual — image25.png (Operator A login):** Red header **Operator A login**. Fields:

- **accounts** placeholder **Please input your accounts**
- **password** placeholder **Please input your password**

Red **Login** button. Watermark **Device for development**.

**Visual — image26.png (Operator B login):** Same layout as image25; header is **Operator B login**.

1. Click the Operator Login button, and enter the account and password of Operator A and B according to the prompts (the initial password must be changed for the first login).

After the operator passes the authentication, the operator can access the KLD menu, which includes KMS Download CA, Load key, Query keys and Exit.

### 2.1 KMS Download CA

Go to the following page and click Download CA Cert. The remote CA certificate will be imported. The message "Download certificate successfully" is displayed. In this process, you need to bind the KLD SN in the background. If the SN is not bound, contact UROVO team.

**Visual — image27.png (Download CA Cert idle):** Status-bar time **1:29 PM**. Purple header **KLD** with a settings gear on the right. Empty white body. Wide purple button **Download CA Cert**. Footer:

- **SN:20241119152801**
- **version: 0.6.20241119104121**

Watermark **Device for development**.

**Visual — image28.png (Certificate Downloading):** Purple header **KLD** + gear. Background text **Certificate Downloading...**. Centered white dialog with three red loading dots and bold purple **Certificate Downloading...**. Purple button **Download CA Cert**. Footer:

- **SN: 20241119152801**
- **version: 2.0.2...** (remainder cut off at the bottom of this screenshot)

Status-bar time **1:33 PM**. Watermark **Device for development**.

**Visual — image29.png (Certificate Downloaded Successfully):** Status-bar time **10:44 PM**. Purple header **KLD** + gear. Background log:

- Certificate Downloading...
- Certificate Downloaded Successfully!

Centered dialog: blue checkmark, **Certificate Downloaded Successfully!**, close **X**. Purple button **Download CA Cert**. Footer **SN: 20241119152801**; version string is partly obscured by the **Device for development** watermark.

### 2.2 Load Key

1. The key cable connects the KLD to the Sub-POS；

**Visual — image30.png (key-cable connection photo):** Two black handhelds on a light-gray surface, linked by a black cable that includes a rectangular inline adapter/module. Red arrows mark the plug points: bottom-center port on the left device, right-side port on the right device. Both devices have white stickers reading **海外技术部**.

- Left (smaller) device: screen on, red header **Operator Menu**, at least an **Exit** tile (red hand icon) visible; Android nav (recent / home / back); green LED at top-left.
- Right (larger, thicker) device: contactless-payment symbol at the top; screen dark; same three nav icons.

2. In the case of operator role login, click the KLD menu item "Load Key"( If prompted”The CA Certificate is not exist, please download first”).

**Visual — image31.png (Operator Menu, Load Key highlighted):** Red header **Operator Menu**. Four tiles:

- **KMS Download CA** — teal circular-arrow icon
- **Load Key** — teal box-with-inbound-arrow icon; a small red diagonal arrow points at this tile
- **Query Keys** — orange-red magnifying glass
- **Exit** — orange-red hand-pressing-button icon (second row, far left)

Watermark **Device for development**.

Attention: you must first click on the 'Load Key' of the master pos,

and then click on the 'Sync Key' of the sub pos.

3. If prompted”The CA Certificate is not exist, please download first”，Download CA Cert”， The default factory download certificate。

**Visual — image32.jpeg (Sub-POS Key Management System, missing CA):** App title **Key Management System** with a settings gear. Status-bar time **2:24 PM**. Background purple buttons **Query Key** and **Sync Key**. Foreground **Exception** dialog: cartoon crashing rocket, green text **The CA Certificate is not exist, please download first**, orange/red **Confirm**. Footer:

- **SN:** `98282135009171`
- **Version:** `55.20240719`

**Visual — image33.png (Sub-POS Key Management System, Download CA Cert):** Photograph of a physical screen. Title **Key Management System** + gear. Prompt **Please input the key's index.** above a thin green underline (input field). Two wide purple buttons; a red arrow points to the upper one:

- **Download CA Cert**
- **Sync Key**

Footer:

- **SN:** `80062347000011`
- **version:** `65.20241025`

Status-bar time **6:04**.

4. Key download result:

**Visual — image34.png (two devices after key download):** Photograph of two rugged handhelds connected by a black USB/key cable.

Left (smaller) device: sticker **海外技术部**. Success dialog **Key Downloaded Successfully!** with a blue checkmark. Background log fragments include **Master Po...**, **Update Key Status**, **Key Exchange**, **Key Verify**.

Right (larger) device: handwritten sticker **80**. Success dialog **Key Downloaded Finish!** with a blue checkmark. Background log shows multiple `KeyIndex` entries, including **17**, **18**, **22**, **23**, **94**, with messages **TMK Key Writing Successfully!**, **Update TMK Key Status OK**, and **Key Exchange, KCV:** values including `1EDA36`, `578AA9`, `C55502`, `002D47`. Partial watermark **Device for deve...**.

Visible in the photograph on a paper above the devices (not KLD UI chrome; one line is not fully legible):

- **2100:** SQ29, SQ29G
- **SQ29UR:** *(remaining text unreadable on this photo)*
- **PB100:** SQ81 高速
- **PB100P:** SQ83 高速
- **PB100P 4G:** SQ83A 高速

These handwritten notes are background objects in the photo, not on-screen KLD labels.

---

## 3 Warning

If you enter the wrong administrator password five times, the device will be locked. In the following figure, use the activation card to activate the device, and the administrator password of the KLD will be restored to the initial password

**Visual — image35.png (device locked / activation):** Status-bar time **10:40 PM**; **P** icon, Urovo-style **U** icon, download-arrow-in-triangle, charging battery. Yellow header **Turn on cellular data**. Body:

- **WARNMING! (0x73000003)** (source spelling)
- **This device has been locked。 Please active this device!!!**
- **Emergency calls only:** toggle **OFF**
- **Wi-Fi connected:** toggle **ON**
- **version:(1.37.24.0203)**

Bottom-left **Safe mode**. Bottom-right button **ACTIVE >**.

---

## Visual coverage check

| Item | Count | Status |
| --- | --- | --- |
| Embedded images in the DOCX | 35 (image1–image35, including image32.jpeg) | All inspected and transcribed above in document order |
| DOCX app-property page count | 14 | Text layer + screenshots cover the documented sections; no uninspected image remains |
| Unreadable / ambiguous | image18 header (KLD vs KED); image24 last placeholder cut off; image28/29 version strings truncated/obscured; image34 SQ29UR handwritten remainder | Marked in place |
