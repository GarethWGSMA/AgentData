---
source: "TS.09_v13.docx"
chunk_id: 055
section_path:
  - "3.5.2 Battery Current Drain"
---

## 3.5.2 Battery Current Drain

The following procedure shall be used to measure the average current drain of the DUT:

- Fully charge the battery on the DUT, with the DUT deactivated, following the manufacturer charging instructions stated in the user manual, using the manufacturer charger.
- Remove the battery from the DUT.
- Re-connect the battery with the measurement circuitry described in section 4 in series with the battery (positive terminal).
- Activate the DUT.
- After activation wait for DUT boot processes to be completed. Place the terminal into the appropriate test configuration and wait for 3 more minutes to be sure that all initialization processes has been completed. (Boot processes refer to events which occur only once per power cycle)
- In idle mode, record the current samples over a continuous 30 minute period.
- Calculate the average current drain (Idle) from the measured samples.
- Calculate the battery life as indicated in the following section.
