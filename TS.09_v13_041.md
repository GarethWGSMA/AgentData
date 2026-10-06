---
source: "TS.09_v13.docx"
chunk_id: 041
section_path:
  - "2.10.3 5G-NR (FR1) Data Transfer Parameters"
---

## 2.10.3 5G-NR (FR1) Data Transfer Parameters

Further assumptions:

When the DUT is in active state, CQI is assumed to be periodic and scheduled such that it is sent every 40 ms to the network. If cDRX feature and CQI reporting cannot be enabled in the same test case due to some test equipment limitations, cDRX enabling shall be preferred to CQI reporting, and the final choice mentioned in the measurement report.
No SRS is transmitted.
No HARQ and ARQ retransmissions are expected – low bit error rate is assumed
No System Information (on PDSCH or PBCH) or paging is received.
A test duration of ten minutes is assumed.

Upload:

The same general parameters as for the 5G-NR FDD and TDD file download use case as defined in table 5G-NR 2 shall be used. The bandwidth and resource allocation shall however be modified as shown in table 5G-NR 3.

| Parameter | Value | Value | Comment |
| --- | --- | --- | --- |
| Parameter | FDD | TDD | Comment |
| DL & UL Channel bandwidth | 10 MHz | 100 MHz | This configuration corresponds to 5Mbit/s uplink for FDD, while 2 Mbit/s for TDD. |
| Uplink downlink configuration | NA | 1 | This configuration corresponds to 5Mbit/s uplink for FDD, while 2 Mbit/s for TDD. |
| Special sub-frame configuration | NA | 4 | This configuration corresponds to 5Mbit/s uplink for FDD, while 2 Mbit/s for TDD. |
| Allocated resource blocks in UL | 11 | 11 | This configuration corresponds to 5Mbit/s uplink for FDD, while 2 Mbit/s for TDD. |
| TBS Index in UL | 20 | 20 | This configuration corresponds to 5Mbit/s uplink for FDD, while 2 Mbit/s for TDD. |
| Allocated resource blocks in DL | 3% of the UL data rate shall be assumed for transferring TCP ACKs in DL | 3% of the UL data rate shall be assumed for transferring TCP ACKs in DL | This configuration corresponds to 5Mbit/s uplink for FDD, while 2 Mbit/s for TDD. |
| TBS Index in DL | 20 | 20 | This configuration corresponds to 5Mbit/s uplink for FDD, while 2 Mbit/s for TDD. |
| PDCCH length | 2 Symbols | 2 Symbols | This configuration corresponds to 5Mbit/s uplink for FDD, while 2 Mbit/s for TDD. |
| OCNG in DL | According to Table 5G-NR_FDD_Idle_1 | According to Table 5G-NR_TDD_Idle_1 | Refer to [20], Annex A.5.1.1 (FDD) and A.5.1.2 (TDD) |

: 5G-NR 3 / General parameters for 5G-NR FDD File Upload use case

Further assumptions:

CQI is assumed to be periodic and scheduled such that it is sent every 40 ms to the network
No SRS is transmitted
No HARQ and ARQ retransmissions are expected – low bit error rate is assumed
No System Information (on PDSCH or PBCH) or paging is received.

Parallel Download/Upload:

The same general parameters as for the 5G-NR FDD and TDD file download use case as defined in Table 5G-NR 2 shall be used. The bandwidth and resource allocation shall however be modified as shown in Table 5G-NR 4.

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
| OCNG in DL | According to Table 5G-NR_FDD Idle_1 | According to Table 5G-NR_TDD Idle_1 | Refer to [20], Annex A.5.1.1 (FDD) and A.5.1.2 (TDD) |
