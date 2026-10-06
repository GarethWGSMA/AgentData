---
source: "TS.26_v15.1.docx"
chunk_id: 014
section_path:
  - "5.1 Dual Application architecture"
---

## 5.1 Dual Application architecture

GSMA Operators promote the following application architecture (below) to pragmatically support the key use case of secured NFC services.

: Dual application architecture

The mobile device User Interface (UI) application executing on the device OS is the consumer facing component. In this example, the UI application interacting with the application on an SE, communicating with the NFC reader, allows the customer to interact with the service functionalities, e.g. with a PoS (point of sale) for a financial service use case or a physical ticketing barrier in the case of an e-ticketing application. However the UI Application component is not seen as mandatory for all use cases, where the Service Provider (SP) could decide to have a UI-less service, including when the service is intended to be deployed on Basic Devices. It could be also the case that device applications without UI are deployed and finally a User Interface does not necessarily require the presence of a display, but it could be achieved by sounds, LEDs or vibrates. In the rest of the document the term “UI” designates all kind of interfaces allowing an interaction with or a simple notification to the user.

The applet component resides within the SE, and works in tandem with the UI application when applicable. It holds the logic of the application and performs actions such as holding secure authentication keys or time-stamped transaction data for transaction resolution, history and fraud prevention etc.

Within this dual-application architecture for secured services, there is need for a consistent communication channel between these two applications. This communication channel could be used to transmit status information passed from the application in the SE to the UI for notifying the user on NFC events. It could also be used for more information exchanges between the SE and the device UI like user authentication toward a SE applet (e.g. PIN code verification).

As the communication channel accesses a secured storage space on the SE, the communication channel itself must have attributes which allow it to be accessed only by authorised UI applications.

The following illustration gives an overview of the device software components required to satisfy the dual application architecture, which delivers key use cases for NFC, in case of a NFC handset with a UICC.

: Mobile Device API generic software stack

The mandated method of communication between these two applications is APDU (Application Protocol Data Unit).

The following figure depicts the typical data flow for a NFC transaction, between a PoS and a UICC, including the routing that the event will need to follow. The event is the trigger from the PoS to the user which indicates an activity in the NFC service. From this activity the nature of the event between the various components can be determined, for example where the event needs to be protected and has attributes which will allow for, or not allow for, any modification. The same flow will take place between a PoS and an eSE

: Typical data flow for card-emulation mode
