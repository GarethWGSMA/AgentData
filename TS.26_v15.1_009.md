---
source: "TS.26_v15.1.docx"
chunk_id: 009
section_path:
  - "1.5 Definition of Terms"
---

## 1.5 Definition of Terms

| Term | Description |
| --- | --- |
| Active CEE | An Active CEE is a CE environment that can receive data based on routing mechanisms (e.g. AID, Protocol and Technology). |
| Active UICC Profile | When the physical UICC is a standard UICC: the UICC itself.<br>When the physical UICC is an eUICC: the combination of the Enabled Profile and the eUICC onto which the Profile has been provisioned. |
| AID Conflict | When two or more applications register with the same Application Identifier |
| AID Conflict Detection | Conflict Detection is the procedure to check for AID Conflict. Conflict Detection can be done<br>1. During registration of Application Identifiers<br>2. When an Application selection is being received from a contactless reader. |
| APDU | An Application Protocol Data Unit (APDU) is the communication unit between a smart card reader and a smart card. |
| Application Identifier | AID, as defined in ISO/IEC 7816-4, used to address a card emulation service or application |
| Basic Device | A Device with no screen or with a small basic display (i.e. not able to display menus) |
| Battery Operational Mode | The battery of the DUT has sufficient power to support all functions in the mobile devices. |
| Battery Low Mode | The battery of DUT has reached “Battery Low Threshold” at which the display and most functionalities of the DUT are automatically switched off, except the clock and a few remaining functions. The battery of the DUT only has sufficient power to support NFC controller to function in card emulation mode. |
| Battery Power-off Mode | The battery of the DUT has reached “Battery Power-off threshold” at which there is no residual power to support NFC controller to function. No functions are available in the DUT. The NFC controller can function if power is provided via the contactless interface (i.e. power by the field). |
| Card Emulation Environment | A Card Emulation Environment is an execution environment used together with a NFC controller to manage a Card Emulation transaction. It can be a Secure Element (e.g. UICC, embedded Secure Element or micro-SD) or an application running in a device host. |
| Default AID Route | The Default AID route is the route used by the NFC Controller when a NFC reader explicitly selects a NFC Service by its AID but the AID is not defined in the NFC Controller’s routing table.<br>Note: this definition is only relevant for devices which support the Multiple Active CEEs model. |
| Device | In the context of this specification, the term Devices is used to represent any electronic equipment supporting NFC functionality into which a NFC Secure Element can be inserted, and that provides a capability for a server to reach the UICC through an Over The Air (OTA) channel. E.g. smartphones, wearables. |
| Embedded UICC | A removable or non-removable UICC which enables the remote and/or local management of Profiles in a secure way.<br>NOTE: The term originates from "embedded UICC". |
| Embedded SE | Secure Element which is a separated chipset and integrated into the devices, owned by the device manufacturer and cannot be removed. |
| Multiple Active CEEs model | A model where the device can activate several CEE at the same time. RF traffic can be provided to a CEE based on routing mechanisms.<br>Note: an implementation may support Multiple Active CEEs model in Battery Operational Mode and Single Active CEE model in Battery Low or Power-Off Mode. |
| Operator | Refers to a Mobile Network Operator who provides the technical capability to access the mobile environment using an Over The Air (OTA) communication channel. The OPERATOR is also the UICC Issuer. An OPERATOR provides a UICC OTA Management System, which is also called the OTA Platform. |
| Prefix of AIDs | An AID prefix will match all AIDs that are starting with the same N bytes of the mentioned AID prefix. |
| Screen Lock | The device functionality can only be accessed via a user intervention. |
| Screen ON | The battery of the device is in Battery Operational Mode and the screen of the device was turned on by the end-user (i.e. the screen is active). |
| Screen OFF | The battery of the device is in Battery Operational Mode and the screen of the device was turned off either by the end-user or automatically by the device after a timeout. |
| Switched OFF | The device was turned OFF by the end-user or the device is in battery low mode or the device is in battery power-off mode. |
| Secure Element | A SE is a tamper-resistant hardware component which is used to provide security, confidentiality, and multiple application environments required to support various business models. In TS.26, the term SE includes UICC, eUICC and eSE. |
| Sensitive API | An API which shall be protected from malicious use. |
| Single Active CEE model | A model where the device only activates one CEE at a time. Other CEEs, if available, are not active. |
