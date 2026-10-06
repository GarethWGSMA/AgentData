---
source: "TS.22_v6.0.docx"
chunk_id: 022
section_path:
  - "4.3 WLAN Radio Link and Connection Quality"
---

## 4.3 WLAN Radio Link and Connection Quality

On most devices, once a WLAN is detected, a device defaults to use the WLAN connection to provide data connectivity to applications. Unfortunately, being connected to the AP does not necessarily mean that there is data connectivity to the Internet or that the connectivity will provide adequate user experience. For the purpose of WLAN access network selection (See Section 4.5) and management of multiple radio connections on the device (See Section 4.6), consideration of the WLAN radio link and connection quality are important to avoid poor user experience.

A device should consider over the air utilization of the WLAN AP (e.g. WLAN channel utilization which may be advertised in beacons), backhaul status of an AP (e.g. Wi-Fi Alliance Hotspot 2.0 WAN metrics information which may be obtained via an ANQP request), WLAN signal strength (e.g. WLAN Beacon RSSI as specified in TS 36.304 [3GPP TS 36.304] clause 5.6.2 for ANDSF and RAN rules) to avoid connection to an AP with no connectivity or which is not suitable to provide basic connectivity. The criteria defining a suitable AP may be default criteria in the device and should include at least a minimum signal strength level (e.g. WLAN Beacon RSSI), a maximum channel utilisation value for air interface loading (as defined by WLAN channel utilization in IEEE 802.11) and a minimum backhaul bandwidth threshold. The minimum backhaul bandwidth may be derived from information received in Wi-Fi Alliance Hotspot 2.0 WAN metrics Information element. These criteria may also be preconfigured by the operator in the device or provisioned as part of operator policy. If criteria (e.g. as defined by priorities and/or thresholds) are pre-configured or provisioned by the operator, they should be considered with higher priority than default values. The device may in addition have proprietary schemes to consider additional parameters in order to determine whether the AP is adequate or not.

Once a device is connected on a WLAN access network it should be able to monitor whether the AP can continue to provide adequate throughput (as defined by a default minimum throughput threshold criterion, preconfigured operator policy on minimum throughput threshold or operator provisioned policy containing a minimum throughput threshold). If the minimum throughput threshold cannot be satisfied, the device should be able to switch its connection to another AP or to a 3GPP network.

| Req ID | Requirement |
| --- | --- |
| TSG22_R2_CM_13 | A device SHALL have the capability to monitor the WLAN signal strength (e.g. WLAN Beacon RSSI). |
| TSG22_R2_CM_14 | A device SHOULD consider the following parameters, when available, in selection of a AP, based on default priorities and/or thresholds for those parameters specified by the manufacturer:<br>-   WLAN signal strength (WLAN Beacon RSSI)<br>-   IEEE 802.11 Channel Utilization IE<br>-   Wi-Fi Alliance Hotspot 2.0  WAN Metrics IE |
| TSG22_R2_CM_15 | A device SHOULD be able to monitor the data throughput level on the serving AP. |
| TSG22_R2_CM_16 | A device SHOULD have the ability to switch their network connection away from a serving AP which is not providing adequate throughput (as defined by a minimum throughput threshold criterion, which is default, preconfigured by operator policy, or provisioned by operator policy) to another AP, or to a 3GPP network. |
| TSG22_R2_CM_17 | A device MAY support provisioning with priorities and/or thresholds related to WLAN signal strength and quality, WLAN Beacon RSSI, Wi-Fi Alliance Hotspot 2.0 WAN metrics information and minimum WLAN data throughput level e.g. pre-configured or as part of operator policies. |
| TSG22_R2_CM_18 | A device SHOULD use provisioned priorities and /or thresholds by the operator, when present, with higher priority than default manufacturer priorities/thresholds. |
| TSG22_R4_CM_52 | A release 12 and post-release 12 device, SHALL use 3GPP operator policies and RAN assistance parameters as defined in TS 23.402 [3GPP TS 23.402] clause 4.8, TS 24.302 [3GPP TS 24.302] clauses 5.4, 6.8 and 6.10 and TS 24.312 [3GPP TS 24.312] for ANDSF and in TS 23.401 [3GPP TS 23.401] clause 4.3.23, TS 23.060 [3GPP TS 23.060] clause 5.3.21, TS 36.304 [3GPP TS 36.304] clause 5.6 , TS 36.331 [3GPP TS 36.331] clause 5.6.12, in TS 25.304 [3GPP TS 25.304] clause 5.10 and TS 25.331 [3GPP TS 25.331] for RAN rules. |
