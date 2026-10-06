---
source: "TS.09_v13.docx"
chunk_id: 027
section_path:
  - "2.6.2 E-UTRA (VoLTE) Talk Time Parameters"
---

## 2.6.2 E-UTRA (VoLTE) Talk Time Parameters

: E-UTRA parameters for talk time

NOTE:	Output power: The mean power of one carrier of the UE, delivered to a load with resistance equal to the nominal load impedance of the transmitter.

Mean power: When applied to E-UTRA transmission this is the power measured in the operating system bandwidth of the carrier. The period of measurement shall be at least one sub-frame (1 ms) for frame structure type 1 and one sub-frame (0.675 ms) for frame structure type 2 excluding the guard interval, unless otherwise stated.

Further assumptions:

. CQI is set to 1
. EPS Network Feature Support is enabled and IMS Voice over PS supported.
. SPS Disabled (UL dynamic scheduling enabled)
. No SRS is transmitted
. No HARQ and ARQ retransmissions are expected – low bit error rate is assumed
. No System Information (on PDSCH or PBCH) or paging is received
. Default Codec is AMR-WB. If the EVS codec is supported, then the EVS AMR-WB IO mode may be used as an alternative implementation of AMR-WB.
