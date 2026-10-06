---
source: "TS.09_v13.docx"
chunk_id: 073
section_path:
  - "6.2 Talk Time Scenarios"
---

## 6.2 Talk Time Scenarios

| Test Case Title | Configuration | Testprocedures | Testprocedures |
| --- | --- | --- | --- |
| Test Case Title | Configuration | Power Supply | Battery Pack |
| 6.1.1	GSM | Section 2.3.3 | Section 3.3 | Section 3.5 |
| 6.1.2	WCDMA | Section 2.4.2 | Section 3.3 | Section 3.5 |
| 6.1.3	VoWiFi (no Cellular Coverage) | Section 2.7.2,<br>2.7.3 and 2.7.4 | Section 3.3 | Section 3.5 |
| 6.1.4	VoLTE | Section 2.6.2 | Section 3.3 | Section 3.5 |
| 6.1.5	VoNR (tbd) | tbd | tbd | tbd |

Description

The purpose of this test is to measure the talk time of the DUT when attached to the access technologies listed in the table above.

Default Codec for VoWiFi and VoLTE is AMR-WB. If the EVS codec is supported, then the EVS AMR-WB IO mode may be used as an alternative implementation of AMR-WB

The UE current consumption and thus the talk time during a VoLTE call is expected to depend on the speech activity pattern due to the use of discontinuous transmission (DTX). Therefore a typical voice activity shall be injected during the talk time measurement, including talk, listen and silent periods.

Initial configuration

Common parameters according to section 2.2

Test Method and general description according to 3.1

Measurement preparation according to section 3.2

Standby specific configuration as mentioned in table above

Test procedure

Test procedure according to section as listed in table above
