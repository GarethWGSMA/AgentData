---
source: "TS.26_v15.1.docx"
chunk_id: 059
section_path:
  - "7.6.2 NFC Event & Access Control requirements"
---

## 7.6.2 NFC Event & Access Control requirements

The same generic requirements are applicable to Android platform with the following requested implementation:

Android permissions

| TS26_NFC_REQ_131 | VOID |
| --- | --- |

:VOID

| TS26_NFC_REQ_191 | The device SHALL ensure that the application has the following permission before forwarding a Transaction event to the application: |
| --- | --- |

| Transaction Event | android.permission.NFC_TRANSACTION_EVENT |
| --- | --- |

: Table EVT_TRANSACTION Permissions

Access control

Transaction intents link an Android application and an applet installed on a Secure Element. For this reason, securing them shall be done with the same rules that restrict applet access by the Android application through the GlobalPlatform Open Mobile API.

| TS26_NFC_REQ_152 | The NFC stack SHALL therefore use internal “Access Control” API to check that the recipient activity has been signed with an authorised certificate. This check is performed at the time the event is being forwarded from the lower layers to the target application. See TS26_NFC_REQ_084.1 |
| --- | --- |
| TS26_NFC_REQ_152.1 | If an application is registered to any “EVT_TRANSACTION”, by omitting the AID in the Intent, it SHALL receive the events of any applets to those accessible using the “Access Control”. |
| TS26_NFC_REQ_152.2 | If no application is authorised as per “Access Control” check, then the event SHALL be discarded by the framework. |
