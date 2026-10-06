---
source: "TS.22_v6.0.docx"
chunk_id: 027
section_path:
  - "4.7 Traffic management across RATs"
---

## 4.7 Traffic management across RATs

Maintaining network operator services across varying network technologies provides better network performance through offloading. However, disruption of services should be kept at a minimum when switching between different network technologies e.g. switching from 3G to WLAN.

It is important that the mobile network connection be kept when a device switches between network technologies for the following reasons:

- For core network capacity (i.e. no new PDP context establishment on 3GPP on every AP connection).
- Charging tickets processing load
- Transparent user interface

It is important that network inactivity timer mechanisms keep working as normal. When a device attaches to a new AP, the following scenarios may apply (in networks configured via DHCP or with static IP configuration):

Switch between APs within the same BSS. In this case, the IP layer connectivity stays the same (layer 2 handover only).
Switch between APs of different BSSs within the same ESS. Depending on the implementation, IP connectivity may stay the same, but may also change.
Switch to an AP of a different ESS, the AP/network is known and configured, and the old lease is not outdated. For example, in private networks, leases can be in the range of days or even static and therefore this situation is not uncommon.

If a devices AP changes, the DHCP function of a device should issue a DHCP request to the new AP even if the identity or network identifier (e.g. SSID) of the AP does not change.  However, this process could be slow since the device needs to go through a complete DHCP exchange before it is able to communicate. RFC 4436 [RFC 4436] proposes to cache information about the network (own IP configuration parameters, MAC and IP addresses of test node(s) in the network) and to probe them quickly using (unicast) ARP after the link comes up.

If the probing confirms that the network looks the same, there is no need to re-acquire the IP address via DHCP. The device simply continues to use its current lease. Nevertheless, it is recommended to do DHCP in parallel, to avoid additional delays if the probes result in a negative answer.

If a device retains information about multiple networks, it can also accelerate the return to your private networks. It also helps if a device switches back and forth between two hotspots for some reason.

In order to improve the IP address utilisation, a device shall send DHCP Release message to an AP to release its IP address in the following circumstances:

1. Users disconnect from applications
2. Users switch from the current network identifier to another
3. Users turn WLAN off
4. Users turn Flight Mode on when one network identifier is connected

3GPP signaling procedures for moving PDN connections between 3GPP and WLAN accesses while ensuring IP address preservation are specified in TS 23.402 [3GPP TS 23.402] for “untrusted WLAN” (based on SWu and S2b) and in TS 23.402 [3GPP TS 23.402] clause 16 signaling procedures for “trusted WLAN” (based on SWw and S2a).

The decision to move certain traffic between 3GPP access and WLAN is taken by the device, based on policy rules and assistance provided by the network, measurements performed by the device and local operating environment information. For 3GPP devices, using USIM credentials for authentication, these policy rules may be either ANDSF traffic steering rules per TS 23.402 [3GPP TS 23.402] clause 4.8, TS 24.302 [3GPP TS 24.302] clauses 5.4, 6.8 and 6.10 and TS 24.312 [3GPP TS 24.312], or 3GPP RAN traffic steering rules per TS 23.401 [3GPP TS 23.401] clause 4.3.23, TS 23.060 [3GPP TS 23.060] clause 5.3.21, TS 36.304 clause 5.6 [3GPP TS 36.304], TS 36.331 [3GPP TS 36.331] clause 5.6.12, TS 25.304 [3GPP TS 25.304] clause 5.10 and TS 25.331 [3GPP TS 25.331].
