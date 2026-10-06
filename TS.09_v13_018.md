---
source: "TS.09_v13.docx"
chunk_id: 018
section_path:
  - "2.4.3 WCDMA PS Data Transfer Parameters"
---

## 2.4.3 WCDMA PS Data Transfer Parameters

The WCDMA bearer configuration of the tests is described below. Some bearer parameters shall be selected among some recommended values. These parameters and the selected value shall be reported with the tests results. The configuration is based on a Category 8 UE or higher.

| Parameters | Value | Comment |
| --- | --- | --- |
| Serving Cell UARFCN (Downlink) | Band I: Mid Range<br>Band II: Mid Range<br>Band IV: Mid Range<br>Band V: Mid Range<br>Band VI: Mid Range<br>Band VIII: Mid Range<br>Band IX: Mid Range | In test results |
| Serving Cell UARFCN (Uplink) | Band I: Mid Range<br>Band II: Mid Range<br>Band IV: Mid Range<br>Band V: Mid Range<br>Band VI: Mid Range<br>Band VIII: Mid Range<br>Band IX: Mid Range | In test results |
| Serving Cell Scrambling Code | 255 | In test results |
| Number Of neighbours Declared In The BA_LIST | 16 | See NOTE below |
| Use Secondary Scrambling Code | No | In test results |
| Fixed Channelization Code | Yes | In test results |
| Hard Handover | No | In test results |
| Soft / Softer Handover | No | In test results |
| Channel Type – UL & DL / Bearer | Interactive Or Background / Hspa In Both Uplink And Downlink |  |
| Uplink tti | 2 ms |  |
| Nominal Avg. UL Inf. Bit Rate | 0 KBPS |  |
| Ack-Nack Repetition Factor | 3 | Required for continuous HS-DPCCH signal |
| CQI Feedback Cycle, k | 4 ms |  |
| CQI Repetition Factor | 2 | Required for continuous HS-DPCCH signal) |
| Beta_C | 15/15 |  |
| ∆ACK, ∆NACK and ∆CQI | 5/15 | beta_hs/Beta_C=5/15 |
| Beta_EC | 5/15 |  |
| AG Index | 12 | This sets the Beta_ED=47/15 |
| Nominal Avg. Inf. Bit Rate | 7200 kbps |  |
| Inter-TTI Distance | 1 tti’s |  |
| Number Of harq Processes | 6 processes |  |
| Information Bit Payload () | 14411 bits |  |
| Binary Channel Bits per TTi | 15360 bits |  |
| Total Available smls In ue | 134400 smls |  |
| Number Of smls Per harq Proc. | 22400 smls |  |
| Coding Rate | 0.94 |  |
| Number Of Physical Channel Codes | 10 Codes |  |
| Modulation | 16qam |  |
| Ioc | -60 dB |  |
|  | 10 dB |  |
| CPICH_Ec/Ior | -10 dB |  |
| P-CCPCH_Ec/Ior | -12 dB |  |
| SCH ec/ior | -12 dB |  |
| DPCH_Ec/Ior | -10 dB |  |
| E-agch ec/ior | -30 dB |  |
| e-hich | -20 dB |  |
| hs-scch-1 | -13 dB |  |
| hs-scch-2 | -20 dB |  |
| hs-pdsch | -1.80 dB |  |
| Duty Cycle | 100% | In test results |
| Terminal Tx Level | 1) Fixed Value Of 10 dBm, And<br>2) Power Distribution As Defined In Circuit Switched Section Above. |  |
| T1: DCH to FACH When No Data Is Transferred | 10 s | In test results |
| T2: FACH to IDLE When No Data Is Transferred | 5 s | In test results |

: WCDMA parameters for Packet Switched Transfer

Note:	Although the UE is required to monitor these neighbour cells, the test equipment does not in fact provide signals. No signals should be present on the neighbour frequencies. If signals are present then the terminal will attempt to synchronise and this is not part of the test. The number of neighbours is the number of intra-frequency neighbours. No GSM neighbour cell is declared in the Inter-RAT neighbour list for WCDMA Standby test.

Where transfer is band specific, the band measured must be specified.
