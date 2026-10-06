---
source: "TS.09_v13.docx"
chunk_id: 017
section_path:
  - "2.4.2 WCDMA Talk Time Parameters"
---

## 2.4.2 WCDMA Talk Time Parameters

All common parameters (section 2.2) apply, plus the WCDMA bearer configuration is described below. Some bearer parameters are left to the vendor to decide. In these cases the values used must be reported with the test results.

| Parameters | Value | Comment |  |
| --- | --- | --- | --- |
| Serving Cell UARFCN (downlink) | Band I: Mid Range<br>Band II: Mid Range<br>Band IV: Mid Range<br>Band V: Mid Range<br>Band VI: Mid Range<br>Band VIII: Mid Range<br>Band IX: Mid Range | All bands supported by the terminal must be measured.<br>Results must indicate which band(s) have been measured, and individual result for each band |  |
| Serving Cell UARFCN (uplink) | Band I: Mid Range<br>Band II: Mid Range<br>Band IV: Mid Range<br>Band V: Mid Range<br>Band VI: Mid Range<br>Band VIII: Mid Range<br>Band IX: Mid Range |  |  |
| Serving Cell Scrambling Code | 255 |  |  |
| Use Secondary Scrambling Code | No |  |  |
| Fixed Channelisation Code | Yes |  |  |
| Hard Handover | No |  |  |
| Soft / Softer Handover | No |  |  |
| Channel type – UL & DL / Bearer | Voice 12.2k (AMR)<br>"Conversational / speech / UL:12.2 DL:12.2 kbps / CS RAB + UL:3.4 DL:3.4 kbps SRBs for DCCH" (as defined in 3GPP TS25.993-6.7.0 Ref #4) |  |  |
| Loc | -60 dBm | Refer to [9], Section 7.2. |  |
|  | -1 dB | Refer to [9], Section 7.2. |  |
| CPICH_Ec/Ior | -10 dB | Refer to [9], Annex E.3.3 | Refer to [9], Annex E.3.3 |
| P-CCPCH_Ec/Ior | -12 dB | Refer to [9], Annex E.3.3 | Refer to [9], Annex E.3.3 |
| DPCH_Ec/Ior | -15 dB | 1.6 dB better than performance test cases in [9], Section 7.2 | 1.6 dB better than performance test cases in [9], Section 7.2 |
| Uplink DTX | No |  |  |
| Terminal Tx level | 1) Fixed value of 10 dBm<br>AND<br>2) Power distribution as defined below |  |  |
| Number of neighbours declared in the BA_LIST | 16 | See NOTE below |  |
| Neighbour cells on different frequency | No |  |  |

: WCDMA parameters for Talk Time

NOTE:	Although the mobile equipment is required to monitor these neighbour cells, the test equipment does not provide signals. No signals should be present on the neighbour frequencies. If signals are present then the terminal will attempt to synchronise and this is not part of the test. The number of neighbours are the number of intra-frequency neighbours. No GSM neighbour cell is declared in the Inter-RAT neighbour list for WCDMA Standby test.

Power distribution should be programmed as follows:

: Terminal Tx Power distribution for WCDMA

| Power dBm | % of time<br>class 3 | % of time<br>class 4 |
| --- | --- | --- |
| 24 | 0,6 | n/a |
| 21 | 1,2 | 1,8 |
| 18 | 2 | 2 |
| 15 | 1,5 | 1,5 |
| 12 | 3,5 | 3,5 |
| 9 | 5,3 | 5,3 |
| 6 | 8 | 8 |
| 3 | 10,6 | 10,6 |
| 0 | 12,2 | 12,2 |
| -3 | 12,9 | 12,9 |
| -6 | 12,2 | 12,2 |
| -9 | 10,6 | 10,6 |
| -12 | 7,9 | 7,9 |
| -15 | 5,3 | 5,3 |
| -20 | 3,5 | 3,5 |
| -30 | 1,5 | 1,5 |
| -40 | 0,7 | 0,7 |
| -50 | 0,5 | 0,5 |
| Total | 100 | 100 |

: UE Tx Power distribution for WCDMA
. This is designed to exercise the (non-linear) WCDMA power amplifier across its full range. The data is taken from operation on a live network.
. The method of testing involves averaging over a defined period. A test set must be configured to produce the relevant power for the relevant percentage of that period
. Alternatively, depending on the test set, it may be easier to individually measure the current at each power level and average according to the % weighting given.
. To ensure that results are always repeatable, the measurements should always be made with the DUT moving from minimum power to maximum power. This will minimise any effects due to residual heat in the DUT after transmitting at higher power levels.
