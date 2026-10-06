---
source: "TS.09_v13.docx"
chunk_id: 023
section_path:
  - "2.6.1 E-UTRA Standby Parameters"
---

## 2.6.1 E-UTRA Standby Parameters

This OCNG Pattern for FDD fills with OCNG all empty PRB-s (PRB-s with no allocation of data or system information) of the DL sub-frames, when the unallocated area is discontinuous in frequency domain (divided in two parts by the allocated area – two sided), starts with PRB 0 and ends with PRB .

| Relative power level  [dB] | Relative power level  [dB] | Relative power level  [dB] | PDSCH Data |
| --- | --- | --- | --- |
| Subframe | Subframe | Subframe | PDSCH Data |
| 0 | 5 | 1 – 4, 6 – 9 | PDSCH Data |
| Allocation | Allocation | Allocation | PDSCH Data |
| 0 – (First allocated PRB-1)<br>and<br>(Last allocated PRB+1) – () | 0 – (First allocated PRB-1)<br>and<br>(Last allocated PRB+1) – () | 0 – (First allocated PRB-1)<br>and<br>(Last allocated PRB+1) – () | PDSCH Data |
| 0 | 0 | 0 | Note 1 |
| NOTE 1:	These physical resource blocks are assigned to an arbitrary number of virtual UEs with one PDSCH per virtual UE; the data transmitted over the OCNG PDSCHs shall be uncorrelated pseudo random data, which is QPSK modulated. The parameteris used to scale the power of PDSCH.<br>NOTE 2:	If two or more transmit antennas with CRS are used in the test, the OCNG shall be transmitted to the virtual users by all the transmit antennas with CRS according to transmission mode 2. The parameter applies to each antenna port separately, so the transmit power is equal between all the transmit antennas with CRS used in the test. The antenna transmission modes are specified in section 7.1 in [15]. | NOTE 1:	These physical resource blocks are assigned to an arbitrary number of virtual UEs with one PDSCH per virtual UE; the data transmitted over the OCNG PDSCHs shall be uncorrelated pseudo random data, which is QPSK modulated. The parameteris used to scale the power of PDSCH.<br>NOTE 2:	If two or more transmit antennas with CRS are used in the test, the OCNG shall be transmitted to the virtual users by all the transmit antennas with CRS according to transmission mode 2. The parameter applies to each antenna port separately, so the transmit power is equal between all the transmit antennas with CRS used in the test. The antenna transmission modes are specified in section 7.1 in [15]. | NOTE 1:	These physical resource blocks are assigned to an arbitrary number of virtual UEs with one PDSCH per virtual UE; the data transmitted over the OCNG PDSCHs shall be uncorrelated pseudo random data, which is QPSK modulated. The parameteris used to scale the power of PDSCH.<br>NOTE 2:	If two or more transmit antennas with CRS are used in the test, the OCNG shall be transmitted to the virtual users by all the transmit antennas with CRS according to transmission mode 2. The parameter applies to each antenna port separately, so the transmit power is equal between all the transmit antennas with CRS used in the test. The antenna transmission modes are specified in section 7.1 in [15]. | NOTE 1:	These physical resource blocks are assigned to an arbitrary number of virtual UEs with one PDSCH per virtual UE; the data transmitted over the OCNG PDSCHs shall be uncorrelated pseudo random data, which is QPSK modulated. The parameteris used to scale the power of PDSCH.<br>NOTE 2:	If two or more transmit antennas with CRS are used in the test, the OCNG shall be transmitted to the virtual users by all the transmit antennas with CRS according to transmission mode 2. The parameter applies to each antenna port separately, so the transmit power is equal between all the transmit antennas with CRS used in the test. The antenna transmission modes are specified in section 7.1 in [15]. |

: E-UTRA_FDD_idle_1 / OP.2 FDD: Two sided dynamic OCNG FDD Pattern
