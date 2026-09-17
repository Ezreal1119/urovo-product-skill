# KLD and Slave Device Authentication

> Canonical original retained (bytes unchanged). This Markdown companion preserves the extractable text layer. Visual protocol: 3/3 converted-PDF pages inspected; the source is a text/table DOCX with **0** embedded images (no diagrams beyond table layout).
>
> - Original: `_shared/operations/kld-mutual-authentication-overview_202609112225/KLD_Mutual_Authentication_Overview.docx`
> - SHA-256: `84e4e5b83f536e35f39a95a5cd9a0443abeca07302e6ffe36cdf7b46220d2eaf`
> - Title: KLD and Slave Device Authentication
> - Language: English
> - Scope: POS-wide mutual authentication before key injection. The body does not name a market model.
> - Distinct from: `_shared/operations/kld-operation-manual_202608181911/` (KLD **app operation** / UI), which is a different document identity.

---

## 1. Roles and Certificates

### Roles

| Role | Description |
| --- | --- |
| KLD (Master) | The party that holds keys and performs injection (Key Distribution Host, KDH) |
| Slave device (Sub-POS / PED) | The party that receives keys (Key Receiving Device, KRD) |

### Certificates / materials

| Certificate / Material | Meaning |
| --- | --- |
| CAKRD | Root CA of the slave-device certificate chain (KRD CA) |
| CredKRD | Slave-device certificate (issued by CAKRD) |
| CAKDH | Root CA of the KLD certificate chain (KDH CA) |
| CredKDH | KLD device certificate (issued by CAKDH) |
| CRL (CAKDH) | KDH-side certificate revocation list, delivered with bind / exchange responses for slave-side verification |

Key injection must not start before mutual authentication is completed.

## 2. Mutual Authentication before Key Injection

Both parties complete mutual authentication through Check Binding: the slave initiates the bind request; the KLD verifies the slave identity and returns its own credential; the slave then verifies the KLD identity.

### 2.1 Slave → KLD (How the KLD authenticates the slave)

1. The slave sends a bind request carrying: device identity (SN / Device ID) and CredKRD (the slave X.509 certificate).
2. The KLD verifies CredKRD using the locally preloaded CAKRD (certificate chain / signature verification).
3. The KLD compares the CredKRD certificate serial number with the device SN in the request (on success, the certificate is treated as bound to that physical device).
4. After successful verification, the KLD stores CredKRD for later key-injection use (for example, protecting key material with the slave public key).

If any step fails, binding fails and subsequent key injection does not proceed.

### 2.2 KLD → Slave (How the slave authenticates the KLD)

1. On successful binding, the KLD response delivers CredKDH (KLD device certificate) and the CAKDH CRL (revocation list).
2. The slave verifies CredKDH in the response using the locally preloaded CAKDH.
3. The slave verifies the CRL as required to ensure CredKDH has not been revoked.
4. After successful verification, the slave trusts the KLD and stores / updates local CredKDH for later exchange-phase signature verification, etc.

Key points:

- The KLD trusts CAKRD → CredKRD and checks the SN.
- The slave trusts CAKDH → CredKDH (and the CRL).
- The bind response delivers CredKDH and the CRL; it does not re-deliver CAKDH (CAKDH is preloaded on the slave).

## 3. High-Level TR-34 Style Key Injection Flow

After mutual authentication succeeds, both parties complete TR-34 key injection in a request–response manner. At a high level:

Mutual authentication → Query injectable keys → Key exchange (encrypted key block + signature) → Key verification (e.g. KCV) → Status confirmation

| Stage | Purpose (high level) |
| --- | --- |
| Check Binding | Complete the mutual certificate and device-identity verification described above; establish trust in the peer public key needed for later sessions |
| Query Key List | The slave queries the KLD for the list of keys available for injection (type / identifier, etc.) |
| Key Exchange | Under mutual trust, wrap the key to be injected in a TR-34 key-block style: protect key material with the slave credential, and have the KLD private key sign the exchange data; the slave verifies the signature, unwraps, and loads the key |
| Key Verify | The slave and KLD check integrity / correctness of the injected key (e.g. KCV comparison) |
| Status Update | The slave reports injection status; the KLD confirms whether this round (or the accumulated multi-key process) is complete |

For multiple keys, the cycle “exchange → verify → status” may be repeated until the list is complete. Message field definitions, algorithms, and step-by-step cryptographic operations are out of scope for this document.

## 4. Trust Relationship Summary

Trust relationship overview:

- CAKRD (preloaded on the KLD) is used to issue/verify CredKRD; the slave presents CredKRD in the bind request.
- CAKDH (preloaded on the slave) is used to verify CredKDH (and the CRL) delivered by the KLD.
- After mutual authentication succeeds, the TR-34 key-injection flow proceeds.

| Verifier | Subject | Basis |
| --- | --- | --- |
| KLD | Slave device | CAKRD verifies CredKRD; CredKRD serial number matches device SN |
| Slave device | KLD | Local CAKDH verifies CredKDH; CRL verified as required |

### Visual notes (pages 1–3)

All three pages are black body text and bordered tables on a white background. No product photos, screenshots, logos, or flow-chart graphics. Page 1 heading **KLD and Slave Device Authentication**; sections 1–2.1. Page 2 continues 2.1 step 4 through section 3 (table through Key Verify). Page 3 completes Key Verify / Status Update, the multi-key cycle note, and section 4.
