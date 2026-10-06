---
source: "TS.22_v6.0.docx"
chunk_id: 023
section_path:
  - "4.4 Intermittent WLAN Connectivity"
---

## 4.4 Intermittent WLAN Connectivity

Users would like to be connected to the best available resource as much as possible with minimum interruption to usability.

Maximising available resources such as switching to higher bandwidth WLAN presents an attractive alternative to users. However, minimum interruption should be ensured. Automatically switching from WLAN access to another WLAN or to 3GPP access (2G/3G/LTE) may present usability problems to a device if it is not properly configured to handle such scenarios.

Hysteresis (meaning that the threshold to switch to WLAN access is different from the threshold to switch away from that access) mechanisms should be implemented with tuned radio thresholds, so that a device which is experiencing signal strength or throughput degradation from its serving AP can determine when to switch to another AP or to 3GPP access.

The device should have a defined access threshold at which it will release its connection to the serving AP, even if there is no other WLAN or 3GPP access network available.

In some cases, WLAN access could be temporarily denied from the network for technical or marketing reasons, without displaying any message to the customer. A device in this situation should avoid network overload by too many successive request attempts.

| Req ID | Requirement |
| --- | --- |
| TSG22_R2_CM_19 | A device SHALL have a hysteresis mechanism to prevent disconnect followed by connection or re-connection in a minimal interval with no improvement in connection conditions. |
| TSG22_R2_CM_20 | A device SHALL limit the number of access retries to the same AP when it receives temporary denied access notification from that AP, according to a limit which may be defined by an operator.<br>(e.g. 1026 notification with EAP-SIM in RFC 4186 [RFC 4186]) |
