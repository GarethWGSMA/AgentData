---
source: "TS.26_v15.1.docx"
chunk_id: 028
section_path:
  - "6.3.3.1.1 NFC Controller Management API"
---

## 6.3.3.1.1 NFC Controller Management API

| TS26_NFC_REQ_055 | The device SHALL support an API that allows applications to dynamically register and un-register NFC application by list of AIDs. |
| --- | --- |
| TS26_NFC_REQ_055.1 | All the AIDs registered dynamically SHALL stay persistent (still available after a power off/on of the device). |
| TS26_NFC_REQ_056 | VOID |
| TS26_NFC_REQ_057 | The device SHOULD support an API that allows applications to dynamically register and un-register NFC application by pattern (e.g. DESFIRE). |
| TS26_NFC_REQ_058 | An API SHALL be offered by the OS to provide a way for the applications to specify which card emulation environment their AIDs are to be routed to.<br>Note: To allow applications to register AIDs belonging to UICC CEE and/or eSE CEE |
| TS26_NFC_REQ_059 | VOID |
| TS26_NFC_REQ_060 | VOID |
| TS26_NFC_REQ_061 | The device MAY support an OS mechanism that allows applications to statically register NFC application by list of AIDs. |
| TS26_NFC_REQ_062 | The device SHOULD support an OS mechanism that allows applications to statically register NFC application by pattern (e.g. DESFIRE). |
| TS26_NFC_REQ_168 | The device SHALL support an OS mechanism for the registration of prefix AIDs and offer a way for applications to use it. |
| TS26_NFC_REQ_168.1 | The device SHALL only allow prefixes longer than or equal to 5 bytes and less than 16 bytes.<br>In the case of an AID registered matching a prefix also registered, the rule is to route according to the longest match. |
