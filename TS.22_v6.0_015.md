---
source: "TS.22_v6.0.docx"
chunk_id: 015
section_path:
  - "3.1 Operator Policy Provisioning"
---

## 3.1 Operator Policy Provisioning

Expanded service of operators through service agreements and partnerships can significantly increase the coverage and list of network identifiers (e.g. SSID) within a user’s subscription. An update mechanism shall be in place to broker the inclusion of new parameters and data (e.g. SSIDs) within the user’s subscription, together with the exclusion or removal of irrelevant ones. OMA DM can provide a means to configure a device, either through the 3GPP network or directly over the WLAN access network or some operators may pre-configure a device to select operator controlled APs. In order for the OMA DM client in the device to be able to access the OMA DM server, it is necessary to bootstrap the device with at least the address of the OMA DM server (e.g. URL of the OMA DM server) and the credentials (e.g. username and password) for the OMA DM client to authenticate to the OMA DM Server.

OMA DM Bootstrap specification v1.2 [OMA Device Management Bootstrap] provides three options for configuring the bootstrap information in the device:

1. At the factory, during the device personalization for instance;
1. Via an OMA Push message from the OMA DM server; or,
1. From the information stored in the UICC (in the EF Bootstrap file).

OMA DM provides a means to provision a device at the initialisation phase from the UICC (see [OMA Device Management Bootstrap]). When bootstrap information is stored in the UICC bootstrap file, according to OMA Device Management Bootstrap specification, a device is required to use the information from the EF Bootstrap file, as the device is a GSM device.
