# Urovo OEMConfig User Manual

Multi-product operational manual for the UrovoOEMConfig application, which exposes Urovo-specific firmware management policies to EMM solutions via Google Play "managed configurations".

## Synchronized Source

- Original: `_shared/operations/urovo-oemconfig-manual_202608151815/Urovo-OEMConfig-Manual.pdf`
- Markdown: `_shared/operations/urovo-oemconfig-manual_202608151815/Urovo-OEMConfig-Manual.md`
- Version: Urovo OEMConfig 1.0, Release 1, Revision 0, 2023-03-17 (first release)
- SHA-256: `4cdd9b7dae13c6a7c38da6dbf342126a81694944c547cd5e1664640a17df7ad0`

## Covered Product Hubs

This source is **platform-wide**: the UrovoOEMConfig application applies to the UROVO Android device portfolio as a whole, not to a specific product subset. It therefore links no individual Product Hub. For MDM/EMM validation status by product and vendor, see [[shared/mdm-certification-summary|MDM Certification Summary]].

## Content Scope

- The OEMConfig standard and how UrovoOEMConfig exposes Urovo-specific firmware settings to EMM solutions.
- All OEMConfig v1.0 configuration groups, their actions, and mandatory configuration items: Clock, Display, NFC, FOTA, General UI, KeyRemap, Power, Wireless General, WLAN, WlanAdvanced, Scanner, and Device Management.
- Detailed configuration-item semantics, formats, and dependencies (e.g., WLAN Static IP and Proxy fields; KeyRemap programmable keys, key codes, broadcast actions, and Start Activity extras).
- Example programmable-key names for the EA630 and PA760 models (illustrative, not a claim about current product coverage).
- Appendix 1 (Android key codes, e.g., 3 = HOME, 4 = BACK, 187 = APP_SWITCH) and Appendix 2 (Device Capability list per model).

## Query Guidance

Use this source for how to configure Urovo-specific settings through an EMM (OEMConfig). It is an operational/configuration reference, not a product specification. Preserve the exact configuration-group, action, and item semantics and the manual's version (1.0, 2023-03-17). The example programmable-key names vary by model and must not be generalized to all products.

## Active Source Discrepancies

No unresolved same-context contradiction was identified.
