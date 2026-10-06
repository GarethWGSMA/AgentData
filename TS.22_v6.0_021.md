---
source: "TS.22_v6.0.docx"
chunk_id: 021
section_path:
  - "4.2 Network Discovery"
---

## 4.2 Network Discovery

Constant scanning for detection of a hotspot may place a heavy toll on the battery life of a Smartphone. A device should implement periodic scanning algorithms that preserve battery life. The scanning algorithm should take into account Passpoint network discovery.

| Req ID | Requirement |
| --- | --- |
| TSG22_R2_CM_10 | A device SHALL be able to provide detailed information per network identifier discovered (such as signal strength, security methods, type of authentication credentials used, known or unknown network) to the user and/or application. |
| TSG22_R2_CM_11 | A device SHALL support a WLAN access network discovery mechanism. |
| TSG22_R2_CM_12 | A device SHOULD be able to listen & report events to an upper layer (e.g. UI) such as new available network, loss of network. |
| TSG22_R3_CM_47 | A device’s WLAN access network discovery mechanism SHALL preserve battery life. |
