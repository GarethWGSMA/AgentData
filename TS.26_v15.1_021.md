---
source: "TS.26_v15.1.docx"
chunk_id: 021
section_path:
  - "6.2.3 Reader/writer mode & TAG management requirements"
---

## 6.2.3 Reader/writer mode & TAG management requirements

All requirements in this chapter are optional for Basic Devices.

| TS26_NFC_REQ_032 | VOID |
| --- | --- |
| TS26_NFC_REQ_033 | The mobile device SHALL support Reader/Writer Mode as per: TS-Analog, TS-Digital and TS-Activity  [NFC Forum Specifications]. |
| TS26_NFC_REQ_034 | VOID |
| TS26_NFC_REQ_035 | The mobile device SHALL support NFC Forum Type 2 Tag, as specified in [NFC Forum Specifications]. Requirement applies to both protocol and application level. |
| TS26_NFC_REQ_036 | The mobile device SHALL support NFC Forum Type 3 Tag, as specified in [NFC Forum Specifications]. Requirement applies to both protocol and application level. |
| TS26_NFC_REQ_037 | The mobile device SHALL support NFC Forum Type 4 Tag, as specified in [NFC Forum Specifications]. Requirement applies to both protocol and application level. |
| TS26_NFC_REQ_192 | The mobile device SHALL support NFC Forum Type 5 Tag, as specified in [NFC Forum Specifications]. Requirement applies to both protocol and application level. |
| TS26_NFC_REQ_038 | Reader mode events SHALL be routed exclusively to the UICC or the Application processor. |
| TS26_NFC_REQ_039 | The default routing for the reader mode events SHALL be via the Application processor. |
| TS26_NFC_REQ_040 | The NFC Controller SHOULD support Reader Mode as per ETSI TS 102 622. |
| TS26_NFC_REQ_041 | The device SHALL support automatic and continuous switching between card emulation and reader mode. |
| TS26_NFC_REQ_159 | VOID |
| TS26_NFC_REQ_160 | The mobile device SHALL support APDU transmission case 1, 2, 3 & 4 including Extended Length Field support as defined in ISO/IEC 7816-4 with 32767 bytes command and response data field size for the Reader/Writer mode. |

Note: 	Default mode Card emulation mode, with a poll for Reader mode, the frequency for the Reader mode poll shall be such that the battery power consumption is kept to a minimum. This implementation will require on-going optimisation; however, the aim is to provide good responsiveness to the consumer.

| TS26_NFC_REQ_042 | A transaction time SHALL take 500ms or less for TAG message length not exceeding 100 bytes. The transaction time is defined from the start of the frame of the first RF command receiving an answer, to the end of the frame of the response to the last received RF command by a device, where the RF command is used to read the content in a tag. |
| --- | --- |
| TS26_NFC_REQ_043 | The mobile device SHALL be able to read/write the NFC Forum Smart Poster RTD. |
| TS26_NFC_REQ_044 | The TAG SHALL be read at a distance of 1 cm and at distances between 0 to 1 cm.<br><br>Note: This requirement will be tested with a TAG Test Reference system agreed in the Test Book group. |
| TS26_NFC_REQ_110 | The TAG SHOULD be read at a distance from 1 cm to 4 cm.<br><br>Note: This requirement will be tested with a TAG Test Reference system agreed in the Test Book group. |
