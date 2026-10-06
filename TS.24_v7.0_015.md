---
source: "TS.24_v7.0.docx"
chunk_id: 015
section_path:
  - "2.5 Operator Antenna Performance Acceptance Values for FWA devices"
---

## 2.5 Operator Antenna Performance Acceptance Values for FWA devices

In this section antenna performance acceptance values are defined for products with integrated cellular modules which are mostly used as data access points. These are products like FWA (Fixed Wireless Access) devices, CPEs (Consumer Premises Equipment). In this section, only LTE and 5G NR (FR1 and FR2) frequency bands are considered. This kind of devices are normally not used close to human body like a mobile phone and thus used only for data transfer between device and base station (BS) via cellular network. However, there are different environments possible during operation, such as:

Device mounted on a pole (e.g., an outdoor FWA device)
Device mounted on a wall (e.g., an outdoor router, FWA device)
Device on a desk (e.g., an indoor FWA device)

It’s also important to distinguish between indoor and outdoor use cases.

For indoor use case (e.g. device on a desk) an omnidirectional antenna pattern for the device is recommended since the Angle of Arrival (AoA) is not defined due to multiple arbitrary reflections of the Rx and Tx signals from the walls and obstacles.

Devices can also be installed outdoors by mounting on a pole or a wall. However, in this document DUTs utilizing an external antenna are not considered, because the external antenna is not part of the device and thus it’s designed independently from the device.

For indoor use case it is appropriate to measure TRP and TRS in all spherical directions (3D).

For outdoor use case with integrated directional antennas, it is more appropriate to consider only a part of the space above the horizon (e.g., +/- 30°). For this scenario the CTIA certification near horizon metric could be used. Regardless which material the wall or pole consist of, the CTIA defined near horizon parameters are recommended:

For radiated power:

NHPRP=Near-Horizon Partial Radiated Power

For radiated sensitivity:

NHPIS=Near-Horizon Partial Isotropic Sensitivity

As these devices are not used close to human body, the acceptance values are defined for Free Space (FS) use case.

It is recommended to test device with near horizon metric when device’s antenna is considered as directive one (based on manufacturer declaration estimated antenna gain of more than 6 dBi is considered as directive antenna). Otherwise, device’s antenna is considered as non-directive one and therefore it is recommended to test the device in conventional way (3D).

| Frequency Band LTE | GSMA Operator Acceptance Values for TRP [dBm] for FWA devices | GSMA Operator Acceptance Values for TRP [dBm] for FWA devices |
| --- | --- | --- |
| Frequency Band LTE | Non-Directional integrated antenna - Free Space - 3D | Directional integrated antenna - Free Space – NHPRP+/-30° |
| FDD Band 1 | 19.5 | 17.5 |
| FDD Band 2 | 19.5 | 17.5 |
| FDD Band 3 | 19.5 | 17.5 |
| FDD Band 4 | 19.5 | 17.5 |
| FDD Band 5 | 19.0 | 17.0 |
| FDD Band 7 | 19.5 | 17.5 |
| FDD Band 8 | 19.0 | 17.0 |
| FDD Band 11 | 19.0 | 17.0 |
| FDD Band 12 | 19.0 | 17.0 |
| FDD Band 13 | 19.0 | 17.0 |
| FDD Band 17 | 19.0 | 17.0 |
| FDD Band 18 | 19.0 | 17.0 |
| FDD Band 19 | 19.0 | 17.0 |
| FDD Band 20 | 19.0 | 17.0 |
| FDD Band 21 | 19.0 | 17.0 |
| FDD Band 25 | 19.5 | 17.5 |
| FDD Band 26 | 19.0 | 17.0 |
| FDD Band 28 | 19.0 | 17.0 |
| TDD Band 38 | 19.5 | 17.5 |
| TDD Band 39 | 19.5 | 17.5 |
| TDD Band 40 | 19.5 | 17.5 |
| TDD Band 41 | 19.5 | 17.5 |
| TDD Band 42 | 19.5 | 17.5 |
| TDD Band 43 | 19.5 | 17.5 |
