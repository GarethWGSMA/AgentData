---
source: "TS.09_v13.docx"
chunk_id: 016
section_path:
  - "2.4.1 WCDMA Standby Parameters"
---

## 2.4.1 WCDMA Standby Parameters

The WCDMA bearer configuration of the tests is described below. Some bearer parameters shall be selected among some recommended values. These parameters and the selected value shall be reported with the tests results. Parameters apply to all scenarios run in standby mode unless otherwise specified.

| Parameter | Recommended Value | Comment |
| --- | --- | --- |
| Serving Cell UARFCN (Downlink) | Band I: Mid Range<br>Band II: Mid Range<br>Band IV: Mid Range<br>Band V: Mid Range<br>Band VI: Mid Range<br>Band VIII: Mid Range<br>Band IX: Mid Range | All bands supported by the DUT must be measured.<br>Results must indicate which band(s) have been measured, and individual result for each band |
| Number of neighbours declared in the BA_List | 16 | See NOTE below |
| Neighbour Cells on different frequency | No |  |
| Serving Cell Scrambling Code | Any | Used value shall be reported with the test results |
| Neighbour Cell Scrambling Codes | Any | See note. Used values shall be reported with the test results |
| Paging Interval | 1.28 s (DRX 7) | This value must be used unless operator requests 2.56 S (DRX 8). |
| Periodic Location Updates | No | T3212 = 0 |
| Number of Paging Indicators per frame | 18 |  |
| Ioc | -60 dBm | Refer to [9] Section 7.1.1 |
|  | -1 dB | Refer to [9] Section 7.1.1 |
| CPICH_Ec/Ior | -3.3 dB | Refer to [9] Annex E.2. |
| PICH_Ec/Ior | -8.3 dB | Refer to [9] Annex E.2. |
| SIntrasearch | Sintrasearch = 12 dB |  |
| Sintersearch | = 10 dB |  |
| Qqualmin | = -20 dB |  |
| Qrxlevlmin | = -113 dBm |  |
| SsearchRAT | SsearchRAT = 4 dB |  |

: WCDMA parameters for Standby Time

NOTE:	Although the DUT is required to monitor these neighbour cells, the test equipment does not provide signals. Signals should not be present on the neighbour frequencies. If signals are present then the DUT will attempt to synchronise and this is not part of the test. The number of neighbours are the number of intra-frequency neighbours. No GSM neighbour cell is declared in the Inter-RAT neighbour list for WCDMA Standby test.
