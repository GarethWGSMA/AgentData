---
source: "TS.22_v6.0.docx"
chunk_id: 025
section_path:
  - "4.5.1 3GPP WLAN Access Network Selection"
---

## 4.5.1 3GPP WLAN Access Network Selection

Per TS 23.402 [3GPP TS 23.402] clause 4.8.6.4, WLAN access network selection in a release 12 or post-release 12 device is based either on ANDSF policies as defined in TS 23.402 [3GPP TS 23.402] clause 4.8, or on RAN rules as defined in TS 23.401 [3GPP TS 23.401] clause 4.3.23 and TS 23.060 [3GPP TS 23.060] clause 5.3.21. Both ANDSF policies and RAN rules are provided by the 3GPP operator. The operator policies may indicate priority among WLAN access networks provisioned by the 3GPP operator. The 3GPP operator policies should have highest priority among all available policies in the device for network selection. However, user preference settings should be able to override 3GPP operator policies on WLAN selection.

A WLAN can provide the device with EPC access in two different flavours: either the WLAN is considered by the operator as a “Trusted access network” per TS 23.402 [TS 23.402] clause 4.3.1.2 and the Trusted WLAN (TWAN) can access a PDN GW via S2a interface, or the WLAN is considered by the operator as an “Untrusted access network” per TS 23.402 [TS 23.402] clause 4.3.1.2 and the device can connect to an Evolved Packet Data Gateway (ePDG) in order to access a PDN GW via S2b interface.

| Req ID | Requirement |
| --- | --- |
| TSG22_R2_CM_22 | A 3GPP device SHOULD consider policies for WLAN access network selection received from a 3GPP operator with the highest priority (unless overridden by user preference settings). |
| TSG22_R2_CM_23 | A device SHALL be able to support the association to a WLAN access network where the SSID is not broadcast. |
| TSG22_R4_CM_59 | A release 12 and post-release 12 device, SHALL consider policies received from the 3GPP operator i.e. either ANDSF policies including the support of RAN Assistance parameters as defined in TS 23.402 [3GPP TS 23.402] clause 4.8, or RAN rules as defined in TS 23.401 [3GPP TS 23.401] clause 4.3.23 and TS 23.060 [3GPP TS 23.060] clause 5.3.21 with highest priority (unless overridden by user preference settings). |
| TSG22_R4_CM_60 | A release 12 or post-release 12 device, when provisioned with both ANDSF and RAN rules, SHALL select the policy to be used as defined in TS 23.402 [3GPP TS 23.402]  clause 4.8.6.4 and TS 24.302 clause 6.10. |
| TSG22_R4_CM_61 | A release 12 or post-release 12 device, when using ANDSF, SHALL select a WLAN as defined  in TS 23.402 [3GPP TS 23.402] clause 4.8, TS 24.302 clauses 5.1.3.2.3, 6.8 and 6.10 and TS 24.312 [3GPP TS 24.312]. |
| TSG22_R4_CM_62 | A release 12 or post-release 12 device, when using RAN Rules, SHALL select a WLAN as defined in TS 36.304 [3GPP TS 36.304] clause 5.6 and in TS 36.331 [3GPP TS 36.331] clause 5.6.12 for E-UTRAN, in TS 25.304 [3GPP TS 25.304] clause 5.10 and in TS 25.331 [3GPP TS 25.331] for UTRAN. |
