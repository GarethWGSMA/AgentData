---
source: "TS.22_v6.0.docx"
chunk_id: 038
section_path:
  - "7.3 Authentication Architecture Overload Data Prevention"
---

## 7.3 Authentication Architecture Overload Data Prevention

In some networks, EAP authentication could be reserved for some tariff plans for marketing reasons (e.g. no WLAN access for basic offers).

Hence, some devices could be parameterised with automatic EAP authentication and perform automatic connection attempts to a WLAN access network. If the network rejects the access request of a device for a repeated number of times due to WLAN barring, the device must stop any other request until a manual attempt is made. Otherwise, this could lead to some core network overload.

Frequent attempts to connect to barred APs will have a detrimental effect on usability and battery life.

According to the relevant IETF RFCs, certain EAP-enabled authentication frames support Fast Re-authentication methods. These are enabled by the Authentication Server providing Fast Re-Authentication Identity and other parameters to the WPATM supplicant instantiated on the end-user device, as part of normal Full Authentication procedure. When the WPA supplicant requires authentication subsequent to a given Full Authentication, it can optionally use a Fast Re-authentication procedure.

Note:

- compared to Fast Re-authentication, Full Re-Authentication places a number of additional loading factors on service-provider access and core-network resources;
- compared to 3GPP mobile data RAN infrastructure, challenges to predicting and engineering against WLAN attachment/detachment scenarios. When Full Authentication is required for each device re-attachment, the additional load becomes difficult to predict.
- For example, with EAP-SIM, according to RFC 4186 clause 10.18, when receiving the error code 1031 – User has not subscribed to the requested service.

For these reasons, where authentication frames support Fast Re-authentication procedures, these should be supported in a device.

| Req ID | Requirement |
| --- | --- |
| TSG22_R2_USE_08 | A device SHALL refrain from attempting an automatic connection when barred due to permanent (and not temporary) authentication failure or notification after the authentication request is rejected, unless a manual attempt is made. |
| TSG22_R2_USE_09 | A device with a UI SHALL notify to the user the failure of authentication. |
| TSG22_R2_USE_10 | A device SHALL implement the fast re-authentication mechanism described in the RFC 4186 – EAP SIM. |
| TSG22_R2_USE_11 | A device SHALL support fast re-authentication mechanism described in the EAP AKA [RFC 4187] / EAP AKA’ [RFC 5448]. |
