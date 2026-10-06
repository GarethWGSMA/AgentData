---
source: "TS.22_v6.0.docx"
chunk_id: 024
section_path:
  - "4.5 WLAN Access Network Selection"
---

## 4.5 WLAN Access Network Selection

WLAN access network selection in a pre-release 12 device should take into consideration 3GPP operator policies for WLAN access network selection. The operator policies may indicate priority among WLAN access networks e.g. based on a pre-configured list of network identifiers or provisioned by the 3GPP operator. The 3GPP operator policies should have highest priority among all available policies in the device for network selection. However, user preference settings should be able to override 3GPP operator policies on WLAN selection.

A device should be able to support association on a preferred WLAN access network, if the SSID is broadcast. Moreover, in order to avoid selection of a WLAN access network with poor radio link and/or data connection quality, a device should evaluate whether a WLAN access network is suitable, according to the requirements of Section 4.3 of this PRD. The criteria for determining whether a WLAN access network is suitable can be default criteria in the device, a criteria pre-configured by the operator or provisioned as part of operator policies for WLAN access network selection.

In the presence of more than one suitable WLAN access network, a device should select the one prioritised by the 3GPP operator policy (unless overridden by user preference settings). A device should also prefer a WLAN access network that is suitable over one that is not suitable, when both networks are allowed by 3GPP operator policy (even though the WLAN access network that is not suitable may be prioritised by the policy).
