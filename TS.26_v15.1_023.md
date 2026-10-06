---
source: "TS.26_v15.1.docx"
chunk_id: 023
section_path:
  - "6.3.1 Mobile Device Modem Requirements"
---

## 6.3.1 Mobile Device Modem Requirements

| TS26_NFC_REQ_045 | For handling logical channel Baseband SHALL provide interfaces based on either the following AT commands or equivalent functionality:<br>AT+CCHO<br>AT+CCHC<br>AT+CGLA |
| --- | --- |
| TS26_NFC_REQ_045.1 | Modem SHALL support all lengths of AID from 5 bytes to 16 bytes as defined in ISO/IEC 7816-4. |
| TS26_NFC_REQ_141 | The modem SHALL provide a way for the application processor to retrieve the answer from the UICC after the selection of an AID. |
| TS26_NFC_REQ_111 | Modem SHALL provide an interface based on AT+CRSM (Restricted SIM Access) or equivalent functionality for internal communication on basic channel. |
| TS26_NFC_REQ_112 | The Modem SHALL prevent the usage of the AT+CSIM or equivalent functionality. |
| TS26_NFC_REQ_113 | Modem SHALL support APDU transmission case 1, 2, 3 & 4 as defined in ISO/IEC 7816-4. |
| TS26_NFC_REQ_161 | Modem SHALL support Extended Length APDU as defined in ISO/IEC 7816-4 with at least 2048 bytes command and response data field size.<br>Note: This requirement will become effective from the 1st January 2018. |
| TS26_NFC_REQ_114 | For all APDU exchanges originating from the Secure Element Access API the Modem driver SHALL forward warning status codes (SW=62XX or 63XX) directly to the application level without any change. |
| TS26_NFC_REQ_155 | For all APDU exchanges originating from the Secure Element Access API the Modem driver SHALL allow the mobile application to perform a GET RESPONSE after any warning status code (SW=62XX or 63XX) is sent back by the UICC. |
| TS26_NFC_REQ_115 | VOID |
| TS26_NFC_REQ_046 | Access to the UICC (logical channel) SHALL be allowed even when the mobile device is in a Radio OFF state, i.e. flight mode, airplane mode etc. |
| TS26_NFC_REQ_142 | The modem SHALL support 19 logical channels in addition to the basic channel. |
