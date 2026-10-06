---
source: "TS.22_v6.0.docx"
chunk_id: 028
section_path:
  - "4.7 Traffic management across RATs"
---

## 4.7 Traffic management across RATs

Both ANDSF and RAN rules may use RAN assistance parameters as described in these clauses. ANDSF additionally uses OPI RAN Assistance parameter as defined in TS 24.312 [3GPP TS 24.312] clause 5.7.21B34. Coexistence between ANDSF and RAN rules is described in TS 23.402 [3GPP TS 23.402] clause 4.8.6.4.

| Req ID | Requirement |
| --- | --- |
| TSG22_R2_CM_39 | VOID |
| TSG22_R2_CM_40 | A device SHALL keep the 3GPP mobile network connection e.g. PDP contexts during WLAN access. |
| TSG22_R2_CM_41 | A device SHALL send a DHCP Release message to an AP to release its IP address in the following circumstances:<br>Users disconnect from applications<br>Users switch from the current network identifier to another<br>Users turn WLAN off<br>Users turn Flight Mode on when one network identifier is connected |
| TSG22_R2_CM_42 | A device SHOULD implement the Detecting Network Attachment in Ipv4 (DNAv4) [RFC 4436]. When implemented, the mechanism SHALL be applied every time a radio link to a new AP is established, even if the identity or network identifier (e.g. SSID) of the AP does not change. |
| TSG22_R2_CM_43 | VOID |
| TSG22_R2_CM_44 | VOID |
| TSG22_R2_CM_45 | VOID |
| TSG22_R4_CM_46 | Release 12 and post-release 12 devices SHOULD implement ANDSF traffic steering rules including the support of RAN Assistance parameters per TS 23.402 clause 4.8 (Inter-System Routing Policy and Inter-APN Routing Policy), TS 24.302 [3GPP TS 24.302] clauses 5.4, 6.8 and 6.10 and TS 24.312 [3GPP TS 24.312]. |
| TSG22_R4_CM_47 | Release 12 and post-release 12 devices SHOULD implement traffic steering using RAN rules per TS 23.401 clause 4.3.23, TS 23.060 [3GPP TS 23.060] clause 5.3.21., TS 36.304 [3GPP TS 36.304] clause 5.6 and TS 36.331 [3GPP TS 36.331] clause 5.6.12 for E-UTRAN, TS 25.304 [3GPP TS 25.304] clause 5.10 and TS 25.331 [3GPP TS 25.331] for UTRAN. |
| TSG22_R4_CM_48 | Release 12 and post-release 12 devices SHOULD implement 3GPP Rel-12 procedures for the support of moving PDN connections between 3GPP access and trusted WLAN where the device IP address is preserved. |
| TSG22_R4_CM_49 | Release 12 and post-release 12 devices SHOULD implement 3GPP procedures for the support of moving PDN connections between 3GPP access and untrusted WLAN where the device IP address is preserved. |
