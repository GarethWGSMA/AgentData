---
source: "TS.06_v28.1.docx"
chunk_id: 023
section_path:
  - "8 TAC (IMEI) Usage Rules"
---

## 8 TAC (IMEI) Usage Rules

Satellite

- A device that connects to a Satellite to provide service (voice &/or data) to one or more users, using non-3GPP-NTN technologies as its primary means of connection.
- Examples would include, but not limited to a hand-held phone, a modem on a ship or airplane.
- Note 1: A Device that supports Satellite communication but also supports 3GPP technologies (Terrestrial or NTN) as primary means of connection, does not fall into this category.

Vehicle TCU

Description - A Telematics Control Unit (TCU) which is an embedded device within a vehicle (Car, Lorry etc.)  that provides two-way information communication between the vehicle and an external network.

Example: A Telematics Control Unit (TCU) can be connected to an TN, NTN, road infrastructure or other vehicles control units through wireless communication, it may collect telematics data from the car, such as location, speed, engine data, connection quality, etc., by connecting with various subsystems in the vehicle via data and control buses. It may also offer in-vehicle consumer media services via Wi-Fi and Bluetooth, voice calling and emergency calling.

Mobile Test Platform: (Used for Test TAC Only)

- Description - A device that provides cellular connectivity for hardware and software development testing.
- If the Equipment Type is listed on the TAC form as “Modem”, “Dongle” or “WLAN Router” then the device operating system, will be automatically checked as “None”.
- Each application is made on a per model basis. The Brand Name, Model Name & Marketing Name need to be provided to identify the model.
- The number of TAC numbers requested per application should be enough to cover a three-month production run. One TAC number (which can be used to create up to one million IMEI numbers) is normally more than sufficient in most applications.
- Any amendment to an existing TAC record must be made to the GSMA Device Database using the “Edit TAC” function.
- Some manufacturers produce special test mobile equipment. This type of equipment can harm network integrity if used in the wrong manner. Subsequently MNOs need to be able to identify such equipment. The following requirements apply.
- Where the equipment is based on an existing ME:
- A separate TAC code should be assigned to the Test ME to distinguish it from the existing/original ME.
- Alternatively, a Test IMEI could be allocated to this type of ME if it is supplied to operators for test purposes only and not available commercially.
- Each Test ME’s IMEI shall conform to the IMEI Integrity and Security provisions in Section 7.
- Where 3GPP/3GPP2 equipment is capable of operating in multiple modes the following principles must be adhered to.
- Where the standards permit the same IMEI shall be used for each mode of operation. Where the standards do not permit the use of IMEI then an IMEI shall be allocated specifically to the 3GPP/3GPP2 part and any applicable identification to the non-3GPP/3GPP2 part/s.
- Where physically detachable modular techniques are utilised to provide the transceiver capability then each transceiver module shall be treated as a separate ME. Therefore, separate TAC allocations are required if an IMEI is applicable to each module.
- Colour variants of the same model. If different models of the same device vary in the colour of the exterior body only, then the same TAC can be used for all models. No other cosmetic variants are allowed under this exception.
