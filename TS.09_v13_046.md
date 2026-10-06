---
source: "TS.09_v13.docx"
chunk_id: 046
section_path:
  - "3.2.2 Power Source and Current Measurement Device"
---

## 3.2.2 Power Source and Current Measurement Device

This device performs the combined functions of providing, regulated DC power to the DUT and measuring the current consumption of the DUT.

The power source should support the following minimum set of features:

- Configurable output voltage with a resolution of 0.01V or better.
- Output voltage range covering the nominal voltage of the DUT battery with some headroom (=nominal voltage + 5%) to compensate for voltage drop in the supply cables.
- Remote sensing to allow the effects of resistance of the supply cables to be compensated for, and to allow maintenance of the nominal voltage at the DUT battery terminals.
- The DC source should have sufficient output current capability, both continuous and peak, to adequately supply the DUT during all measurements. Current limiting of the power supply shall not function during a measurement.

The following current measurement capability when configured for standby and dedicated mode tests should be met or exceeded:

| Parameter | Idle Mode Requirement | Dedicated Mode Requirement |
| --- | --- | --- |
| Internal Resistance | <= 0.1 ohms* | <= 0.1 ohms* |
| Sampling Frequency | >= 50 ksps | >= 50 ksps |
| Resolution | <= 0.1mA | <= 0.5mA |

: Measurement requirements for Power Supply
