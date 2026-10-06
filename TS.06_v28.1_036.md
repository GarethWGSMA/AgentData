---
source: "TS.06_v28.1.docx"
chunk_id: 036
section_path:
  - "17 TAC Allocation Process"
---

## 17 TAC Allocation Process

List of Test IMEI allocating bodies

| 1st 6 digits of the Test IMEI | Allocating Body | Contact Person(s) | Telephone | Fax | E-mail |
| --- | --- | --- | --- | --- | --- |
| 001 001-001 017 | GSM North America, CTIA | Ms. Karen Castro | +1 202 736 3223 | +1 202 466 3413 | CTIA - IMEI IMEI@ctiacertification.org |
|  |  |  |  |  |  |
| 00 44 MMMM | TÜV SÜD | Mr. John Talbot | +44 1932 251264 | +44 1932 251201 | John.Talbot@tuv-sud.co.uk<br> imei@tuvsud.com |
|  |  |  |  |  |  |
| 00 86 MMMM | TAF (Telecommunication Terminal Industry Forum Association<br>) | Ms. Su Hui | +86 10 82052809 | +86 10 82051448 | suhui@taf.org.cn |

Informative Annex – IMEISV (IMEI Software Version)

The Network can also request the IMEISV from Phase 2 (or later) ME. The IMEISV shall contain the first 14 digits of the IMEI plus a Software Version Number (SVN). The SVN shall be incremented when the ME software is modified. Allocation of the 2 digit SVN may be controlled by the Reporting Body, at the discretion of the Reporting Body. SVN of “99” is reserved for future use (See GSM 03.03).

GSM 02.16 - MS Software Version Number (SVN)

A Software Version Number (SVN) field shall be provided. This allows the ME manufacturer to identify different software versions of a given type approved mobile.

The SVN is a separate field from the IMEI, although it is associated with the IMEI, and when the network requests the IMEI from the MS, the SVN (if present) is also sent towards the network. It comprises 2 decimal digits.

3GPP TS 22.016 - MS Software Version Number (SVN)

A Software Version Number (SVN) field shall be provided. This allows the ME manufacturer to identify different software versions of a given mobile.

The SVN is a separate field from the IMEI, although it is associated with the IMEI, and when the network requests the IMEI from the MS, the SVN (if present) is also sent towards the network.

Structure of the IMEISV

The structure of the IMEISV is as follows:

| TAC | Serial No | SVN |
| --- | --- | --- |
| NNXXXXXX | ZZZZZZ | SS |
| Notes:-<br>NN		Reporting Body Identifier<br>XXXXXX	ME Model Identifier defined by Reporting Body<br>ZZZZZZ	Allocated by Reporting Body but assigned per ME by the manufacturer<br>SS		Software Version Number 00 – 98. 99 is reserved for future use. | Notes:-<br>NN		Reporting Body Identifier<br>XXXXXX	ME Model Identifier defined by Reporting Body<br>ZZZZZZ	Allocated by Reporting Body but assigned per ME by the manufacturer<br>SS		Software Version Number 00 – 98. 99 is reserved for future use. | Notes:-<br>NN		Reporting Body Identifier<br>XXXXXX	ME Model Identifier defined by Reporting Body<br>ZZZZZZ	Allocated by Reporting Body but assigned per ME by the manufacturer<br>SS		Software Version Number 00 – 98. 99 is reserved for future use. |

Software Version Number Allocation Principles

The Reporting Body, at their discretion, may control allocation of the SVN. All ME designed to Phase 2 or later requirements shall increment the SVN for new versions of software. The initial version number shall be 00. The SVN of 99 shall be reserved.

- The allocation process for SVN shall be one of the following procedures:
- The Reporting Body allocates a new SVN number a new software release.
- The Reporting Body defines the allocating process to be applied by the Type Allocation Holder.

If there are more than 99 software versions released the Reporting Body may undertake one of the following options.

- Issue a new TAC code for the ME Model
Security Requirements

The SVN is not subject to the same security requirements as the IMEI as it is associated with the ME software. The SVN should be contained within the software and incremented every time new software is commercially released. The SVN should uniquely identify the software version.

Informative Annex – Historical Structure of the IMEI
Historical IMEI Structure

The IMEI structure valid until 31/12/02 is as follows:

| TAC | FAC | Serial No | Check Digit |
| --- | --- | --- | --- |
| NNXXXX | YY | ZZZZZZ | A |

Discussions within the industry, including 3GPP2, agreed that the structure change to combine the TAC and FAC into a single eight-digit TAC code.

This format has been documented in the 3GPP requirements 02.16, 03.03, 22.016 and 23.003.

Effectively the FAC code should be considered as obsolete.
