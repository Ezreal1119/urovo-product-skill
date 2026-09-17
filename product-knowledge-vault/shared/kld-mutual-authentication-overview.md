# KLD Mutual Authentication Overview

Multi-product English overview of KLD (Master / KDH) and slave-device (Sub-POS / PED / KRD) **mutual certificate authentication** before TR-34-style key injection. The body text does not name a market model.

## Synchronized Source

- Original: `_shared/operations/kld-mutual-authentication-overview_202609112225/KLD_Mutual_Authentication_Overview.docx`
- Markdown: `_shared/operations/kld-mutual-authentication-overview_202609112225/KLD_Mutual_Authentication_Overview.md`
- SHA-256: `84e4e5b83f536e35f39a95a5cd9a0443abeca07302e6ffe36cdf7b46220d2eaf`
- Format: DOCX, 3 pages, 0 embedded images
- Distinct from [[shared/kld-operation-manual|KLD Operation Manual]] (app UI / login / Load Key)

## Covered Product Hubs

POS-wide operational documentation. Backlinks are on the current POS Product Hubs.

- [[products/i5300|i5300]]
- [[products/i5300L|i5300L]]
- [[products/i9000S|i9000S]]
- [[products/i9100|i9100]]
- [[products/i9200|i9200]]
- [[products/i9600|i9600]]

Related: [[shared/kms-standard-solution-key-exchange-en|KMS Standard Solution — Customer Key Exchange and KMS Key Loading]]; [[shared/kld-operation-manual|KLD Operation Manual]].

## Content Scope

- Roles: KLD (Master, KDH) holds keys; Slave device (Sub-POS / PED, KRD) receives keys.
- Materials: CAKRD / CredKRD; CAKDH / CredKDH; CRL (CAKDH) delivered with bind/exchange responses.
- Key injection must not start before mutual authentication completes.
- Check Binding: slave sends SN/Device ID + CredKRD; KLD verifies with preloaded CAKRD and matches certificate serial number to device SN; KLD returns CredKDH + CRL; slave verifies with preloaded CAKDH (CAKDH is not re-delivered).
- After success: Query Key List → TR-34-style Key Exchange (wrap with slave credential, KLD signs) → Key Verify (e.g. KCV) → Status Update. Multi-key cycles may repeat. Message fields and algorithms are out of scope.

## Query Guidance

Use this source for **how KLD and a Sub-POS authenticate each other with certificates** before injection. For tapping through the KLD Android UI, use [[shared/kld-operation-manual|KLD Operation Manual]]. For customer-to-UROVO KMS exchange packages, use [[shared/kms-standard-solution-key-exchange-en|KMS Standard Solution]].

## Active Source Discrepancies

No unresolved same-context contradiction with other current local sources was identified.
