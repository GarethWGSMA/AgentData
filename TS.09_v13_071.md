---
source: "TS.09_v13.docx"
chunk_id: 071
section_path:
  - "5.3.3 Power Consumption during Power Saving Mode"
---

## 5.3.3 Power Consumption during Power Saving Mode

To measure the average current when DUT is in power saving mode.

Initial configuration

DUT is in idle mode.

DUT is in a test location with good network coverage

DUT is equipped with dummy battery and connected to the power consumption tester via power line

Test procedure

Set the output voltage of power consumption tester the same as DUT nominal voltage
Switch on power consumption tester.
DUT enters into power saving mode. Start power consumption measurement. Measure the average current over a continuous min{5 minute, T3412} period while DUT is in power saving mode.
Stop power consumption measurement.
Record the voltage (V) and average current (IPSM) in step 3.
