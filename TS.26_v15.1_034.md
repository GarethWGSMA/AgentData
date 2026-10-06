---
source: "TS.26_v15.1.docx"
chunk_id: 034
section_path:
  - "6.6 Security"
---

## 6.6 Security

Access API & Secure Element Access Control Requirements

The main objective of the Access Control mechanism is to protect communication with the Secure elements.

From this cache, the Access Control can determine if the relationship between the UI application and the SE applet (application signature/AID) is valid, and then authorise a communication or send an exception.

| TS26_NFC_REQ_082 | Open OS devices SHALL provide access control as per GlobalPlatform, Secure Element Access Control specification for each available SE. |
| --- | --- |
| TS26_NFC_REQ_082.1 | The access rules & associate caching mechanism, a.k.a Access Control Enforcer, SHALL be specific to each SE. |
| TS26_NFC_REQ_083 | When no access control data (files or applets) is found on a SE the OS SHALL deny access to this SE. |
| TS26_NFC_REQ_121 | Access Control Enforcer SHALL check if Access Rules has been updated only when a new logical channel is open. All rules SHALL stay valid until the channel is closed. |
| TS26_NFC_REQ_122 | Access Control Enforcer SHALL cache the rules from the Secure Element<br>(ARF mechanism or ARA with GET DATA[ALL]). |
| TS26_NFC_REQ_122.1 | Access Control Enforcer cache SHALL be rebuilt when the device is switched on or the Secure Element is powered on. |
| TS26_NFC_REQ_122.2 | When the Access Control Enforcer checks if the Access Rules have been updated, the cache SHALL only be refreshed if the “Refresh Tag” is updated. |
| TS26_NFC_REQ_163 | The device SHALL not log any APDU or AID exchanged in a communication with an applet located in an SE (UICC, eSE, …). |
| TS26_NFC_REQ_169 | The Access Control Enforcer SHALL be able to parse rules with unknown or missing tags. |
| TS26_NFC_REQ_169.1 | The Access Control Enforcer SHALL ignore rules with unknown or missing tags and SHALL process the rest of the ruleset. |
