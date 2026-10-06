---
source: "TS.09_v13.docx"
chunk_id: 070
section_path:
  - "5.3.2 Power Consumption during Idle Mode"
---

## 5.3.2 Power Consumption during Idle Mode

Description

To measure the average current when DUT is in standby mode.

Initial configuration

DUT is powered off

DUT is in a test location with good network coverage

DUT is equipped with dummy battery and connected to the power consumption tester via power line

Test procedure

1. Set the output voltage of power consumption tester the same as DUT nominal voltage
1. Switch on power consumption tester and power on the DUT.
1. Start power consumption measurement when DUT completes registration on the IoT service platform and enters into standby mode. Measure the average current for 5 minutes while DUT is in standby mode. Record the test results
1. Stop power consumption measurement.
1. Record the voltage (V) and average current (IIdle) in step 3.
