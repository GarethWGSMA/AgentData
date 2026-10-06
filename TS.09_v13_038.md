---
source: "TS.09_v13.docx"
chunk_id: 038
section_path:
  - "2.10.1 5G-NR (FR1) Standby Parameters"
---

## 2.10.1 5G-NR (FR1) Standby Parameters

The 5G-NR bearer configuration of the tests are described below. Some bearer parameters shall be selected among some recommended values. These parameters and the selected value shall be reported with the tests results. Parameters apply to all scenarios run in standby mode unless otherwise specified.

| Parameter | Recommended Value | Recommended Value | Recommended Value | Comment |
| --- | --- | --- | --- | --- |
| Parameter | FDD | FDD | TDD | Comment |
| Serving Cell Downlink EARFCN | Mid range for all supported 5G-NR bands | Mid range for all supported 5G-NR bands | Mid range for all supported 5G-NR bands | All bands supported by the DUT must be measured.<br>Results must indicate which band(s) have been measured, and individual result for each band |
| Number of neighbours declared in the neighbour cell list | 16 intra-frequency,<br>0 inter-frequency,<br>0 inter-RAT,<br>no MBSFN cells (in case of EN-DC or DSS) | 16 intra-frequency,<br>0 inter-frequency,<br>0 inter-RAT,<br>no MBSFN cells (in case of EN-DC or DSS) | 16 intra-frequency,<br>0 inter-frequency,<br>0 inter-RAT,<br>no MBSFN cells (in case of EN-DC or DSS) | Although the DUT is required to monitor these neighbour cells, the test equipment does not in fact provide signals. |
| DRX Cycle | 1.28 s | 1.28 s | 1.28 s | Results must indicate the used DRX cycle. |
| Periodic TAU | No | No | No | T3412 = 111xxxxx |
| SubCarrier Spacing (SCS) FR1 | 15 kHz, | 15 kHz, | 30 kHz |  |
| SubCarrier Spacing (SCS) FR2 | 120 kHz | 120 kHz | 120 kHz |  |
| Reference Signal Energy per Resource Element (RS EPRE) | -85 dBm/15kHz | -85 dBm/15kHz | -85 dBm/15kHz | Refer to [20], Annex C.0-<br>Default value used for 3GPP performance test setup and signalling tests. |
|  | -98 dBm/15kHz | -98 dBm/15kHz | -98 dBm/15kHz |  |
| Uplink downlink configuration | NA | NA | 1 | Refer to [20], Annex C.2 |
| Special sub-frame configuration | NA | NA | 4 | Refer to [20], Annex C.2 |
| PBCH | NA | NA | NA | Refer to [20], Annex C.2 |
| SSS | NA | NA | NA | Refer to [20], Annex C.2 |
| PSS | NA | NA | NA | Refer to [20], Annex C.2 |
| PDCCH | NA | NA | NA | Refer to [20], Annex C.2 |
| PDSCH | NA | NA | NA | Refer to [20], Annex C.2 |
| PBCH DMRS | NA | NA | NA | Refer to [20], Annex C.2 |
| PDCCH DMRS | NA | NA | NA | Refer to [20], Annex C.2 |
| PDSCH DMRS | NA | NA | NA | Refer to [20], Annex C.2 |
| CSI-RS | NA | NA | NA | Refer to [20], Annex C.2 |
| Serving cell bandwidth | 10 MHz | 100 MHz | 100 MHz |  |
| Number of antenna ports at gNodeB | 2 - low bands<br>4 - mid bands | 4 | 4 |  |
| Cyclic Prefix Length | Normal | Normal | Normal | No extended cyclic prefix |
| Physical Layer ID (Ncell ID) | 0 | 0 | 0 | 0 = default value |
| PHICH Duration | Normal | Normal | Normal | 1 symbol only, no extended PHICH |
| PDCCH length | 2 symbols | 2 symbols | 2 symbols | Refer to [20], Annex G.1 |
| DCI Aggregation Level | 4 CCEs | 4 CCEs | 4 CCEs | Refer to [20], Annex C.3.1<br>Note that there is no UL in this test so DCI 0 is not relevant |
| Qrxlevmin | -140 dBm | -140 dBm | -140 dBm | Lower than the expected RSRP to ensure that the DUT camps on the target cell |
| Qqualmin | -34 dB | -34 dB | -34 dB | Lower than the expected RSRQ to ensure that the DUT camps on the target cell. |
| SintraSearchP | 0 dB | 0 dB | 0 dB | I.e. DUT may choose not to perform intra-frequency measurements. |
| SintraSearchQ | 0 dB | 0 dB | 0 dB | I.e. DUT may choose not to perform intra-frequency measurements. |
| Paging and System Information change notification on PDCCH | No | No | No | No P-RNTI on PDCCH > no paging |
| System Information Reception | No | No | No | System information will be transmitted, but not received by the DUT during the test. |
| IMS VoPS | Not supported | Not supported | Not supported | EPS Network Feature Support |
| OCNG | According to Table: 5G-NR_FDD_IDLE _1 | According to Table: 5G-NR_FDD_IDLE _1 | According to Table: 5G-NR_TDD_IDLE _1 | Refer to [20], Annex A.5.1.1 (FDD) and A.5.1.2 (TDD) |
