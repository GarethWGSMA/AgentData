---
source: "TS.09_v13.docx"
chunk_id: 045
section_path:
  - "3.2.1 Dummy Battery Fixture"
---

## 3.2.1 Dummy Battery Fixture

The dummy battery fixture is a device designed to replace the usual battery pack to facilitate powering the DUT from an external DC source and simulating “normal” indications to any active battery management functions within the DUT.

The dummy battery may consist of a battery pack where the connections to the internal cells have been broken and connections instead made to the DC source. Alternatively, it may consist of a fabricated part with similar dimensions and connections to a battery pack and containing or simulating any required active battery management components.

The dummy battery should provide a connection between the battery terminals of the DUT and the DC power source whilst minimising, as far as possible, the resistance, inductance and length of cables required.

Separate “source and sense” conductors may be used to accurately maintain the nominal battery voltage as close to the DUT terminals as possible.

It may be necessary to include some capacitance across the DUT terminals to counteract the effects of cable inductance on the DUT terminal voltage when the DUT draws transient bursts of current. Such capacitance should be kept to a minimum, bearing in mind that it will affect the temporal resolution of the current sampling.
