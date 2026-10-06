---
source: "TS.22_v6.0.docx"
chunk_id: 037
section_path:
  - "7.2 Status Information"
---

## 7.2 Status Information

For better user experience, pertinent device status information should be provided to the user using a consolidated or convenient interface such as icons and or status notifications.

Status information, such as network coverage, signal level and battery strength, byte counter, connection manager, network identity, encryption status, shall be provided through an application or operating system information. Additional information from Passpoint can also be provided, such as WLAN link status, WLAN uplink and downlink data rates. WLAN access network name or logo should be displayed when connected to Passpoint APs.

Status about authentication success and failure may also be indicated on a device. If the WLAN connection is insecure, a notification message should be displayed to the user when a device associates with an AP for the first time.

If the WLAN connection is secure (i.e. AP is Passpoint certified or supports WPA2-Enterprise and EAP authentication over IEEE 802.1X), an icon indicating a secure connection should be visible to the user (e.g. padlock layered on WLAN signal strength icon). If the WLAN connection is insecure, a notification message should be displayed to the user when a device associates with the AP for the first time.

| Req ID | Requirement |
| --- | --- |
| TSG22_R2_USE_04 | A device that has a UI SHALL indicate the status of the device connection. |
| TSG22_R2_USE_05 | A device SHOULD offer programming interfaces providing Status Information to applications. |
| TSG22_R2_USE_06 | A device SHOULD offer an API compliant with the OMA [OpenCMAPI] for Status Information & notifications functions. |
| TSG22_R2_USE_07 | Link status information from a Passpoint AP MAY be used to improve link status information presented to the user or applications. |
