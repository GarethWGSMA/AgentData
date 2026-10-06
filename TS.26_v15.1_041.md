---
source: "TS.26_v15.1.docx"
chunk_id: 041
section_path:
  - "7.1 NFC Device Architecture"
---

## 7.1 NFC Device Architecture

Android is providing, software components, to use the NFC controller and to access one or more Secure Elements (SEs).

: Android NFC software stack

The previous figure gives an overview of a possible Android implementation as an example showing how this requirement can be mapped to an OS.

On Android the architecture could be encapsulated in an Android Service. Having a single service ensures that security checks (who is accessing the service) and resource management (freeing up a logical channel) can be guaranteed.

On Android, such a background component might rely on a RIL extension for accessing the UICC and on some specific libraries, for communicating with any embedded secure elements.
