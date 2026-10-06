---
source: "TS.26_v15.1.docx"
chunk_id: 053
section_path:
  - "7.4 UI Application triggering requirements"
---

## 7.4 UI Application triggering requirements

The same generic requirements are applicable to Android platform with the following requested implementation:

| TS26_NFC_REQ_129 | VOID |
| --- | --- |

: VOID

| TS26_NFC_REQ_096 | VOID |
| --- | --- |

: VOID

| TS26_NFC_REQ_187 | Transaction Event is provided natively by Android.<br>A Transaction Event (EVT_TRANSACTION) SHALL be triggered based on the following information: |
| --- | --- |

| Action | android.nfc.action.TRANSACTION_DETECTED |
| --- | --- |
| Mime type | - |
| URI | nfc://secure:0/<SEName>/<AID><br>- SEName reflects the originating SE<br>It must be compliant with GlobalPlatform Open Mobile API<br>- AID reflects the originating UICC applet identifier, in upper case hexadecimal format |

: Table: Intent Details for TRANSACTION_DETECTED

| TS26_NFC_REQ_188 | Transaction event data SHALL be set in the following extended field: |
| --- | --- |

| android.nfc.extra.AID<br>ByteArray | Contains the card “Application Identifier” |
| --- | --- |
| android.nfc.extra.DATA<br>ByteArray | Payload conveyed by the HCI event<br>“EVT_TRANSACTION” [optional] |
| android.nfc.extra.SECURE _ELEMENT_NAME<br>String | Indicates the Secure Element on which the transaction occurred.<br>eSE1...eSEn for Embedded Secure Elements, SIM1...SIMn for UICC, etc. |

: Table: TRANSACTION_DETECTED data

| TS26_NFC_REQ_098 | VOID |
| --- | --- |
| TS26_NFC_REQ_182 | VOID |
| TS26_NFC_REQ_097 | VOID |
| TS26_NFC_REQ_099 | VOID |
| TS26_NFC_REQ_189 | The framework SHALL generate a send broadcast intent toward application signed with an allowed hash in access rules. |
