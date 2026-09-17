# KMS Standard Solution — Customer Key Exchange and KMS Key Loading

Multi-product English operational instruction (V1.0, 2026-07-13) for exchanging customer keys into UROVO's Key Management System (KMS) and loading them. It describes the MK/SK and DUKPT hierarchies; it does not name a specific market model.

## Synchronized Source

- Original: `_shared/operations/kms-standard-solution-key-exchange-en_202608181911/KMS-Standard-Solution-Customer-Key-Exchange-and-KMS-Key-Loading-EN_V1.0.docx`
- Markdown: `_shared/operations/kms-standard-solution-key-exchange-en_202608181911/KMS-Standard-Solution-Customer-Key-Exchange-and-KMS-Key-Loading-EN_V1.0.md`
- Version: V1.0, Zhang Weixiang, 2026.7.13 (initial release)
- SHA-256: `44877b44cbb018cd68104f2debeb7ed67c620af7faac4c74d1171cc020368989`
- Format: DOCX; 1 embedded cover logo (UROVO / 优博讯 / 领跑行业移动应用) transcribed in the companion

## Covered Product Hubs

This source is **POS-wide process documentation**: it standardizes customer-to-UROVO KMS key exchange for payment terminals and does not enumerate market models. Backlinks are on the current POS Product Hubs.

- [[products/i5300|i5300]]
- [[products/i5300L|i5300L]]
- [[products/i9000S|i9000S]]
- [[products/i9100|i9100]]
- [[products/i9200|i9200]]
- [[products/i9600|i9600]]

Related device-side loading procedure: [[shared/kld-operation-manual|KLD Operation Manual]].

## Content Scope

- Purpose: standardize key exchange, receipt, verification, and loading so keys stay confidential, intact, and traceable.
- Two KMS-supported hierarchies: **MK/SK** and **DUKPT**.
- Principles: separation of key components, dual control, separation of transmission channels, complete audit trail, need-to-know.
- MK/SK flow: receive KEK components in tamper-evident physical packages → enter/combine/verify KCV in KMS → receive TR-31 TMK ciphertext protected by that KEK → import/unwrap/activate TMK.
- DUKPT method 1: receive BDK components in physical packages, combine/verify, then configure KSN and related parameters.
- DUKPT method 2: receive ZMK components, then receive TR-31 BDK ciphertext protected by the ZMK; ZMK is for key exchange/protection only, not for encrypting or decrypting transaction data.
- Customer information checklist, exception handling (including a ban on sending a complete plaintext key by telephone, IM, or ordinary email without prior confirmation), and non-sensitive result confirmation.

## Query Guidance

Use this source for **how the customer and UROVO exchange keys into KMS** (KEK/TMK, BDK, ZMK, TR-31, KCV, KSN). It is not a product specification and does not document the on-device KLD UI. Preserve the V1.0 date and the exact hierarchy names. For Master POS / Sub-POS key injection screens and the key cable, use [[shared/kld-operation-manual|KLD Operation Manual]].

## Active Source Discrepancies

No unresolved same-context contradiction was identified.
