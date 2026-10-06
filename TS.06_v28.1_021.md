---
source: "TS.06_v28.1.docx"
chunk_id: 021
section_path:
  - "8 TAC (IMEI) Usage Rules"
---

## 8 TAC (IMEI) Usage Rules

The following requirements shall be adhered to:

- Each TAC can only be used for a single ME Model
- One ME Model will have a single device type and will have one or more TAC.
- Modular Equipment may use an interchangeable transceiver module to achieve the ability to operate in alternative 3GPP/3GPP2 bands. Such equipment is to treat each transceiver module as a separate ME. This will mean that each transceiver equipment module would be subject to Type Allocation and be allocated a separate TAC and therefore separate IMEIs. The IMEI shall not be duplicated in separate transceiver equipment.
- Requirements for a device containing multiple transceivers:
- If a device contains two or more transceivers, each transceiver must be separately identified on networks.
- If two or more transceivers within the same device are identical (e.g., same chipset, same frequency bands, same control software), then each transceiver can use the same TAC, but different IMEI.
- A single transceiver may serve one or several UICCs/eUICC Profiles/SUPI-NsI(s). If only one (U)SIM/eUICC Profile on one of the served UICCs/eUICCs or only one of the SUPI-NsI(s) can be used to connect to the network at any time, then only one IMEI is required. If more than one (U)SIM/eUICC Profile/SUPI-NsI can be served at the same time by a transceiver, for example in Stand-by Mode, the transceiver shall have multiple unique IMEIs so that all (U)SIMs/eUICC Profiles/SUPI-NsI(s) that are served at the same time will use a separate unique IMEI.
- See TS.37 Requirements for Multi SIM Devices, for more information about the implementation of Multiple (U)SIM in devices.
- For devices with:
- Multiple (U)SIMs/eUICC Profiles/SUPI-NsI(s) which are all Active at the same time (have simultaneous connections to the network) each (U)SIM/eUICC Profile/SUPI-NsI must use a separate, unique IMEI.
- Multiple (U)SIMs/eUICC Profiles/SUPI-NsI(s) where some (U)SIM(s) /eUICC Profiles/SUPI-NsI (s) are in Standby Mode (only listening on the network) each (U)SIM/SUPI-NsI(s) must use a separate, unique IMEI.
- Multiple (U)SIMs/eUICC Profiles/SUPI-NsI(s) which are all Passive (only one can connect to the network at any time and the connection is switched between the (U)SIM/eUICC Profiles/SUPI-NsI) only one IMEI is required to be allocated to the transceiver.
- If the transceivers are different (e.g., different chipset, different frequency bands, different control software), then the transceivers must have a different TAC, and the transceiver serving the (U)SIM(s)/eUICC Profiles/SUPI-NsI(s) would therefore have a different IMEI from the same TAC.
- Each transceiver shall have enough unique IMEIs so that all (U)SIMs/eUICC Profiles/SUPI-NsI(s) that are served at the same time can use separate, unique IMEIs.
- For further requirements for devices with Multiple (U)SIMs, see GSMA PRD TS.37.
- All TAC numbers allocated by the Reporting Bodies are stored in the GSMA Device Database. For confidentiality reasons, access to the Device Database is restricted.
- Before applying for a TAC number, the applicant company must first register with a GSMA appointed RB. Evidence must be provided with (or in addition to) the application to ensure the following:
- That the applicant (i.e., Brand Owner) is a legitimate organization and is selling a product that is to connect to the Telecoms Network,
- For Modem manufacturers, it should be the manufacturer who requests the TAC as these may go into many different devices. In all other cases it should be the Brand Owner who requests the TAC.
- TAC can be requested for NTN Devices. These may connect to NTN only or NTN and TN networks.
- NTN frequency bands can be selected with any Equipment Type listed below.
- All devices may connect to 3GPP TN and/or NTN
- The following Equipment Types are listed on the TAC application form:

Mobile / Feature Phone:

- Description - A device supporting basic personal communication services, e.g., voice call and SMS. (Not strictly limited to basic services, but not entering in the definition of a Smartphone).
