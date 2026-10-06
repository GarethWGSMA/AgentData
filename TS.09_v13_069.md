---
source: "TS.09_v13.docx"
chunk_id: 069
section_path:
  - "5.3.1 Power Consumption of switching on"
---

## 5.3.1 Power Consumption of switching on

Description

To measure the average current and time taken to switch on the DUT.

Initial configuration

DUT is powered off

DUT is in a test location with good network coverage

DUT is equipped with dummy battery and connected to the power consumption tester via power line

Test procedure

1. Set the output voltage of power consumption tester the same as DUT nominal voltage.
1. Switch on power consumption tester and start power consumption measurement.
1. Power on the DUT. Measure and record the average current and time taken during the registration procedure. The registration procedure starts from switching on DUT and ends at the time when DUT enters into idle mode.
1. Stop power consumption measurement.
1. Switch off the DUT
1. Repeat step 3-5 twice more. Get the average current and test duration of three times.
1. Record the voltage (V), average current (ISwitchOn) and duration (TSwitchOn) (in seconds) of registration.
