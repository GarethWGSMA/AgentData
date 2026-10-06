---
source: "TS.26_v15.1.docx"
chunk_id: 030
section_path:
  - "6.3.3.1.2 AID Conflict Resolution"
---

## 6.3.3.1.2 AID Conflict Resolution

| TS26_NFC_REQ_068 | The device SHALL provide a mechanism to handle AID Conflict. |
| --- | --- |
| TS26_NFC_REQ_068.01 | AID Conflict resolution SHOULD follow the same mechanisms whether NFC services registration is dynamic or static. |
| TS26_NFC_REQ_068.02 | When managing AID conflict resolution, the device SHALL follow the end-user preferences.<br>Note: In case of a Basic Device, end-user preference may have been set via a paired device or from a connected PC. The way this is achieved is out of scope of this document. |
| TS26_NFC_REQ_068.03 | For non Basic Devices, when AID conflict resolution implies user choice at transaction time the user SHOULD be able to make their decision persistent, until the terms of the AID conflict change (another application is installed or removed, which claims the same AID), or the user goes into the menus to revisit their decision.<br>Note: For Basic Devices the end-user is not able to make such choice at transaction time. It is the responsibility of the device manufacturer to implement mechanisms that will detect such conflict at installation time and ask for end-user preferences. |
