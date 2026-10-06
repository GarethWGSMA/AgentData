---
source: "TS.22_v6.0.docx"
chunk_id: 020
section_path:
  - "4.1 Connection Management Client"
---

## 4.1 Connection Management Client

Connection management clients interface between several layers providing an intuitive means of managing connectivity, preferences and networks. The implementation will vary per operating system and manufacturer but most of the work of the client should be to use API calls rather than issuing low level calls itself. This will make the build of clients easier and more uniform throughout devices and operating systems.

Connection management clients are in charge of managing all connections. In the context of this document, the connection management client, or application manages different WLAN access network connections based on a device status, connection conditions, operator policies and user profiles associated with these connections.

The following are examples of connection management APIs that a device could implement to improve WLAN management:

- Turn on and turn off the WLAN (including support of flight mode, where flight mode means that a device has the functionality to turn off wireless modules in case the transmitting and receiving of the wireless signals impacts the safety of aircraft flight.)
- Query if WLAN functionality is on or off
- Interact with the connection manager to connect to and disconnect from APs
- Use the operator predefined list of preferred network identifiers (e.g. SSID)
- Add, delete, modify and manage WLAN profiles, including information such as network identifiers (e.g. SSID), secured or open network, discover security methods and authentication credentials.
- Access to detailed information per network identifier, such as the WLAN signal strength per network identifier (e.g. SSID – active or inactive), WLAN channel physical rate, backhaul capability (if available), security methods and authentication credentials used, known or unknown network)
- Access to the list of available network identifiers (e.g. SSID)
- Support automatic & manual connection modes
- Force the association to a specific network identifier (e.g. SSID), visible or not.
- Listen to the WLAN events such as new available network, loss of network, successful association on a specific network identifier (e.g. SSID).
- Access to information on an active session using a specific network identifier (e.g. a SSID) such as IP address, MAC Address, Subnet Address
- Modify information on WLAN connection such as IP address, Subnet Address

| Req ID | Requirement |
| --- | --- |
| TSG22_R2_CM_05 | A device SHALL have at least one pre-installed connection management client. |
| TSG22_R2_CM_06 | A device SHOULD have programming interfaces/APIs to control and/or manage WLAN connections. |
| TSG22_R2_CM_07 | VOID |
| TSG22_R2_CM_08 | A device SHOULD offer an API compliant with the OMA [OpenCMAPI] for WLAN management. |
| TSG22_R3_CM_46 | The connection manager SHALL provide an API to turn on and turn off the WLAN including support of flight mode, where flight mode means that a device SHALL have the functionality to turn off wireless modules. |
| TSG22_R5_CM_63 | A device SHOULD prefer a 5 GHz connection over a 2.4 GHz connection when both are available for the same specific network identifier. |
