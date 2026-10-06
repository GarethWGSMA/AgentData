---
source: "TS.26_v15.1.docx"
chunk_id: 024
section_path:
  - "6.3.2 Secure Element Access API requirements"
---

## 6.3.2 Secure Element Access API requirements

The SIMalliance group has published the “Open Mobile API” specification until version 3.2. The specification has thereafter moved to GlobalPlatform Device committee. From this document, any mobile device manufacturer will be able to provide a standardised API for access to the different Secure Elements such as the UICC SE. This feature is not specific to NFC and has much broader use cases, it is also used in the context of NFC services.

| TS26_NFC_REQ_047 | OS implementations SHALL provide an API for communicating with all SE inside the device (UICC, eUICC, eSE, …). |
| --- | --- |
| TS26_NFC_REQ_047.1 | Communication with SEs SHALL be done through the logical channels. |
| TS26_NFC_REQ_047.2 | Communication with the Active UICC Profile SHALL prevent access to basic channel (channel 0). |
| TS26_NFC_REQ_047.3 | The API SHALL implement the GlobalPlatform Open Mobile API transport layer or provide an equivalent set of features. |
| TS26_NFC_REQ_048 | VOID |
| TS26_NFC_REQ_049 | VOID |
| TS26_NFC_REQ_050 | VOID |
| TS26_NFC_REQ_183 | The API SHALL be able to send the Select by AID command with zero length AID (as defined in GlobalPlatform card specification) to the eSE.<br>Note: In order to select the Issuer Security Domain without knowing the AID. |
