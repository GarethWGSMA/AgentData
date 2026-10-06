---
source: "TS.09_v13.docx"
chunk_id: 026
section_path:
  - "2.6.2 E-UTRA (VoLTE) Talk Time Parameters"
---

## 2.6.2 E-UTRA (VoLTE) Talk Time Parameters

The E-UTRA bearer configuration for Voice over LTE tests is described below. Some bearer parameters shall be selected among some recommended values. These parameters and the selected value shall be reported with the tests results.

| Parameter | Recommended Value | Recommended Value | Comment |
| --- | --- | --- | --- |
| Parameter | FDD | TDD | Comment |
| Serving Cell Downlink EARFCN | MID RANGE for all supported E-UTRA bands | MID RANGE for all supported E-UTRA bands | All bands supported by the handset must be measured.<br>Results must indicate which band(s) have been measured, and individual result for each band. |
| Serving Cell Uplink EARFCN | MID RANGE for all supported E-UTRA bands | MID RANGE for all supported E-UTRA bands | All bands supported by the handset must be measured.<br>Results must indicate which band(s) have been measured, and individual result for each band. |
| Number of neighbours declared in the neighbour cell list | 16 intra-frequency,<br>0 inter-frequency,<br>0 inter-RAT,<br>no MBSFN cells | 16 intra-frequency,<br>0 inter-frequency,<br>0 inter-RAT,<br>no MBSFN cells | Although the mobile equipment is required to monitor these neighbour cells, the test equipment does not in fact provide signals. |
| Reference Signal Energy Per Resource Element (RS EPRE) | -85 dBm/15kHz | -85 dBm/15kHz | Refer to [13], Annex C.0<br>Default value used for 3GPP performance test setup and signalling tests. |
| PBCH EPRE Ratio | PBCH_RA = 0 dB<br>PBCH_RB = 0 dB | PBCH_RA = 0 dB<br>PBCH_RB = 0 dB | Refer to [13], Annex C.2 |
| PSS EPRE Ratio | PSS_RA = 0 dB | PSS_RA = 0 dB | Refer to [13], Annex C.2 |
| SSS EPRE Ratio | SSS_RA = 0 dB | SSS_RA = 0 dB | Refer to [13], Annex C.2 |
| PCFICH EPRE Ratio | PCFICH_RB = 0 dB | PCFICH_RB = 0 dB | Refer to [13], Annex C.2 |
| PDCCH EPRE Ratio | PDCCH_RA = 0 dB<br>PDCCH_RB = 0 dB | PDCCH_RA = 0 dB<br>PDCCH_RB = 0 dB | Refer to [13], Annex C.2 |
| PDSCH EPRE Ratio | PDSCH_RA = 0 dB<br>PDSCH_RB = 0 dB | PDSCH_RA = 0 dB<br>PDSCH_RB = 0 dB | Refer to [13], Annex C.2 |
| PHICH EPRE Ratio | PHICH_RA = 0 dB<br>PHICH_RB = 0 dB | PHICH_RA = 0 dB<br>PHICH_RB = 0 dB | Refer to [13], Annex C.2 |
| RoHC | On | On | 3GPP Profile1 |
| UL TX Power level | 10 dBm | 10 dBm | The Output Power of the DUT as defined in [11]<br>See NOTE below |
| DL Transmission scheme | 2x2 closed loop spatial multiplexing | 2x2 closed loop spatial multiplexing | i.e. uses TX Mode 4 |
| Cyclic Prefix Length | Normal | Normal | No extended cyclic prefix |
| PHICH Duration | Normal | Normal | 1 symbol only, no extended PHICH |
| DCI Aggregation Level | 4 CCEs for DCI0<br>8 CCEs for all other DCI formats | 4 CCEs for DCI0<br>8 CCEs for all other DCI formats | Refer to [13], Annex C.3.1 |
| DRX Configuration | DRX : On | DRX : On |  |
| LongDRX-Cycle | 40 sub-frames | 40 sub-frames | Result must indicate used value |
| onDuration Timer | 4 sub-frames | 4 sub-frames | Result must indicate used value |
| DRX-Inactivity Time | 4 sub-frames | 4 sub-frames | Result must indicate used value |
| Short DRX | Off | Off |  |
| DL and UL Channel Bandwidth | 10 MHz | 10 MHz | This configuration corresponds to 0.6 Mbit/s DL / 0.5 Mbit/s UL for FDD, while 0.35 Mbit/s DL / 0.214 Mbit/s UL for TDD. |
| Uplink downlink configuration | NA | 1 | This configuration corresponds to 0.6 Mbit/s DL / 0.5 Mbit/s UL for FDD, while 0.35 Mbit/s DL / 0.214 Mbit/s UL for TDD. |
| Special subframe configuration | NA | 4 | This configuration corresponds to 0.6 Mbit/s DL / 0.5 Mbit/s UL for FDD, while 0.35 Mbit/s DL / 0.214 Mbit/s UL for TDD. |
| NRB (DL) | 12 | 12 | This configuration corresponds to 0.6 Mbit/s DL / 0.5 Mbit/s UL for FDD, while 0.35 Mbit/s DL / 0.214 Mbit/s UL for TDD. |
| MCS (DL) | 0 | 0 | This configuration corresponds to 0.6 Mbit/s DL / 0.5 Mbit/s UL for FDD, while 0.35 Mbit/s DL / 0.214 Mbit/s UL for TDD. |
| NRB (UL) | 20 | 20 | This configuration corresponds to 0.6 Mbit/s DL / 0.5 Mbit/s UL for FDD, while 0.35 Mbit/s DL / 0.214 Mbit/s UL for TDD. |
| MCS (UL) | 0 | 0 | This configuration corresponds to 0.6 Mbit/s DL / 0.5 Mbit/s UL for FDD, while 0.35 Mbit/s DL / 0.214 Mbit/s UL for TDD. |
| PDCCH length | 2 symbols | 2 symbols | This configuration corresponds to 0.6 Mbit/s DL / 0.5 Mbit/s UL for FDD, while 0.35 Mbit/s DL / 0.214 Mbit/s UL for TDD. |
| OCNG | According to Table E-UTRA_FDD_Idle_1 | According to Table_E-UTRA_TDD_Idle_1 | 3GPP [13], Annex A.5.1.2 |
