---
source: "TS.22_v6.0.docx"
chunk_id: 026
section_path:
  - "4.6 Managing Radio Connections based on Multiple Access Technologies"
---

## 4.6 Managing Radio Connections based on Multiple Access Technologies

3GPP operators would like to effectively manage the distribution of data traffic between the 3GPP and WLAN access networks in order to maximise the overall system capacity whilst not compromising the user experience. In order to achieve those objectives, it is required that a device can offload a data flow from 3GPP to WLAN as well as switch the data flow back from WLAN to 3GPP. If the device has more than one data flow e.g. from different applications running in parallel on the device, it is also required that the device can maintain both the 3GPP connection and WLAN connection to allow distribution of the separate flows on different access technologies.

The 3GPP operator may provide a device with policies (e.g. subscription specific policies) that indicate, for example, the preferred access technology (e.g. 3GPP vs. WLAN) to use under specific conditions, priority among WLAN access networks or how traffic should be distributed between the 3GPP and WLAN access networks. The conditions for applying specific policies such as location and time and the rules for distributing traffic between access technologies may be based on policy management solutions, for example, ANDSF (Access Network Discovery and Selection Function) as defined in 3GPP TS 23.402 [3GPP TS 23.402], 3GPP TS 24.302 [3GPP TS 24.302] and TS 24.312 [3GPP TS 24.312].

A device should adhere to policies received from the 3GPP network e.g. priority among WLAN access networks or between 3GPP and WLAN, unless this would conflict with user preference settings (which should be considered with highest priority) or would result in selection of a WLAN access network that is not suitable. The device should evaluate whether a WLAN access network is suitable according to the principles in Section 4.3 of this PRD. Thus, in presence of more than one suitable WLAN access network, a device should select the one prioritised by the 3GPP operator policy (unless overridden by user preference settings). A device should also prefer a WLAN access network that is suitable over one that is not suitable, when both networks are allowed by 3GPP operator policy (even though the WLAN access network that is not suitable may be prioritised by the policy).

A device may also consider the status of a device e.g. battery life for choosing not to connect to a WLAN access network (and connect to 3GPP), provided that no 3GPP operator policy is available that prioritises WLAN over 3GPP or 3GPP operator policy prioritises WLAN, but the available WLAN access networks (that can be accessed according to operator policy) are not suitable. Alternatively, a device may connect to a WLAN access network that is not suitable if there is no other connectivity option available i.e. the 3GPP network or another suitable WLAN access network that the device is allowed to access according to operator policy or a WLAN access network prioritised by user preference.

| Req ID | Requirement |
| --- | --- |
| TSG22_R2_CM_24 | A device SHOULD be able to off-load a data flow from 3GPP to WLAN (and vice versa). |
| TSG22_R2_CM_25 | A device SHOULD be able to maintain concurrent 3GPP and WLAN connectivity. |
| TSG22_R2_CM_26 | VOID |
| TSG22_R2_CM_48 | VOID |
| TSG22_R3_CM_50 | A device SHALL enable the selection of the appropriate access technology based on the following priority order:<br>User Preference<br>Operator Policy<br>Device status and heuristics |
