---
source: "TS.26_v15.1.docx"
chunk_id: 035
section_path:
  - "6.6.1 NFC Event & Access Control requirements"
---

## 6.6.1 NFC Event & Access Control requirements

“EVT_TRANSACTION” messages are sensitive data. Intercepting these events might help a malicious application to lure a user into entering sensitive information into a fake UI.

The NFC stack shall therefore implement GlobalPlatform Secure Element Access Control specification to check that the recipient activity has been signed with an authorised certificate. This check is performed at the time the event is being forwarded from the lower layers to the target application using, when already populated, the cached SEAC rules for performance reasons. If no application is authorised as per “Access Control” check, then the event is discarded.

| TS26_NFC_REQ_084 | The OS implementation SHALL support the use of the GlobalPlatform Secure Element Access Control enforcer to manage Transaction Events originating from a Secure Element and SHALL ensure that this event is made available only to authorised OS applications. |
| --- | --- |
| TS26_NFC_REQ_084.1 | The OS SHALL re-use the caching mechanism as described in TS26_NFC_REQ_122<br><br>Note: As per TS26_NFC_REQ_121 Refresh tag is not used in this scenario as no open logical channel is performed by the Transaction Event itself. |
| TS26_NFC_REQ_085 | The device SHALL prevent the case that an application UI is triggered from an applet when the access conditions would not allow the application UI to exchange APDUs with this applet and there is no rule explicitly granting the NFC event permission. |
