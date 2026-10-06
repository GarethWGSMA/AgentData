---
source: "TS.22_v6.0.docx"
chunk_id: 043
section_path:
  - "10 IMS Services"
---

## 10 IMS Services

There are existing GSMA PRDs that are relevant to service support on terminals. They should be considered in conjunction with this document. With respect to the support of IMS based services being delivered over WLAN, the relevant GSMA PRDs are:

IR.51 IMS Profile for Voice, Video and SMS over untrusted Wi-Fi access, Version 6.0, 01 May 2018
IR.61 Wi-Fi Roaming Guidelines, Version 12.0, 27 September 2017
IR.92 IMS Profile for Voice and SMS, Version 12.0, 02 May 2018
IR.94 IMS Profile for Conversational Video Service, Version 12.0, 12 June 2017

With the deployment of Passpoint networks, the development of Carrier Wi-Fi as well as presence of Wi-Fi in many homes, operators are now wishing to deploy services that make use of the Wi-Fi networks to deliver services to their customers. An example of such is IMS based service over Wi-Fi, in particular voice (Wi-Fi Calling) and SMS.

Terminals using Wi-Fi requiring to use these services, must be able to access the EPC via WLAN, either trusted WLAN or untrusted WLAN, as defined in 3GPP TS 23.402.

The terminals need to support the following aspects:

IMS basic capabilities and supplementary services for telephony
Real-time media negotiation, transport, and codecs
Wi-Fi wireless technology (as described in this document GSMA PRD TS.22) and (evolved) packet core capabilities
Functionality that is relevant across the protocol stack and subsystems.

A terminal compliant to this profile must support IMS-based telephony as detailed in the GSMA PRD IR.51 which defines a voice and video over Wi-Fi IMS profile by profiling a number of Wi-Fi, (Evolved) Packet Core, IMS core, and terminal features. These features are considered essential to launch interoperable IMS based voice and video over Wi-Fi. GSMA PRD IR.51 is based on the IMS Voice and SMS profile described in GSMA PRD IR.92 and on the IMS Profile for Conversational Video Service profile described in GSMA PRD IR.94. The defined profile is compliant with 3GPP specifications.

GSMA PRD IR.51 also references this document, GSMA PRD TS.22, which outlines the Wi-Fi wireless technology and packet core feature set. Consequently, the two documents need to be considered in unison.

Reference also needs to be made to GSMA PRD IR.61, which describes some of the network and terminal requirements for the support of SWu, SWw and S2b interfaces.

The terminal needs to be able to support a PDN connection as defined in 3GPP TS 23.402 [3GPP TS 23.402] to the EPC over the Wi-Fi wireless interface to access IMS based voice, SMS and video services.

NOTE: Emergency calls over EPC-integrated Wi-Fi is not specified in 3GPP.

This document only provides details of access to the EPC using untrusted Wi-Fi networks as supported by terminals and networks.

If the terminals support either IMS-based voice or SMS or video services, (or a combination), the following requirements must be met by the terminal.

| Req ID | Requirement |
| --- | --- |
| TSG22_R3_SVC_01 | Terminals MAY support IMS based voice, or SMS, or video service, over Wi-Fi. |
