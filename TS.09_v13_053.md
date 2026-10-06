---
source: "TS.09_v13.docx"
chunk_id: 053
section_path:
  - "3.4.2 Battery Current Drain"
---

## 3.4.2 Battery Current Drain

The following procedure shall be used to measure the average current drain of the DUT:

- The DUT battery is replaced with the “dummy battery” circuit described in section 3.2.1.
- The dummy battery is connected to a combined DC power source and current measurement device capable of meeting the minimum measurement requirements specified in section 3.2.2.
- The DC power source is configured to maintain a voltage equal to the Nominal Battery Voltage across the dummy battery terminals. Determination of the Nominal Battery Voltage is described in section 4.2.
- Activate the DUT
- Wait three minutes after activation for DUT boot processes to be completed. Place the terminal into the appropriate test configuration and wait for 30 s.
- While the terminal is still in the test configuration record the current samples
- Over a continuous 10 minutes period for connected mode operations.
- (For testing an application use the times specified in the preceding section)
- Calculate the average current drain (In dedicated) from the measured samples.
- If appropriate to the test, record the volume of data transferred in the thirty minute period.
- Calculate the battery life as indicated in the following section.
