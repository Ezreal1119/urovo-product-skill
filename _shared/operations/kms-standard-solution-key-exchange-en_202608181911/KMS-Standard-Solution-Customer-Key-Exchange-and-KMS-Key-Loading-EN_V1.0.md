# KMS Standard Solution — Customer Key Exchange and KMS Key Loading Instructions

> Canonical original retained (bytes unchanged). This Markdown companion preserves the extractable text, tables, lists, and the one embedded cover image.
>
> - Original: `_shared/operations/kms-standard-solution-key-exchange-en_202608181911/KMS-Standard-Solution-Customer-Key-Exchange-and-KMS-Key-Loading-EN_V1.0.docx`
> - Title (core properties): KMS Standard Solution - Customer Key Exchange and KMS Key Loading Instructions
> - Subject: English translation, Version 1.0
> - Keywords: KMS, MK/SK, DUKPT, KEK, TMK, BDK, ZMK, TR-31, KSN
> - Author: Zhang Weixiang
> - Core created / modified: 2026-07-13
> - Visual coverage: 1 embedded image (cover logo) inspected; 13 pages per DOCX app properties.

---

## Cover

**Embedded image (image1.png, 423×116):** UROVO® horizontal logo. Cyan/light-blue wordmark **UROVO** with ® above the V, followed by Chinese **优博讯** (the first character 优 has a small light-green accent stroke). A thin cyan horizontal rule separates the wordmark from the tagline **领跑行业移动应用**. White background.

Cover table (single column):

|  |
| --- |
| *(UROVO logo, transcribed above)* |
| KMS Standard Solution |
| Customer Key Exchange and KMS Key Loading Instructions |
| V1.0 |
| **Zhang Weixiang** |
| **2026.7.13** |

---

## Revision Statement

**Department Responsible for Preparation and Interpretation:**

Related Standards or Documents in This Series:

Consistency with Relevant International Standards or Documents:

Other Standards or Documents Superseded or Withdrawn:

Relationship with Related Standards or Documents:

| Version | Author | Date | Change Description |
| --- | --- | --- | --- |
| V1.0 | Zhang Weixiang | 2026.7.13 | Initial release |
|  |  |  |  |
|  |  |  |  |
|  |  |  |  |
|  |  |  |  |
|  |  |  |  |
|  |  |  |  |
|  |  |  |  |
|  |  |  |  |
|  |  |  |  |
|  |  |  |  |
|  |  |  |  |
|  |  |  |  |

The revision table contains twelve blank reserved rows after the V1.0 entry.

---

## 1. Purpose

This document is established to standardize the key exchange, receipt, verification, and loading processes between our company and the customer, and to ensure the confidentiality, integrity, and traceability of keys during transmission, import, and use.

Our Key Management System (KMS) currently supports the following two key hierarchies:

1. MK/SK key hierarchy;
2. DUKPT key hierarchy.

Because the two key hierarchies use different root keys, transmission methods, and loading processes, they are described separately in this document.

## 2. Basic Principles

Customer key exchange and KMS key loading shall follow the principles below:

1. **Separation of Key Components**
   - When keys are exchanged in the form of key components, different components shall be generated, held, and transferred separately by different key custodians. No single person shall have access to the complete key.

2. **Dual Control**
   - The receipt, entry, combination, and verification of key components shall, in principle, be jointly performed by at least two authorized persons under mutual supervision.

3. **Separation of Transmission Channels**
   - Key components, encrypted key files, key check values, and related passwords shall be transmitted through mutually independent channels to prevent disclosure of the complete key if a single transmission channel is compromised.

4. **Complete Audit Trail**
   - Necessary approval, handover, and operation records shall be retained for the receipt, verification, entry, import, and activation of keys to support subsequent audits and traceability.

5. **Need-to-Know Principle**
   - Only authorized key management personnel are permitted to access key components, encrypted key files, and related sensitive information.

## 3. MK/SK Key Hierarchy Exchange and Loading Process

### 3.1 Key Hierarchy Description

The MK/SK key hierarchy generally consists of master keys and working keys.

Specifically:

- MK is the master key used to protect or derive other keys;
- SK is the working key used for specific business scenarios;
- Under our current KMS onboarding process, the customer first provides KEK key components;
- After the KEK is combined in the KMS, it is used to protect the TMK subsequently provided by the customer;
- The customer then provides a TR-31-formatted TMK ciphertext file.

### 3.2 Step 1: Receive KEK Key Components

The customer splits the KEK into multiple key components, which are packaged separately by different key custodians.

KEK key components shall be delivered to our company in physical packages with tamper-evident seals and unique serial numbers. In principle, different key components shall be packaged separately and may be transferred in separate packages, under separate seals, or through separate handovers, as agreed by both parties.

The physical package may contain the following:

- KEK key component;
- Key component number;
- Key usage description;
- Key algorithm and length;
- Key version information;
- Key check value or component check information;
- Key handover form;
- Other information agreed by both parties.

Upon receipt of the physical package, our company shall verify the following:

1. Whether the package and seal are intact;
2. Whether the package number matches the handover record;
3. Whether the number of key components is as agreed;
4. Whether the key algorithm, length, version, and usage are clearly specified;
5. Whether there is any package damage, seal anomaly, or inconsistency in the information.

If any anomaly is found, our company shall suspend subsequent key loading operations and promptly confirm the issue with the customer.

### 3.3 Step 2: Enter and Combine the KEK

Authorized key custodians of our company shall separately enter the received KEK components into the KMS in a controlled environment.

The entry process shall follow the dual-control principle. Different key components shall be entered separately by the corresponding authorized personnel, and the system shall combine the components to form the complete KEK.

After the KEK has been combined, its key check value shall be verified.

If the KEK check value calculated by the KMS matches the value provided by the customer, the process may continue. If the values do not match, the operation shall be stopped immediately and the following items shall be checked:

- Whether any key component was entered incorrectly;
- Whether the order of the key components is correct;
- Whether the key algorithm and key length are consistent;
- Whether the key components belong to the same KEK set;
- Whether the check value provided by the customer is correct.

Until the issue has been confirmed, the KEK shall not be used to import any other business key.

### 3.4 Step 3: Receive the TR-31-Formatted TMK Ciphertext File

After the KEK has been successfully loaded into our KMS and verified, the customer shall provide a TMK ciphertext file protected by that KEK.

The TMK ciphertext file shall be encapsulated in the TR-31 key block format.

The TR-31 key block provided by the customer shall specify, or allow identification of, the following information:

- Key usage;
- Key algorithm;
- Key length;
- Key mode of use;
- Key version;
- Key exportability;
- Key block integrity-protection information;
- Other TR-31 key block header attributes.

The TMK ciphertext file may be transmitted through a secure electronic channel agreed by both parties, but it shall not be transmitted through the same channel as the complete plaintext KEK or all KEK components.

### 3.5 Step 4: Import the TMK

After receiving the TR-31-formatted TMK ciphertext file, authorized personnel of our company shall import it into the KMS.

The KMS shall use the loaded KEK to unwrap the TR-31 key block, verify its integrity, and check the following:

1. Whether the TR-31 key block format is valid;
2. Whether the key block has been altered;
3. Whether the key usage is as agreed;
4. Whether the key algorithm and length meet the system requirements;
5. Whether the key usage attributes are appropriate for the actual business scenario;
6. Whether the TMK check value matches the information provided by the customer.

The TMK may be activated in the KMS only after all verifications have passed.

### 3.6 MK/SK Key Hierarchy Process Overview

The overall MK/SK key hierarchy process is as follows:

The customer generates and splits the KEK
-> The customer transfers the KEK components in physical packages
-> Our company separately enters and combines the KEK components in the KMS
-> Both parties verify the KEK check value
-> The customer uses the KEK to encapsulate the TMK
-> The customer transfers the TR-31-formatted TMK ciphertext file
-> Our KMS imports and verifies the TMK
-> The TMK is activated and used for subsequent business key management.

## 4. DUKPT Key Hierarchy Exchange and Loading Process

### 4.1 Key Hierarchy Description

The DUKPT key hierarchy uses the BDK as the base derivation key and combines it with the terminal's initial Key Serial Number (KSN) and other information to derive the terminal's initial key and subsequent transaction keys.

Our company currently supports the following two methods for BDK exchange:

1. Direct receipt of BDK key components;
2. Receipt of ZMK key components first, followed by a TR-31-formatted BDK ciphertext protected by the ZMK.

The customer may select either method according to its own key management framework and security requirements.

## 5. DUKPT Method 1: Direct Receipt of BDK Key Components

### 5.1 BDK Component Generation

The customer splits the BDK into multiple key components, which are generated and held separately by different key custodians.

No individual key component shall be equivalent to the complete BDK, and no single person shall hold all BDK components at the same time.

### 5.2 BDK Component Transfer

BDK components shall be transferred to our company in physical packages with tamper-evident seals and unique serial numbers.

In principle, different BDK components shall be transferred in separate packages or through separate handovers and shall be accompanied by the necessary information, including:

- BDK component number;
- DUKPT key usage;
- Key name, algorithm, and length;
- BDK check value;
- Corresponding customer or project identifier;

Upon receipt, our company shall check the integrity of the package, seal status, number of components, and consistency of the related information.

### 5.3 BDK Entry and Combination

Authorized personnel of our company shall separately enter the BDK components into the KMS in a controlled environment, and the KMS shall combine them into the BDK.

After the BDK has been combined, the BDK check value shall be calculated and verified.

If the check value matches, the BDK may be formally stored and used for DUKPT-related key derivation. If the check values do not match, the operation shall be stopped immediately and the issue shall be investigated.

### 5.4 BDK Parameter Configuration

After the BDK has been loaded, our company shall configure DUKPT-related parameters for the specific project, including but not limited to:

- BDK identifier;
- Key name, algorithm, and length;
- KSN format rules;

The relevant parameters shall be consistent with the information provided by the customer.

### 5.5 Method 1 Process Overview

The customer generates and splits the BDK
-> The customer transfers the BDK components in physical packages
-> Our company separately enters and combines the BDK components in the KMS
-> Both parties verify the BDK check value
-> The customer provides the KSN and related DUKPT parameters for configuration by our company
-> The BDK is activated.

## 6. DUKPT Method 2: Receipt of ZMK Components and TR-31-Formatted BDK Ciphertext

### 6.1 Method Description

Under this method, the customer does not directly provide plaintext BDK components to our company. Instead, the customer first provides ZMK components.

After the ZMK has been combined in our KMS, the customer uses the ZMK to protect the BDK and provides the BDK to our company as a TR-31-formatted key block.

The ZMK is used only for key exchange and key protection and is not used directly to encrypt or decrypt transaction data.

### 6.2 Step 1: Receive ZMK Key Components

The customer splits the ZMK into multiple key components and transfers them in physical packages with tamper-evident seals and unique serial numbers.

The physical package may contain:

- ZMK key component;
- Component number;
- Key algorithm and length;
- ZMK check value;
- Customer or project identifier;
- Key usage description;

Different ZMK components shall be held and transferred by different personnel and, wherever possible, shall be packaged independently.

### 6.3 Step 2: Enter and Combine the ZMK

Authorized key custodians of our company shall separately enter the ZMK components into the KMS, and the system shall combine them into the ZMK.

After the ZMK has been combined, its key check value shall be verified. Only after the value has been confirmed may the ZMK be used to unwrap the BDK ciphertext subsequently provided by the customer.

### 6.4 Step 3: Receive the TR-31-Formatted BDK Ciphertext

The customer uses the ZMK confirmed by both parties to protect the BDK and generates a TR-31-formatted BDK key block.

The BDK ciphertext file provided by the customer shall contain or clearly specify the following information:

- BDK key number;
- Key name, algorithm, and length;
- BDK check value;
- KSN-related parameters;
- TR-31 key block version and other necessary attributes.

The BDK ciphertext file may be transmitted through a secure electronic channel agreed by both parties.

All ZMK components and the BDK ciphertext file shall not be transmitted simultaneously through the same non-isolated channel.

### 6.5 Step 4: Import the BDK

After receiving the TR-31-formatted BDK ciphertext, our company shall import it into the KMS.

The KMS shall use the loaded ZMK to unwrap the BDK key block and perform the following checks:

1. TR-31 key block format check;
2. Key block integrity check;
3. Key algorithm and length check;
4. BDK check value check;

After all checks have passed, the BDK shall be securely stored in the KMS, and the corresponding KSN and other DUKPT parameters shall be configured according to the information provided by the customer.

### 6.6 Method 2 Process Overview

The customer generates and splits the ZMK
-> The customer transfers the ZMK components in physical packages
-> Our company separately enters and combines the ZMK components in the KMS
-> Both parties verify the ZMK check value
-> The customer uses the ZMK to encapsulate the BDK
-> The customer transfers the TR-31-formatted BDK ciphertext file
-> Our KMS imports and verifies the BDK
-> The customer provides the KSN and related DUKPT parameters for configuration by our company
-> The BDK is activated.

## 7. Summary of Key Exchange Methods

| Key Hierarchy | Phase 1 Exchange | Phase 2 Exchange | KMS Loading Result |
| --- | --- | --- | --- |
| MK/SK | Receive KEK components in physical packages | Receive TR-31-formatted TMK ciphertext protected by the KEK | Establish the KEK in the KMS and import the TMK |
| DUKPT Method 1 | Directly receive BDK components in physical packages | None | Directly combine and establish the BDK in the KMS |
| DUKPT Method 2 | Receive ZMK components in physical packages | Receive TR-31-formatted BDK ciphertext protected by the ZMK | Establish the ZMK in the KMS and import the BDK |

## 8. Information to Be Provided by the Customer

To ensure successful key loading, the customer should, in principle, provide the following information in advance:

1. Customer name and project name;
2. Key hierarchy to be used;
3. Key usage;
4. Key algorithm;
5. Key length;
6. Key version;
7. Key check value;
8. Number of key components;
9. TR-31 key block version;
10. Key block protection key information;
11. KSN format and range for the DUKPT hierarchy;
12. Contact person and key handover personnel information;
13. Other business parameters agreed by both parties.

The customer shall ensure that the provided key usage, algorithm, length, version, check value, and TR-31 key block attributes are mutually consistent.

## 9. Exception Handling

During key exchange and loading, our company may suspend operations if any of the following occurs:

- The physical package is damaged or the seal is abnormal;
- The number of key components does not match the agreed number;
- The source of the key components or the handover personnel cannot be verified;
- The key check values do not match;
- The TR-31 key block cannot be parsed;
- The TR-31 key block integrity check fails;
- The key usage, algorithm, or length is inconsistent with the agreement;
- The BDK does not match the KSN parameters;
- Any other anomaly that may affect key security.

If an anomaly occurs, both parties shall jointly confirm the cause. Where necessary, the customer shall regenerate and retransmit the key components or encrypted key file.

Without prior confirmation by both parties, a complete plaintext key shall not be sent directly by telephone, instant messaging tools, or ordinary email.

## 10. Completion and Result Confirmation

After the key has been successfully loaded into the KMS, our company shall report the loading result to the customer as agreed by both parties.

The reported information may include:

- Whether the key was loaded successfully;
- Key type;
- Key version;
- Key check value;
- Project identifier;
- KSN parameter configuration result;
- Current key status;
- Operation date;
- Other non-sensitive confirmation information.

The reported information shall not contain the complete plaintext key, all key components, or any sensitive data that could be used to reconstruct the complete key.

## 11. Summary

Our KMS supports the MK/SK and DUKPT key hierarchies.

For the MK/SK key hierarchy, our company first receives and enters KEK components delivered in physical packages, and then receives and imports a TR-31-formatted TMK ciphertext protected by that KEK.

For the DUKPT key hierarchy, the customer may either provide BDK components directly or first provide ZMK components and then provide a TR-31-formatted BDK ciphertext protected by the ZMK.

Regardless of the method used, key exchange and loading shall follow the principles of key-component separation, dual control, separation of transmission channels, integrity verification, need-to-know access, and complete audit trails, thereby ensuring effective protection of customer keys throughout their lifecycle.
