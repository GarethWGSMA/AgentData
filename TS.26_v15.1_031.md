---
source: "TS.26_v15.1.docx"
chunk_id: 031
section_path:
  - "6.4 UI Application triggering requirements"
---

## 6.4 UI Application triggering requirements

When a transaction has been executed by an applet on a Secure Element, it may need to inform the application layer. To do this, an applet may trigger an event known as “EVT_TRANSACTION”. This HCI event will be sent to the NFC Controller over SWP line. The NFC Controller will then forward this event to the device application processor where the event may trigger an authorized registered mobile application.

How to register a mobile application including the exact mechanism depends on the mobile OS used. This section intends to define the content of this event message and the main principles for its management.

The event message holds the following information:

- SEName (mandatory) reflecting the originating SE. It must be compliant with GlobalPlatform Open Mobile API naming convention and below complementary requirement in case of UICC, using types which are appropriate to the OS programming environment.
- AID (mandatory) reflecting the originating SE (UICC) applet identifier if available
- Parameters (mandatory) holding the payload conveyed by the HCI event EVT_TRANSACTION if available
- When AID is omitted from the URI, application component are registered to any “EVT_TRANSACTION” events sent from the specified Secure Element.

| TS26_NFC_REQ_069 | For UICC, Secure Element Name SHALL be SIM[smartcard slot] (e.g. SIM/SIM1, SIM2… SIMn). |
| --- | --- |
| TS26_NFC_REQ_070 | For embedded SE, Secure Element Name SHALL be eSE[number] (e.g. eSE/eSE1, eSE2, etc.). |
| TS26_NFC_REQ_071 | The device SHALL support HCI event EVT_TRANSACTION as per ETSI TS 102 622. |
| TS26_NFC_REQ_072 | The OS implementation SHALL provide a mechanism to inform authorised OS applications of Transaction Events and this SHALL include the Secure Element name and the AID of the applet which triggered the transaction and PARAMETERS holding the payload conveyed by the HCI EVT_TRANSACTION event. |
| TS26_NFC_REQ_073 | VOID |
| TS26_NFC_REQ_074 | VOID |
| TS26_NFC_REQ_144 | Across all the different system components and the APIs exposed to the developers, the OS/Framework SHALL make available only existing Secure Elements and SHALL name them in a coherent way (i.e. using the same Secure Element names for OMAPI and Transaction events). |
