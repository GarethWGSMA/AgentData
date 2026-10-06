---
source: "TS.22_v6.0.docx"
chunk_id: 018
section_path:
  - "3.1.3 3GPP Operator policy coexistence"
---

## 3.1.3 3GPP Operator policy coexistence

The WLAN access selection and the traffic routing behaviour of a device using SIM credentials within a single PLMN shall be controlled either by the ANDSF rules or by the RAN rules not by both. The device can be provisioned with both policies, and the device shall select the policy to be used as defined in TS 23.402 [3GPP TS 23.402] clause 4.8.6.4 and TS 24.302 [3GPP TS 24.302] clause 6.10.

3GPP Home Operator and/or Visited Operator policies may be used to assist the device in selecting a WLAN access point and in steering traffic between 3GPP and WLAN accesses.

For WLAN selection, according to TS 24.302 [3GPP TS 24.302] clause 5.1.3.2.3, the following applies:

- When the network uses RAN rules with a release 12 or post-release 12 device as defined in TS 23.401 [3GPP TS 23.401] clause 4.3.23 and TS 23.060 [3GPP TS 23.060] clause 5.3.21, a list of WLAN identities (e.g. SSID, HESSID) as part of RAN Assistance parameters may be sent by the 3GPP RAN to the device.
- When the network uses ANDSF rules with a release 12 or post-release 12 device as defined in TS 23.402 [3GPP TS 23.402] clause 4.8.2.1.6, the Home and Visited Operator WLAN Selection Policies (WLANSP) that include a list of Preferred Roaming Partners defined in WFA HS 2.0 [Passpoint] and identified by their PLMN identifiers or NAI Realms as specified in IEEE 802.11-2016 [IEEE 802.11-2016] and, for authentication purposes, a list of Preferred SSID may be sent to the device via OMA DM.

A device may be pre-provisioned by necessary subscription information (e.g. SSIDs and accompanying security keys) for connection to operator-owned WLAN access networks.

3GPP has, in addition, defined a set of I-WLAN parameters provisioned into the USIM [3GPP TS 31.102] to be used by the device. In addition, 3GPP has also defined OTA (Over The Air) mechanisms in order to update the USIM parameters including the WLAN parameters [3GPP TS 31.115] [3GPP TS 31.116]. However, as stated in TS 24.234 [3GPP TS 24.234] “WLAN Network Selection supersedes I-WLAN for device WLAN selection as specified in 3GPP TS 24.302 from Rel-12 onwards”. This means that WLAN selection and associated PLMN selection are non-backward compatible between Release 12 and pre-Release 12. This also means that Release 12 features are not supported by devices that use I-WLAN feature for WLAN selection and associated PLMN selection.

| Req ID | Requirement | Requirement |
| --- | --- | --- |
| TSG22_R2_CM_01 | A pre-Release 12 device SHALL support provisioning of WLAN parameters (e.g. network identifiers) using the USIM as specified in 3GPP TS 31.102 [3GPP TS 31.102] and 3GPP TS 24.234 [3GPP TS24.234]. However, as stated in TS 24.234 [3GPP TS 24.234] “WLAN Network Selection supersedes I-WLAN for device WLAN selection as specified in 3GPP TS 24.302 from Rel-12 onwards”, no such requirement exists for Release 12 and post-Release 12 devices. |  |
| TSG22_R3_CM_49 | A device that supports OMA DM Management Objects SHOULD support mandatory features of OMA DM Bootstrap as defined in [OMA Device Management Bootstrap] and the conditional features of OMA DM Bootstrap relevant to a GSMA device described in this document. |  |
| TSG22_R4_CM_50 | A Release 12 or post-release 12 device SHOULD support provisioning of WLAN parameters (e.g. network identifiers) using the USIM via 3GPP ANDSF as specified in TS 23.402 [3GPP TS 23.402] , TS 24.302 [3GPP TS 24.302] clauses 5.1.3.2.3, 6.8 and 6.10 and TS 24.312 [3GPP TS 24.312]. |  |
| TSG22_R4_CM_51 | A Release 12 or post-release 12 device SHOULD support provisioning of WLAN parameters (e.g. network identifiers) using the USIM via 3GPP RAN Rules provisioned by E-UTRAN/UTRAN as specified in TS 23.401 [3GPP TS 23.401], TS 23.060 [3GPP TS 23.060], TS 36.304 [3GPP TS 36.304] clause 5.6, TS 36.331 [3GPP TS 36.331] clause 5.6.12, TS 25.304 [3GPP TS 25.304] clause 5.10, TS 25.331 [3GPP TS 25.331]. |  |
