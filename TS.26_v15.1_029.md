---
source: "TS.26_v15.1.docx"
chunk_id: 029
section_path:
  - "6.2.2 Card Emulation Mode Requirements"
---

## 6.2.2 Card Emulation Mode Requirements

| TS26_NFC_REQ_095 | The device SHALL support routing to active CEEs. |
| --- | --- |
| TS26_NFC_REQ_118.1 | At first power up or factory reset the device SHALL set the route for NFCA and NFCB technologies (as defined in NFC Forum specification) to the UICC. |
| TS26_NFC_REQ_118.2 | At first power up or factory reset the device SHALL set the route for ISO_DEP protocol (as defined in NFC Forum specification) to the UICC. |
| TS26_NFC_REQ_118.3 | At first power up or factory reset the device SHOULD set the Default AID route to the UICC. |
| TS26_NFC_REQ_162 | When a NFC Reader explicitly selects a NFC Service by its AID but the AID is not defined in the NFC Controller’s routing table, the NFC Controller SHALL route the transaction to the Card Emulation Environment identified as Default AID route. |
| TS26_NFC_REQ_162.1 | The default AID route SHALL be independent of any other routes configured in the NFC controller (such as those for RF Protocol (for example: ISO_DEP, T2T, T3T, T4T, T5T) or RF Technology (for example: NFC_A, NFC_B, NFC_F, NFC_V)). |
| TS26_NFC_REQ_119 | VOID |
| TS26_NFC_REQ_063 | When a NFC application is uninstalled, the device SHALL remove all information related to this application from the routing table. |
| TS26_NFC_REQ_063.1 | When a NFC application is disabled, the device SHALL remove all information related to this application from the NFC routing table.<br><br>Note: this also applies for preinstalled applications that cannot be uninstalled but that can only be disabled. |
| TS26_NFC_REQ_064 | When a NFC application is updated or re-enabled, the device SHALL update the routing table according to the new registration information (removing/adding elements).<br><br>Note: Static elements from the previous version will be removed and static elements from the new version will be added. |
| TS26_NFC_REQ_143 | When the device needs to update the routing table because of new AID registration; AND<br>there is not enough space in the routing table for all required AIDs while maintaining the current default route; AND<br>there would be enough space in the routing table for all required AIDs if the default AID route was changed to one of the other card emulation environments,<br>THEN the device SHALL change the default AID route automatically to one of those other card emulation environments and SHALL update the routing table accordingly.<br>In such situation, there SHALL be no user interaction at all.<br>Note: This mechanism needs to be totally transparent for end users as this is a solution resolving the chipset routing table size shortage. |
| TS26_NFC_REQ_065 | The device SHALL provide a routing mechanism using the following priority: AID, then default AID route, then RF protocol and then RF technology. |
| TS26_NFC_REQ_065.1 | When the device is powered off and a NFC reader is trying to select by AID a NFC service relying on the HCE technology, the NFC Controller SHALL return an ISO error code (‘6A82’) indicating this service is not available. |
| TS26_NFC_REQ_066 | VOID |
| TS26_NFC_REQ_067 | When manual mechanism is used to register the new NFC service, the device SHOULD provide high level information to the user (i.e. NFC service name and not AID, etc.). |
