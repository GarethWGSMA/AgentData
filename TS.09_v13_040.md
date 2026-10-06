---
source: "TS.09_v13.docx"
chunk_id: 040
section_path:
  - "2.10.3 5G-NR (FR1) Data Transfer Parameters"
---

## 2.10.3 5G-NR (FR1) Data Transfer Parameters

Download:

Some bearer parameters shall be selected among some recommended values. These parameters and the selected value shall be reported with the tests results.

| Parameter | Recommended Value | Recommended Value | Comment |
| --- | --- | --- | --- |
| Parameter | FDD | TDD | Comment |
| Serving Cell Downlink EARFCN | Mid range for all supported 5G-NR bands | Mid range for all supported 5G-NR bands | All bands supported by the handset must be measured.<br>Results must indicate which band(s) have been measured, and individual result for each band. |
| Serving Cell Uplink EARFCN | Mid range for all supported 5G-NR bands | Mid range for all supported 5G-NR bands | All bands supported by the handset must be measured.<br>Results must indicate which band(s) have been measured, and individual result for each band. |
| Number of neighbours declared in the neighbour cell list | 16 intra-frequency,<br>0 inter-frequency,<br>0 inter-RAT,<br>no MBSFN cells (in case of EN-DC or DSS) | 16 intra-frequency,<br>0 inter-frequency,<br>0 inter-RAT,<br>no MBSFN cells (in case of EN-DC or DSS) | Although the mobile equipment is required to monitor these neighbour cells, the test equipment does not in fact provide signals. |
| Reference Signal Energy Per Resource Element (RS EPRE) | -85 dBm/15kHz | -85 dBm/15kHz | Refer to [20], Annex C.0<br>Default value used for 3GPP performance test setup and signalling tests. |
| SSS |  |  | Refer to [20], Annex C.2 |
| PSS | NA | NA | Refer to [20], Annex C.2 |
| PDCCH | NA | NA | Refer to [20], Annex C.2 |
| PDSCH | NA | NA | Refer to [20], Annex C.2 |
| PBCH DMRS | NA | NA | Refer to [20], Annex C.2 |
| PDCCH DMRS | NA | NA | Refer to [20], Annex C.2 |
| PDSCH DMRS | NA | NA | Refer to [20], Annex C.2 |
| CSI-RS | NA | NA | Refer to [20], Annex C.2 |
| RoHC | No | No |  |
| UL TX Power level | 10 dBm | 10 dBm | The output power of the DUT as defined in [16]<br>See NOTE below |
| DL Transmission scheme | 2x2 closed loop spatial multiplexing | 4x4 closed loop spatial multiplexing | i.e. uses TX Mode 4 |
| Cyclic Prefix Length | Normal | Normal | No extended cyclic prefix |
| PHICH Duration | Normal | Normal | 1 symbol only, no extended PHICH |
| Aggregation Level | 4 CCEs | 8 CCEs | Refer to [20],C.3.1 |
| DL and UL Channel Bandwidth | 10 MHz | 100 MHz |  |
| Uplink downlink configuration | NA | 1 |  |
| Special subframe configuration | NA | 4 |  |
| Slot configuration pattern | N/A | DDDSUDDSUU |  |
| Allocated resource blocks in DL | 52 (SCS=15kHz, BW=10MHz) | 273 (SCS=30kHz, BW=100MHz) |  |
| TBS Index in DL | 19 | 19 |  |
| Allocated resource blocks in UL | 3% of the DL data rate shall be assumed for transferring TCP ACKs in UL | 3% of the DL data rate shall be assumed for transferring TCP ACKs in UL |  |
| TBS Index in UL | 20 | 20 |  |
| PDCCH length | 2 symbols | 2 symbols |  |
| OCNG | According to Table 5G-NR_FDD_Idle_1 | According to Table 5G-NR_TDD_Idle_1 | Refer to [20], Annex A.5.1.1 (FDD) and A.5.1.2 (TDD) |
| DRX Configuration | DRX : On | DRX : On |  |
| LongDRX-Cycle | 320 sub-frames | 320 sub-frames | Result must indicate used value |
| onDuration Timer | 2 sub-frames | 2 sub-frames | Result must indicate used value |
| DRX-Inactivity Time | 100 sub-frames | 100 sub-frames | Result must indicate used value |
| Short DRX | Off | Off |  |

: 5G-NR 2 / General parameters for 5G-NR FDD and
TDD File Download use case

NOTE:	Output power: The mean power of one carrier of the UE, delivered to a load with resistance equal to the nominal load impedance of the transmitter.

Mean power: When applied to 5G-NR transmission this is the power measured in the operating system bandwidth of the carrier. The period of measurement shall be at least one sub-frame (1 ms) for frame structure type 1 and one sub-frame (0.675 ms) for frame structure type 2 excluding the guard interval, unless otherwise stated.
