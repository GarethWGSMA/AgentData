---
source: "TS.09_v13.docx"
chunk_id: 056
section_path:
  - "3.5.3 Measurement Circuitry"
---

## 3.5.3 Measurement Circuitry

Sampled measurements of the voltage across the sense resistor shall be performed. The following measurement equipment is recommended. Equipment of equivalent performance can be used but this must be indicated in the test results.

| Parameter | Idle Mode Setting |
| --- | --- |
| Measurement Resistance | 0.5 ohms |
| Tolerance/Type | 1%, 0.5W, High Precision Metal Film Resistor |
| Sampling Frequency | 50 ksps |
| Resolution | 0.1mA over the full dynamic range of DUT currents. |
| Noise Floor | Less than lowest ADC step |

: Measurement circuitry for Standby Time

NOTE:	It is important that a controlled RF environment is presented to the DUT and it is recommended this is done using a RF shielded enclosure. This is necessary because the idle mode BA (BCCH) contains a number of ARFCNs. If the DUT detects RF power at these frequencies, it may attempt synchronisation to the carrier, which will increase power consumption. Shielding the DUT will minimise the probability of this occurring, but potential leakage paths through the BSS simulator should not be ignored.

- Good engineering practice should be applied to the measurement of current drawn.
- A low value of series resistance is used for sensing the current drawn from the battery.
- Its value needs to be accurately measured between the points at which the voltage across it is to be measured, with due consideration for the resistance of any connecting cables.
- Any constraints on the measurement of the voltage (e.g. due to test equipment grounding arrangements) should be reflected in the physical positioning of the resistance in the supply circuit.
- Voltages drop between battery and DUT in the measurement circuit shall also be considered as this may affect DUT performances”.
- It is also important that leakage into the measurement circuitry does not affect the results.
