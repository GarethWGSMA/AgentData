---
source: "TS.09_v13.docx"
chunk_id: 014
section_path:
  - "2.3.2 GSM/GPRS Standby Parameters"
---

## 2.3.2 GSM/GPRS Standby Parameters

For GPRS most of the key parameters can be kept from GSM configuration (see section 2.3.1) but the paging type and interval needs to be addressed.

Two possibilities for paging types are available:

1. Network mode of operation I. All paging messages (GSM or GPRS) are sent on the PPCH - or CCCH-PCH if no PPCH is present. In PS connected mode CS paging arrives on the PDTCH.
1. Network mode of operation II. All paging messages are sent on the CCCH-PCH whether PS connected or not. This means the mobile equipment must monitor paging channel even when in a packet call.

Most deployed GPRS networks operate in network mode I or network mode II, therefore mode II has been adopted as the standard. For simplicity the paging has been selected to arrive on the CCCH-PCH

Finally, the paging interval needs to be considered. As the decisions on paging mode and channel lead to use the same paging system as in GSM, the same paging interval was selected: 5 multi frames.

| Parameter | Value | Comment |
| --- | --- | --- |
| Network Mode of Operation | II |  |
| Paging Channel | CCCH-PCH |  |
| Paging Interval | 5 Multi Frames |  |
| All other Parameters | As for GSM Standby |  |

: GSM/GPRS parameters for Standby Time

NOTE:	The selected parameters for GSM/GPRS standby are effectively the same as those used in GSM. Therefore, the same results should be obtained when measuring/modelling GSM and GSM/GPRS as per the details above.
