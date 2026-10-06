---
source: "TS.09_v13.docx"
chunk_id: 030
section_path:
  - "2.6.3 E-UTRA PS Data Transfer Parameters"
---

## 2.6.3 E-UTRA PS Data Transfer Parameters

The same general parameters as for the E-UTRA FDD and TDD file download use case as defined in Table E-UTRA_2 shall be used. The bandwidth and resource allocation shall however be modified as shown in Table E-UTRA 4.

| Parameter | Value | Value | Comment |
| --- | --- | --- | --- |
| Parameter | FDD | TDD | Comment |
| DL & UL Channel bandwidth | 10 MHz | 10 MHz | This configuration corresponds to 50 Mbit/s downlink and 25 Mbit/s uplink for FDD or 28 Mbit/s downlink and 10 Mbit/s uplink for TDD.. |
| Uplink downlink configuration | NA | 1 | This configuration corresponds to 50 Mbit/s downlink and 25 Mbit/s uplink for FDD or 28 Mbit/s downlink and 10 Mbit/s uplink for TDD.. |
| Special sub-frame configuration | NA | 4 | This configuration corresponds to 50 Mbit/s downlink and 25 Mbit/s uplink for FDD or 28 Mbit/s downlink and 10 Mbit/s uplink for TDD.. |
| Allocated resource blocks in UL | 50 | 50 | This configuration corresponds to 50 Mbit/s downlink and 25 Mbit/s uplink for FDD or 28 Mbit/s downlink and 10 Mbit/s uplink for TDD.. |
| TBS Index in UL | 21 | 21 | This configuration corresponds to 50 Mbit/s downlink and 25 Mbit/s uplink for FDD or 28 Mbit/s downlink and 10 Mbit/s uplink for TDD.. |
| Allocated resource blocks in DL | 50 | 50 | This configuration corresponds to 50 Mbit/s downlink and 25 Mbit/s uplink for FDD or 28 Mbit/s downlink and 10 Mbit/s uplink for TDD.. |
| TBS Index in DL | 21 | 21 | This configuration corresponds to 50 Mbit/s downlink and 25 Mbit/s uplink for FDD or 28 Mbit/s downlink and 10 Mbit/s uplink for TDD.. |
| PDCCH length | 2 Symbols | 2 Symbols | This configuration corresponds to 50 Mbit/s downlink and 25 Mbit/s uplink for FDD or 28 Mbit/s downlink and 10 Mbit/s uplink for TDD.. |
| OCNG in DL | According to Table E-UTRA_FDD Idle_1 | According to Table E-UTRA_TDD Idle_1 | [13], Annex A.5.1.2 |

: E-UTRA 4 / General parameters for E-UTRA FDD File DL/UL use case

Further assumptions:

. When the DUT is in active state, CQI is assumed to be periodic and scheduled such that it is sent every 40 ms to the network. If cDRX feature and CQI reporting cannot be enabled in the same test case due to some test equipment limitations, cDRX enabling shall be preferred to CQI reporting and the final choice mentioned in the measurement report.
. No SRS is transmitted.
. No HARQ and ARQ retransmissions are expected – low bit error rate is assumed
. No System Information (on PDSCH or PBCH) or paging is received.
