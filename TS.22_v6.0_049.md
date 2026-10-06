---
source: "TS.22_v6.0.docx"
chunk_id: 049
section_path:
  - "10.4 Wi-Fi Calling/VoWiFi"
---

## 10.4 Wi-Fi Calling/VoWiFi

The set of requirements are listed below:

| Req ID | Requirement |
| --- | --- |
| TSG22_R6_SVC_10 | Terminals SHALL be capable of providing a single and integrated user interface for any mobile service that is delivered over both cellular and Wi-Fi access networks. |
| TSG22_R6_SVC_11 | Terminals SHALL provide a UI that enables the user to change the Wi-Fi Calling settings (e.g., to change the Wi-Fi vs. Cellular preferred setting, or to enable/disable Wi-Fi Calling). Note, disabling Wi-Fi Calling functionality changes the connection setting of the terminal to Cellular only mode. |
| TSG22_R6_SVC_12 | Terminals SHALL enable Wi-Fi Calling by default when the terminal first boots up and no user preferences have been set. |
| TSG22_R6_SVC_13 | Terminals SHALL allow users to select one of the calling options: Wi-Fi only (e.g., when international roaming), Wi-Fi preferred, cellular preferred and cellular only. |
| TSG22_R6_SVC_14 | Terminals SHALL use Wi-Fi preferred profile by default when Wi-Fi Calling is enabled |
| TSG22_R6_SVC_15 | When Wi-Fi preferred is enabled by the user (and Wi-Fi preferred is allowed by the provider policy) and the terminal is within range of an available Wi-Fi network, the terminal SHALL access Wi-Fi Calling services irrespective of availability of the cellular network. |
| TSG22_R6_SVC_16 | When Wi-Fi preferred is enabled and no Wi-Fi network is available, the terminal SHALL use the cellular network (if available) for all services while continuing to monitor for Wi-Fi. |
| TSG22_R6_SVC_17 | When Wi-Fi only is enabled (i.e. don’t use Cellular), the terminal SHALL switch off the cellular radio and it SHALL access Wi-Fi Calling services when Wi-Fi is available. |
| TSG22_R6_SVC_18 | When Wi-Fi only is enabled (i.e. don’t use Cellular), the terminal SHALL route all non IMS data traffic over Wi-Fi. |
| TSG22_R6_SVC_19 | When Wi-Fi only is enabled (i.e. don’t use Cellular), and if no qualified Wi-Fi networks are available, the terminal SHALL not try to scan/enable/connect to the cellular network. |
| TSG22_R6_SVC_20 | If Wi-Fi Calling is disabled while Wi-Fi only is enabled, then the Wi-Fi only behaviour SHALL no longer apply (i.e., the terminal can use cellular access to support voice calling). |
| TSG22_R6_SVC_21 | When cellular preferred is enabled, the terminal SHALL select an available cellular network for access to calling services when both cellular and Wi-Fi are available. |
| TSG22_R6_SVC_22 | When cellular preferred is enabled and a cellular network is not available or cellular coverage is poor, the terminal SHALL access Wi-Fi Calling services over an available Wi-Fi network. |
| TSG22_R6_SVC_23 | When cellular preferred is enabled, the terminal SHALL not try to handover active Wi-Fi Calling sessions from cellular to Wi-Fi when good cellular coverage is available. |
| TSG22_R6_SVC_24 | When cellular preferred is enabled, the terminal SHALL seamlessly handover active Wi-Fi Calling sessions from cellular to Wi-Fi if cellular coverage becomes poor. |
| TSG22_R6_SVC_25 | When cellular only is enabled, the terminal SHALL access all Wi-Fi Calling services (e.g., voice, video, text) over cellular. The terminal SHALL provide data services (e.g., internet browsing) over available Wi-Fi. For example, when cellular-only is enabled, and there is no cellular coverage or poor cellular coverage, the terminal will behave as if there were no Wi-Fi Calling; i.e., it will always attempt to use cellular for Wi-Fi Calling services, and it will not attempt to provide mobile voice and text over Wi-Fi after connecting to Wi-Fi. |
| TSG22_R6_SVC_26 | Terminals SHALL provide a user-friendly UI for initiating emergency calls. |
| TSG22_R6_SVC_27 | Terminals SHALL support initiating a Wi-Fi Calling call from the phone’s native dialer, contact list, and call logs. |
| TSG22_R6_SVC_28 | Terminals SHALL support receiving a Wi-Fi Calling call using the phone’s native interface. |
| TSG22_R6_SVC_29 | Terminals SHALL support Wi-Fi Calling messaging services from the phone’s native SMS/MMS application. |
| TSG22_R6_SVC_30 | Terminals SHALL support user browsing of Internet and checking emails and other data connection activities while active in a Wi-Fi Calling call. |
| TSG22_R6_SVC_31 | When the user changes the terminal’s Wi-Fi Calling setting from “disabled” to “enabled”, the terminal SHALL select an access network based on network availability and network preference settings, and register with the IMS over that access network. |
| TSG22_R6_SVC_32 | When the user changes the terminal’s Wi-Fi Calling setting from “enabled” to “disabled”, the terminal SHALL de-register with the home IMS. |
| TSG22_R6_SVC_33 | When the terminal is set to Airplane mode and the Wi-Fi is enabled with connectivity, the terminal MAY attempt to register for Wi-Fi Calling based on the operator’s policy. |
| TSG22_R6_SVC_34 | If the terminal is in airplane mode and the user enables Wi-Fi, the terminal SHALL follow the connection preferences set in determining connection. The preferences shall not be changed automatically. |
| TSG22_R6_SVC_35 | If the terminal is in airplane mode and Wi-Fi Calling is set to cellular preferred mode and the Wi-Fi is enabled, the terminal SHALL register for Wi-Fi Calling but shall not attempt to search for cellular coverage. |
| TSG22_R6_SVC_36 | While in airplane mode with Wi-Fi enabled (i.e., cellular radio is disabled), the terminal SHALL attempt to access emergency services over Wi-Fi. |
| TSG22_R6_SVC_37 | If the terminal is registered for Wi-Fi Calling and the user disables airplane mode, the IMS registration SHALL be maintained. |
| TSG22_R6_SVC_38 | If the terminal detects a handover trigger during a voice call that is established over Wi-Fi (e.g., low RSSI level), and there are no alternate cellular or Wi-Fi networks available, then the terminal SHALL generate a two tone beep alerting user that the call might drop. |
| TSG22_R6_SVC_39 | Terminals SHALL select either cellular or Wi-Fi access for emergency calls, based on operator policy configured in the terminal or conveyed to the terminal at network attachment time. |
| TSG22_R6_SVC_40 | Terminals SHALL establish emergency calls over an available Wi-Fi network if no cellular network is available. |
| TSG22_R6_SVC_41 | When the terminal is on a Wi-Fi call, the Wi-Fi Calling icon SHALL indicate that the call is on Wi-Fi. |
| TSG22_R6_SVC_42 | If the user attempts to initiate a call while Wi-Fi Calling is disabled, and there is no cellular coverage, then the terminal SHOULD pop up a message that reminds the user to enable Wi-Fi Calling in order to make calls. |
| TSG22_R6_SVC_43 | Terminals SHALL have a capability to update or modify Wi-Fi calling IMS settings based on the SIM Card insert. This allows a user to change MNO or to pass their terminal to a different user who will have an open market-like terminal. |
