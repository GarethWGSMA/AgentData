---
source: "TS.09_v13.docx"
chunk_id: 013
section_path:
  - "2.3.1 GSM Standby Parameters"
---

## 2.3.1 GSM Standby Parameters

The GSM configuration of the tests are described below. Some bearer parameters shall be selected among some recommended values. These parameters and the selected value shall be reported with the tests results.

| Parameter | Value | Comment |
| --- | --- | --- |
| BCCH | ARFCN :<br>189 for 850 MHz<br>62 for 900 MHz<br>698 for 1800 MHz<br>660 for 1900 MHz | All values are chosen to be mid band.<br>All bands supported by the DUT must be measured.<br>Results must indicate which band(s) have been measured, and individual result for each band. |
| Rx Level | -82 dBm |  |
| Paging Interval | 5 Multi Frames |  |
| No of Neighbour Cells declared in the BA_List | 16 frequencies as defined in Annex A |  |
| Periodic Location Updates | No | T3212 = 0 |

: GSM parameters for Standby Time

NOTE: 	Although the DUT is required to monitor these neighbour cells, the test equipment does not provide signals on these frequencies. No signals should be present on the neighbour frequencies. If signals are present then the DUT will attempt to synchronise to the best 6 neighbour frequencies, and this is not part of the test.
