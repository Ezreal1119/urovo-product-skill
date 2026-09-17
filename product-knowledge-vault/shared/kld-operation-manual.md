# KLD Operation Manual

Multi-product English operation manual (cover date 2025.07.07) for the UROVO Key Loading Device (KLD) application on a Master POS, and for loading keys to a Sub-POS. The body text does not name a specific market model.

## Synchronized Source

- Original: `_shared/operations/kld-operation-manual_202608181911/KLD_Operation_20250707.docx`
- Markdown: `_shared/operations/kld-operation-manual_202608181911/KLD_Operation_20250707.md`
- Cover date: 2025.07.07
- SHA-256: `8926bd27a5e267fcbe6c6e70209d28ffe959d5840164eda106cde841f0b9394a`
- Format: DOCX with 35 embedded screenshots/photos (image1–image35); all inspected and transcribed in the companion

## Covered Product Hubs

This source is **POS-wide operational documentation** for Master POS (KLD) and Sub-POS key loading. It does not enumerate market models. Backlinks are on the current POS Product Hubs.

- [[products/i5300|i5300]]
- [[products/i5300L|i5300L]]
- [[products/i9000S|i9000S]]
- [[products/i9100|i9100]]
- [[products/i9200|i9200]]
- [[products/i9600|i9600]]

Related customer-to-KMS exchange process: [[shared/kms-standard-solution-key-exchange-en|KMS Standard Solution — Customer Key Exchange and KMS Key Loading]].

## Content Scope

- Dual-control login: Administrator A default password all `1`, Administrator B all `2`; both must be changed at first login. Operator A and Operator B must be created after first administrator login.
- Administrator **Key Import**:
  - Manual-Inputed BDK (TDES) (Import Menu also shows Manual-Inputed BDK AES): two plaintext components, per-component KCV(CMAC)/KCV(ECB), XOR KCV, then KSN Prefix (KSN, max 10 bytes), `randomDigits` 0 or 2, DUKPT key index 1–4.
  - Manual-Inputed KEK Key (XOR of two components, or plaintext plus all-zero second component) then **Import Master Key(ciphered)** from an XLS whose columns are SN, KEK index, master key index, ciphertext key, kcv, key algorithm (`TDES` / `AES128` / `AES192` / `AES256`).
- Administrator **Management**: Member Management (Add / Delete / Modify Operator Password), Record Management, Delete Key.
- Operator menu: **KMS Download CA**, **Load Key**, **Query Keys**, **Exit**. CA download requires the KLD SN to be bound in the background; if unbound, contact the UROVO team.
- Load Key: connect the key cable (KLD to Sub-POS), click **Load Key** on the Master POS first, then **Sync Key** on the Sub-POS. Sub-POS **Key Management System** may show `The CA Certificate is not exist, please download first`.
- Lockout: five wrong administrator passwords lock the device; activation card restores the KLD administrator password to the initial password. Screenshot error code `WARNMING! (0x73000003)`, button **ACTIVE >**, version `(1.37.24.0203)`, Safe mode.
- Screenshot-only identifiers (do not treat as catalog claims): KLD SN `20241119152801`; Sub-POS SN `98282135009171` version `55.20240719`; Sub-POS SN `80062347000011` version `65.20241025`. A photo also shows unrelated handwritten paper (2100/SQ29, PB100/SQ81, etc.); that paper is not KLD UI.

## Query Guidance

Use this source for **how to operate the KLD app** (administrator/operator login, BDK/KEK/TMK import, CA download, Load Key / Sync Key, lockout). Preserve on-screen labels and source spelling. It is not a product specification. For customer-to-UROVO KMS exchange (TR-31, ZMK, physical packages), use [[shared/kms-standard-solution-key-exchange-en|KMS Standard Solution]].

## Active Source Discrepancies

No unresolved same-context contradiction with other current local sources was identified. Screenshot version strings for KLD SN `20241119152801` differ across photos (`0.6.20241119104121` vs a truncated `2.0.2...`) and are different captures, not a Hub discrepancy.
