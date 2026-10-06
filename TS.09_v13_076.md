---
source: "TS.09_v13.docx"
chunk_id: 076
section_path:
  - "7.3.1 Power Consumption of Data Transfer Event during Active Mode"
---

## 7.3.1 Power Consumption of Data Transfer Event during Active Mode

Description

To measure the average current of a data transfer event for DUT in active mode, e.g. status reporting.

Initial configuration

DUT is powered off

DUT is in a test location with good network coverage

DUT is equipped with dummy battery and connected to the power consumption tester via power line

Test procedure

1. Set the output voltage of power consumption tester the same as DUT nominal voltage
1. Switch on power consumption tester and power on the DUT.
1. Trigger a data transfer event on DUT when DUT enters into idle mode.
1. Start power consumption measurement. Measure and record the average current and time during this data transfer event.
1. Stop power consumption measurement after the DUT completes the data transfer and enters into idle mode again.
1. Repeat step 3-5 twice more. Get the average current and test duration of three times.
1. Record the voltage (V), average current (IDTE) and time (TDTE) (in seconds).
