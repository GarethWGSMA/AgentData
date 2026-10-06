---
source: "TS.09_v13.docx"
chunk_id: 031
section_path:
  - "2.7.1 WLAN Standby Parameters"
---

## 2.7.1 WLAN Standby Parameters

This section is applicable for a DUT with WLAN capabilities. WLAN parameters of the test Access Point (AP) are described below:

| Parameter | Mandatory Value | Comment |
| --- | --- | --- |
| WLAN Standards | IEEE 802.11b/g/a/n |  |
| WLAN Frequency<br>(2.4 GHz) | 7 |  |
| WLAN Frequency<br>(5 GHz) | 36 | DUTs that support the 2.4 GHz and the 5 GHz band be tested in each band |
| Authentication / Ciphering | WPA2 |  |
| DTIM Period | 3 |  |
| WMM/UAPSD Power Save | 1) Both Turned On, and<br>2) Both Turned Off | All WLAN tests in which a WLAN access Point is used shall be run twice with WMM/UAPSD turned On And turned Off. |
| WLAN RSSI | -70 dBm |  |
| Beacon Interval | 100 ms |  |

: Access Point WLAN parameters

WLAN parameters of the DUT are described below: The DUT shall be put in the mode that the user will encounter in the production model. Those values need to be recorded into the Annex B Pro-forma table.

| Parameter | Recommended Values | Comment |
| --- | --- | --- |
| WLAN Standards | IEEE 802.11b/g/A/N | Used value shall be reported with the test results |
| Long Retry Limit | 4 | Used value shall be reported with the test results |
| Short Retry Limit | 7 | Used value shall be reported with the test results |
| RTS Threshold | 2346 | Used value shall be reported with the test results |
| Tx Power Level | 100 mW | Used value shall be reported with the test results |
| WLAN Network Scan Period | Every 5 Minutes | Used value shall be reported with the test results |

: DUT WLAN parameters
