---
source: "TS.22_v6.0.docx"
chunk_id: 039
section_path:
  - "7.4 Access to U/SIM When 3GPP Radio is in Flight Mode"
---

## 7.4 Access to U/SIM When 3GPP Radio is in Flight Mode

There is the potential use case for a terminal to have its Wi-Fi radio enabled but its 3GPP radio is off, such as the 3GPP radio being in flight mode. One such case may be in an aircraft where use of the Internet via an on board Wi-Fi network is permitted but the use of cellular radio is still banned. Some customers turn off their 3GPP connections when roaming and their devices should still be able to use Passpoint based authentication when roaming.

If the WLAN is Passpoint enabled, then the terminal needs to be able to access the U/SIM credentials for authentication on the WLAN even though the 3GPP radio is off or in flight mode.

| Req ID | Requirement |
| --- | --- |
| TSG22_R3_USE_12 | Terminals SHOULD allow Passpoint authentication using U/SIM credentials even though the 3GPP radio is off or in flight mode. |
