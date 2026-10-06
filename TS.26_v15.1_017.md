---
source: "TS.26_v15.1.docx"
chunk_id: 017
section_path:
  - "6.1 NFC Device Architecture"
---

## 6.1 NFC Device Architecture

The following figure provides an overview of a typical Mobile NFC architecture:

: Mobile NFC Architecture

The device provides, as standard component, a NFC controller and one or more SEs.

The NFC Stack is driving the NFC Controller and is typically providing software APIs enabling:

- Management of Multiple Secure Element (activation, deactivation, routing, etc.)
- Management of the NFC events
- An external API available for 3rd party applications to manage reader/writer mode, Peer to Peer mode and Card Emulation mode from Device
- An internal API to provide a communication channel with an embedded Secure Element for APDU exchanges

The Secure Element Access API provides a communication channel (using APDU commands) allowing 3rd party applications running on the Mobile OS to exchange data with Secure Element Applets. This API provides an abstraction level common for all Secure Elements and could rely on different low level APIs for the physical access:

- RIL extension for accessing the UICC
- Specific libraries for communicating with other embedded secure elements

In order to implement security mechanisms (e.g. Secure Element Access Control), the Secure Element Access API shall use Mobile OS mechanisms such as UIDs or application certificates to identify the calling application.
