---
source: "TS.06_v28.1.docx"
chunk_id: 037
section_path:
  - "17 TAC Allocation Process"
---

## 17 TAC Allocation Process

It was noted that there was a need for a transition period to allow:

- The Operators to modify their systems to use the eight-digit TAC rather than a six digit one
- The Manufacturers to make any necessary changes to their production processes.
- The Reporting Bodies to make any changes to their IMEI allocation systems.
- The GSM Association to make any changes to their databases and systems.
- The Contractor to make any changes to its systems.

The transition period ran from 31/12/02 until 1/4/04.

To achieve this transition, all eight-digit TAC codes allocated between 31/12/02 and 31/3/04 were given unique combinations of the first six digits (NNXXXX) with the seventh and eighth digits (YY) being fixed to 00.

Any request by a Terminal Manufacturer for a FAC code after 31/12/02 resulted in that Manufacturer being supplied with a fresh 8-digit TAC. This was to allow the 3GPP industry to move to the 8-digit TAC code without the need to implement changes to their IMEI analysis and tracking systems before 1/4/04.

The meaning of the acronyms for the IMEI format valid until 31/12/02 is:

| TAC | Type Allocation Code, formerly known as Type Approval Code |
| --- | --- |
| NN | Reporting Body Identifier |
| XXXX | ME Type Identifier defined by Reporting Body |
| FAC | Final Assembly Code |
| YY | Under control of the Reporting Body. May be used to indicate the manufacturing site. More than one FAC per site should be used to permit production of greater than 1000000 ME. |
| ZZZZZZ | Allocated by Reporting Body but assigned per ME by the manufacturer |
| A | Phase 1 = 0<br>Phase 2 (or later) = Check digit, defined as a function of all other IMEI digits |

Type Allocation Code - 6 digits. (Valid prior to 01/01/03)

The TAC identifies the Type Allocation Code, formerly known as the Type Approval Code, for the type of the ME. It consists of two parts; the first part defines the Reporting Body allocating the TAC and the second part defines the ME type.

The following allocation principles apply:

- Each ME Type shall have a unique TAC code or set of TAC codes.
- More than one TAC may be allocated to an ME Type at the discretion of the Reporting Body. This may be done to permit the production of more than 1 million units or to distinguish between market variations.
- The TAC code shall uniquely identify an ME Type.
- If the TAC was granted to a particular software version of one ME Type that is then used in another ME type the TAC code shall be different.
- TAC codes may vary between software versions for a phase 1 ME Type at the discretion of the Reporting Body.
- In Phase 2 (and later releases) the TAC shall remain the same and the SV number shall identify the software version. See IMEISV.
- Where there is more than one Type Allocation Holder for an ME Type then the TAC code shall be different.
Reporting Body Identifier (NN) – 2 digits (valid prior to 01/01/03)

The first two digits of the TAC are the Reporting Body Identifier. These digits indicate which Reporting Body issued the IMEI. The GSM Association shall coordinate the allocation of the first 2 digits to Reporting Bodies. See Annex A for IMEI Reporting Body Identifiers that have already been allocated.

Valid Range 00 – 99 in accordance with allocations in Annex A

The following allocation principles apply:

- The GSM Association shall coordinate the allocation of the Reporting Body Identifier.
- The Reporting Body Identifier shall uniquely identify the Reporting Body.
- If for some reason the same Reporting Body Identifier must be used, then the first digit of the ME Type Identifier will also be used to define the Reporting Body. The GSM Association shall coordinate the allocation to the Reporting Body of the range of values of the first digit of the ME Type Identifier. This range shall be contiguous. This approach is to be avoided if at all possible.
ME Type Identifier (XXXX) – 4 digits (valid prior to 01/01/03)
