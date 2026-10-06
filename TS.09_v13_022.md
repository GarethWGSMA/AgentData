---
source: "TS.09_v13.docx"
chunk_id: 022
section_path:
  - "2.6.1 E-UTRA Standby Parameters"
---

## 2.6.1 E-UTRA Standby Parameters

The E-UTRA bearer configuration of the tests are described below. Some bearer parameters shall be selected among some recommended values. These parameters and the selected value shall be reported with the tests results. Parameters apply to all scenarios run in standby mode unless otherwise specified.

| Parameter | Recommended Value | Recommended Value | Comment |
| --- | --- | --- | --- |
| Parameter | FDD | TDD | Comment |
| Serving Cell Downlink EARFCN | Mid range for all supported E-UTRA bands | Mid range for all supported E-UTRA bands | All bands supported by the DUT must be measured.<br>Results must indicate which band(s) have been measured, and individual result for each band |
| Number of neighbours declared in the neighbour cell list | 16 intra-frequency,<br>0 inter-frequency,<br>0 inter-RAT,<br>no MBSFN cells | 16 intra-frequency,<br>0 inter-frequency,<br>0 inter-RAT,<br>no MBSFN cells | Although the DUT is required to monitor these neighbour cells, the test equipment does not in fact provide signals. |
| DRX Cycle | 1.28 s | 1.28 s | Results must indicate the used DRX cycle. |
| Periodic TAU | No | No | T3412 = 111xxxxx |
| Reference Signal Energy per Resource Element (RS EPRE) | -85 dBm/15kHz | -85 dBm/15kHz | Refer to [13], Annex C.0<br>Default value used for 3GPP performance test setup and signalling tests. |
|  | -98 dBm/15kHz | -98 dBm/15kHz |  |
| Uplink downlink configuration | NA | 1 | Refer to [13], Annex C.2 |
| Special sub-frame configuration | NA | 4 | Refer to [13], Annex C.2 |
| PBCH EPRE Ratio | PBCH_RA = 0 dB<br>PBCH_RB = 0 dB | PBCH_RA = 0 dB<br>PBCH_RB = 0 dB | Refer to [13], Annex C.2 |
| PSS EPRE Ratio | PSS_RA = 0 dB | PSS_RA = 0 dB | Refer to [13], Annex C.2 |
| SSS EPRE Ratio | SSS_RA = 0 dB | SSS_RA = 0 dB | Refer to [13], Annex C.2 |
| PCFICH EPRE Ratio | PCFICH_RB = 0 dB | PCFICH_RB = 0 dB | Refer to [13], Annex C.2 |
| PDCCH EPRE Ratio | PDCCH_RA = 0 dB<br>PDCCH_RB = 0 dB | PDCCH_RA = 0 dB<br>PDCCH_RB = 0 dB | Refer to [13], Annex C.2 |
| PDSCH EPRE Ratio | PDSCH_RA = 0 dB<br>PDSCH_RB = 0 dB | PDSCH_RA = 0 dB<br>PDSCH_RB = 0 dB | Refer to [13], Annex C.2 |
| PHICH EPRE Ratio | PHICH_RA = 0 dB<br>PHICH_RB = 0 dB | PHICH_RA = 0 dB<br>PHICH_RB = 0 dB | Refer to [13], Annex C.2 |
| Serving cell bandwidth | 10 MHz | 10 MHz |  |
| Number of antenna ports at eNodeB | 2 | 2 |  |
| Cyclic Prefix Length | Normal | Normal | No extended cyclic prefix |
| PHICH Duration | Normal | Normal | 1 symbol only, no extended PHICH |
| PDCCH length | 2 symbols | 2 symbols | Refer to [13], Annex C.1 |
| DCI Aggregation Level | 8 CCEs | 8 CCEs | Refer to [13], Annex C.3.1<br>Note that there is no UL in this test so DCI 0 is not relevant |
| Qrxlevmin | -120 dBm | -120 dBm | Lower than the expected RSRP to ensure that the DUT camps on the target cell |
| Qqualmin | -20 dB | -20 dB | Lower than the expected RSRQ to ensure that the DUT camps on the target cell. |
| SintraSearchP | 0 dB | 0 dB | I.e. DUT may choose not to perform intra-frequency measurements.<br>NOTE: In Rel-8 only SIntraSearch is sent. In case Rel-8 is used this shall have the same value as SIntraSearchP in the table. |
| SintraSearchQ | 0 dB | 0 dB | I.e. DUT may choose not to perform intra-frequency measurements.<br>NOTE: In Rel-8 only SIntraSearch is sent. In case Rel-8 is used this shall have the same value as SIntraSearchP in the table. |
| Paging and System Information change notification on PDCCH | No | No | No P-RNTI on PDCCH |
| System Information Reception | No | No | System information will be transmitted, but not received by the DUT during the test. |
| IMS VoPS | supported | supported | EPS Network Feature Support |
| OCNG | According to Table E-UTRA_FDD Idle_1 | According to Table E-UTRA TDD_Idle_1 | [13], Annex A.5.1.2 |

: E-UTRA_Idle_1 Parameters for E-UTRA Standby use case
