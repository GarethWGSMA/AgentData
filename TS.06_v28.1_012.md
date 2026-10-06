---
source: "TS.06_v28.1.docx"
chunk_id: 012
section_path:
  - "5 International Mobile Equipment Identity (IMEI)"
---

## 5 International Mobile Equipment Identity (IMEI)

The IMEI uniquely identifies an individual mobile device. The IMEI is unique to every ME and thereby provides a means for controlling access to 3GPP/3GPP2 networks based on ME Model or individual units.

The “IMEI” consists of a number of fields totalling 15 digits. All digits have the range of 0 to 9 coded as binary coded decimal. Values outside this range are not permitted.

Some of the fields in the IMEI are under the control of the Reporting Body (RB). The remainder is under the control of the Type Allocation Holder.

For the IMEI format prior to 01/01/03 please refer to Annex D of this document. The IMEI format valid from 01/01/03 is as shown below:

| TAC | Serial No | Check Digit |
| --- | --- | --- |
| NNXXXXXX | ZZZZZZ | A |

The meaning of the acronyms for the IMEI format is:

| TAC | Type Allocation Code |
| --- | --- |
| NN | Reporting Body Identifier |
| XXXXXX | ME Model Identifier defined by the Reporting Body |
| ZZZZZZ | The range is allocated by the Reporting Body but assigned per ME by the Type Allocation Holder |
| A | Check digit, defined as a function of all other digits |
