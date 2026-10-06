---
source: "TS.09_v13.docx"
chunk_id: 029
section_path:
  - "2.6.3 E-UTRA PS Data Transfer Parameters"
---

## 2.6.3 E-UTRA PS Data Transfer Parameters

: E-UTRA 2 / General parameters for E-UTRA FDD and
TDD File Download use case

NOTE:	Output power: The mean power of one carrier of the UE, delivered to a load with resistance equal to the nominal load impedance of the transmitter.

Mean power: When applied to E-UTRA transmission this is the power measured in the operating system bandwidth of the carrier. The period of measurement shall be at least one sub-frame (1 ms) for frame structure type 1 and one sub-frame (0.675 ms) for frame structure type 2 excluding the guard interval, unless otherwise stated.

Further assumptions:

. When the DUT is in active state, CQI is assumed to be periodic and scheduled such that it is sent every 40 ms to the network. If cDRX feature and CQI reporting cannot be enabled in the same test case due to some test equipment limitations, cDRX enabling shall be preferred to CQI reporting, and the final choice mentioned in the measurement report.
. No SRS is transmitted.
. No HARQ and ARQ retransmissions are expected – low bit error rate is assumed
. No System Information (on PDSCH or PBCH) or paging is received.
. A test duration of ten minutes is assumed.

Upload:

The same general parameters as for the E-UTRA FDD and TDD file download use case as defined in table E-UTRA_2 shall be used. The bandwidth and resource allocation shall however be modified as shown in table E-UTRA 3.

| Parameter | Value | Value | Comment |
| --- | --- | --- | --- |
| Parameter | FDD | TDD | Comment |
| DL & UL Channel bandwidth | 10 MHz | 10 MHz | This configuration corresponds to 5Mbit/s uplink for FDD, while 2 Mbit/s for TDD. |
| Uplink downlink configuration | NA | 1 | This configuration corresponds to 5Mbit/s uplink for FDD, while 2 Mbit/s for TDD. |
| Special sub-frame configuration | NA | 4 | This configuration corresponds to 5Mbit/s uplink for FDD, while 2 Mbit/s for TDD. |
| Allocated resource blocks in UL | 11 | 11 | This configuration corresponds to 5Mbit/s uplink for FDD, while 2 Mbit/s for TDD. |
| TBS Index in UL | 20 | 20 | This configuration corresponds to 5Mbit/s uplink for FDD, while 2 Mbit/s for TDD. |
| Allocated resource blocks in DL | 3% of the UL data rate shall be assumed for transferring TCP ACKs in DL | 3% of the UL data rate shall be assumed for transferring TCP ACKs in DL | This configuration corresponds to 5Mbit/s uplink for FDD, while 2 Mbit/s for TDD. |
| TBS Index in DL | 20 | 20 | This configuration corresponds to 5Mbit/s uplink for FDD, while 2 Mbit/s for TDD. |
| PDCCH length | 2 Symbols | 2 Symbols | This configuration corresponds to 5Mbit/s uplink for FDD, while 2 Mbit/s for TDD. |
| OCNG in DL | According to Table E-UTRA_FDD_Idle_1 | According to Table E-UTRA_TDD_Idle_1 | [13], Annex A.5.1.2 |

: E-UTRA 3 / General parameters for E-UTRA FDD File Upload use case

Further assumptions:

. CQI is assumed to be periodic and scheduled such that it is sent every 40 ms to the network
. No SRS is transmitted
. No HARQ and ARQ retransmissions are expected – low bit error rate is assumed
. No System Information (on PDSCH or PBCH) or paging is received.

Parallel Download/Upload:
