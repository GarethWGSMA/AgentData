---
source: "TS.22_v6.0.docx"
chunk_id: 032
section_path:
  - "1.1.1. (U)SIM based EAP methods and 3GPP Service Provider selection"
---

## 1.1.1. (U)SIM based EAP methods and 3GPP Service Provider selection

Release 12 and post-release 12 devices, procedures are specified in TS 24.302 [3GPP TS 24.302] clause 5.2.3.2.

| Req ID | Requirement |
| --- | --- |
| TSG22_R2_SEC_01 | VOID |
| TSG22_R2_SEC_02 | A device with a SIM inserted and selected SHALL use EAP-SIM to authenticate with a WLAN that has a roaming agreement (either direct or via a VPLMN) with the HPLMN of the SIM. |
| TSG22_R2_SEC_03 | A device with a UICC inserted and a USIM selected SHALL by default use either EAP-AKA or EAP-AKA’ to authenticate with a WLAN that has a roaming agreement (either direct or via a VPLMN) with the HPLMN of the USIM. |
| TSG22_R2_SEC_04 | It SHALL be possible for the operator to configure whether a device, with a USIM inserted and a USIM selected, is allowed to use EAP-SIM (when supported by the USIM) when connecting to a WLAN that has a roaming agreement (either direct or via a VPLMN) with the HPLMN of the USIM. This might be, for example, in the factory or by another method.<br><br>Note: This is to cover the case where the HPLMN AAA does not support EAP-AKA or EAP-AKA’. |
| TSG22_R2_SEC_05 | It SHALL be possible for the operator to configure whether a device, with a USIM inserted and a USIM selected, shall use EAP-AKA or EAP-AKA’ when connecting to a WLAN that has a roaming agreement (either direct or via a VPLMN) with the HPLMN of the USIM. This might be, for example, in the factory or by another method. |
| TSG22_R2_SEC_06 | VOID |
| TSG22_R3_SEC_09 | A device SHALL support identity privacy mechanisms described in EAP-SIM [RFC 4186] / EAP-AKA [RFC 4187] / EAP-AKA’ [RFC 5448] |
| TSG22_R3_SEC_10 | A device, with a USIM inserted and a USIM selected, SHALL store the pseudonym, re-authentication identities and related parameters used in the identity privacy mechanism and in the fast re-authentication mechanism, respectively, in the UICC when the corresponding files are present as specified in [3GPP TS 31.102], so that it can be maintained across reboots. |
| TSG22_R4_SEC_11 | A pre-release 12 device, with a USIM inserted and a USIM selected, SHALL support PLMN selection procedure as specified in TS 24.234 [3GPP TS 24.234] clause 5.2. |
| TSG22_R4_SEC_12 | A release 12 or post-release 12 device, with a USIM inserted and a USIM selected, SHALL support 3GPP Service Provider selection as defined in TS 24.302 [3GPP TS 24.302] clause 5.2.3.2. |
| TSG22_R6_SEC_13 | It SHALL be possible for a device to request the available EAP methods, to determine if they correspond to the type of SIM/UICC it holds, when connecting to a WLAN access network. |
