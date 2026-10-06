---
source: "TS.09_v13.docx"
chunk_id: 050
section_path:
  - "3.3.2 Battery Current Drain"
---

## 3.3.2 Battery Current Drain

The following procedure shall be used to measure the average current drain of the DUT:

1. The DUT battery is replaced with the “dummy battery” circuit described in section 3.2.1.
1. The dummy battery is connected to a combined DC power source and current measurement device capable of meeting the minimum measurement requirements specified in section 3.2.2.
1. The DC power source is configured to maintain a voltage equal to the Nominal Battery Voltage across the dummy battery terminals. Determination of the Nominal Battery Voltage is described in section 4.2.
1. Activate the DUT
1. Wait 3 minutes after activation for DUT boot processes to be completed.
1. In idle mode, record the current samples over a continuous 30 minute period.
1. Calculate the average current drain (Iidle) from the measured samples.
1. Calculate the battery life as indicated in the following section.

NOTE:	It is important that a controlled RF environment is presented to the DUT and it is recommended this is done using a RF shielded enclosure. This is necessary because the idle mode BA (BCCH) contains a number of ARFCNs. If the DUT detects RF power at these frequencies, it may attempt synchronisation to the carrier, which will increase power consumption. Shielding the DUT will minimise the probability of this occurring, but potential leakage paths through the BSS simulator should not be ignored.
