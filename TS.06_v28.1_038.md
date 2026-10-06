---
source: "TS.06_v28.1.docx"
chunk_id: 038
section_path:
  - "17 TAC Allocation Process"
---

## 17 TAC Allocation Process

The following 4 digits of the TAC are under the control of the Reporting Body. These 4 digits together with the Reporting Body 2 digit identifier uniquely identify each ME Type.

Valid Range 0000 – 9999
The following allocation principles apply:
- Every ME Type shall have a unique TAC or set of TACs. A TAC may not be associated with more than one ME Type. An ME Type may have more than one TAC.
- Major changes to the ME Build Level shall require a new ME Type Identifier. Major changes to ME Build Level would normally include the addition of new features or changes that modify the performance of the ME Type. Minor changes to the ME Build Level that do not change the performance of the ME require no new ME Type Identifier. The Reporting Body shall determine what constitutes a major or minor change to the ME Build Level.
- The ME Type Identifier should be allocated sequentially wherever possible. Gaps in the ME type range are to be avoided if possible.
- Multiband or multimode ME shall only have one TAC and therefore one IMEI. Where more than one Reporting Body is involved in the allocation of the IMEI coordination is required between the Reporting Bodies to ensure that all requirements have been met before the IMEI is allocated.
Final Assembly Code (FAC) - 2 digits (valid prior to 01/01/03)

These two digits (YY) are generally used to identify the specific factory or manufacturing site of the ME. The allocation of the FAC is under the control of the Reporting Body.

Valid Range 00 – 99

The following allocation principles apply:

- More than one FAC should be allocated where necessary to a Factory or site to allow for the situation where the factory produces more than 1 million units per ME Type.
- Further FACs should be requested and assigned for a ME type where the Serial Number Range is exhausted.
- A FAC shall not be used to distinguish between ME Types.
Serial Number (SNR) - 6 digits (valid prior to 01/01/03)

The 6-digit SNR (ZZZZZZ) in combination with the FAC is used to uniquely identify each ME of a particular ME Type.

Valid Range 000000 – 999999

The following allocation principles apply:

- Each ME of each ME Type must have a unique Serial Number in combination with the FAC for a given TAC code.
- SNR shall be allocated sequentially wherever possible.
- The Reporting Body may allocate a partial range to be used for the serial number.
Spare Digit / Check Digit – 1 digit (valid prior to 01/01/03)
Phase 1/1+ ME

For Phase 1 ME this is a spare digit, and its use has not been defined. The spare digit shall always be transmitted to the network as “0”.

Phase 2 (and latter) ME

For Phase 2 (or later) mobiles it shall be a Check Digit calculated according to Luhn formula (ISO/IEC 7812). See GSM 02.16. The Check Digit shall not be transmitted to the network. The Check Digit is a function of all other digits in the IMEI. The Software Version Number (SVN) of a Phase 2 (or later) mobile is not included in the calculation.

The purpose of the Check Digit is to help guard against the possibility of incorrect entries to the CEIR and EIR equipment.

The presentation of Check Digit (CD) both electronically (see Section 5) and in printed form on the label and packaging is very important. Logistics (using bar-code reader) and EIR/CEIR administration cannot use the CD unless it is printed outside of the packaging, and on the ME IMEI/Type Accreditation label.

The check digit shall always be transmitted to the network as “0”.

Test TAC Application form.

If a Test IMEI/TAC is required as defined in GSMA PRD TS.06 section 9.0 then the details in the following form must to be completed and sent to the IMEI Helpdesk (imeihelpdesk@gsma.com) the Helpdesk will then pass on the Test TAC request form to the appropriate Reporting Body for processing.

Test TAC application form
