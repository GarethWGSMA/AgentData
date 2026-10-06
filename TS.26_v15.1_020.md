---
source: "TS.26_v15.1.docx"
chunk_id: 020
section_path:
  - "6.2.2 Card Emulation Mode Requirements"
---

## 6.2.2 Card Emulation Mode Requirements

| TS26_NFC_REQ_025 | The mobile device SHALL support Card Emulation as per: TS-Analog, TS-Digital and TS-Activity [NFC Forum Specifications]. |
| --- | --- |
| TS26_NFC_REQ_025.1 | VOID |
| TS26_NFC_REQ_026 | Card Emulation mode SHALL be enabled when the NFC is turned on. |
| TS26_NFC_REQ_027 | For Card emulation mode the read distance SHALL be in the 0cm – 2cms range for battery operational mode, battery low mode. |
| TS26_NFC_REQ_028 | In Single Active CEE model the Active UICC Profile SHALL be the default CEE, that is the active CEE at first start up or after a factory reset. |
| TS26_NFC_REQ_029 | Manufacturers SHALL provide to operators the capability to customise settings for defining if the UICC card emulation is enabled / disabled when the device is powered off, screen is off or locked.<br>Note: this will not be via a UI. |
| TS26_NFC_REQ_030 | In the case of a factory reset, the operator customised settings (as per TSG26_NFC_REQ_029) SHALL remain. |
| TS26_NFC_REQ_031 | Operator settings as stated in TS26_NFC_REQ_029 above SHALL only be valid if NFC is enabled. |
| TS26_NFC_REQ_157 | The device SHALL implement the requirements of the EMV Contactless Communication Protocol Specification, Book D. |
| TS26_NFC_REQ_158 | Card emulation mode SHALL support APDU transmission case 1, 2, 3 & 4 as defined in ISO/IEC 7816-4 including Extended Length Field support. Command and response data field size minimum of 2048 bytes SHALL be supported.<br>Note 1: Currently, the support for extended length APDU is not a common feature of NFC-UICC. At this point in time, NFC-UICC in the field typically don’t support extended length APDU. Both handset architecture and NFC-UICC have to be compliant in order for the device to support the extended length APDU feature.<br>Note 2: The implementation of the protocol and the mechanisms leading to the use of the extended length APDU option according to ISO/IEC 7816-4 have to be ensured by a negotiation between the contactless reader and the selected application in the NFC-UICC. |
