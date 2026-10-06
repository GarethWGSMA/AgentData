---
source: "TS.16_v5.0.docx"
chunk_id: 007
section_path:
  - "5 TAC (IMEI) Usage Rules"
---

## 5 TAC (IMEI) Usage Rules

The following requirements must be adhered to:

Each ME Model must have its own TAC. One ME Model will have one or more TAC
Modular Equipment may use an interchangeable transceiver module to allow it to operate in alternative GSM bands. Such equipment is to treat each transceiver module as a separate ME. This means that each transceiver equipment module would be subject to Type Allocation and be allocated a separate IMEI/TAC. The IMEI shall not be duplicated in separate transceiver equipment.
Requirements for a device containing multiple transceivers:
If a device contains two or more transceivers, each transceiver must be separately identified on networks.
If two or more transceivers within the same device are identical (e.g. same chipset, same frequency bands, same control software), then each transceiver can use the same TAC, but different IMEI.
If the transceivers are different (e.g. different chipset, different frequency bands, different control software), then the transceivers must have different TACs.
A single transceiver may be connected to one or several UICCs/eUICCs. If only one (U)SIM on one of the connected UICCs/eUICCs can be used to connect to the network at any time then only one IMEI is required. If more than one (U)SIM can be connected at the same time to a transceiver, for example in Stand-by Mode, the transceiver shall have multiple, unique IMEIs so that all (U)SIMs, that are connected at the same time, will use a separate, unique IMEI.
For devices with:
Multiple SIMs which are all Active at the same time (have simultaneous connections to the network) each SIM must use a separate, unique IMEI.
Multiple SIMs where some SIM(s) are in Standby Mode (only listening on the network) each SIM must use a separate, unique IMEI
Multiple SIMs which are all Passive (only one can connect to the network at any time and the connection is switched between the SIM) only one IMEI is required to be allocated to the transceiver.
If the transceivers are different (e.g. different chipset, different frequency bands, different control software), then the transceivers must have a different TAC, and the SIM(s) associated with that transceiver would have an IMEI from the same TAC.
