---
source: "TS.09_v13.docx"
chunk_id: 015
section_path:
  - "2.3.3 GSM Talk Time and GPRS PS Data Transfer Parameters"
---

## 2.3.3 GSM Talk Time and GPRS PS Data Transfer Parameters

All common parameters (section 2.2) apply, plus the additional GSM configuration parameters. Some bearer parameters shall be selected among some recommended values. These parameters and the selected value shall be reported with the tests results.

| Parameter | Value | Comment |
| --- | --- | --- |
| Hopping | On |  |
| Hopping Sequence (850) | 128, 159, 189, 219, 251 |  |
| Hopping Sequence (900) | 1, 30, 62, 93, 124 |  |
| Hopping Sequence (1800) | 512, 600, 690, 780, 855 |  |
| Hopping Sequence (1900) | 512, 590, 670, 750, 810 |  |
| Hopping Sequence (450) | 259, 268, 276, 284, 293 |  |
| Hopping Sequence (480) | 306, 315, 323, 331, 340 |  |
| Handover | No |  |
| Rx Level | -82 dBm |  |
| Terminal Tx Level (900, 850, 480 & 450) | (max, PCL=7 (29 dBm), min) | Used pcl values for max and min shall be reported with the test results |
| Terminal Tx Level (1800, 1900) | (max, PCL=1 (28 dBm), min) | Used pcl values for max and min shall be reported with the test results |
| Uplink Dtx | Off |  |
| Call | Continuous |  |
| Codec | EFR |  |
| No of neighbour cells declared in the BA_LIST | 16 Frequencies As Defined In Annex A |  |

: GSM parameters for Talk Time and Packet Switched Data Transfer

NOTE:	Where transfer is band specific, the band measured must be specified

The following parameters are suggested based on observations of real operation. Justifications follow the table. However these are only suggestions and it is recommended that vendors define the test for their most efficient transfer mode. The test results and the channel parameters used to perform the test should all be reported in the last column of the table.

| Parameter | Suggested Value | Used Value<br>(To Be Reported) |
| --- | --- | --- |
| Multi-Slot Class | 12 |  |
| Terminal Type | 1 |  |
| Slots (Uplink) | 1 |  |
| Slots (Downlink) | 4 |  |
| Duty Cycle | 100% |  |
| Coding Scheme | CS4 |  |
| CS Can Change | No |  |
| Transfer Mode | Acknowledged |  |
| Non Transparent | Yes |  |
| Retransmissions | Yes |  |

: Additional parameters for Packet Switched Transfer

All GPRS UEs currently available are generally “class 12” or higher. Therefore, “class 12” operation (4DL, 1UL slots) has been chosen as the baseline for this test. Type 1 operation has also been chosen as being the lowest common denominator.

Other parameters have been selected to represent the terminal being used as a modem for download of a large block of data. This choice was made for two reasons:

1. It is an operation that the user will actually perform, and that will occur in much the same way regardless of the user (unlike browsing for example, which is highly user specific)
1. It is relatively easy to set up on test equipment.

Acknowledged mode is specified as this is generally used for data downloads. For the same reason non-transparent mode is chosen. Finally, the coding scheme with the highest throughput (lowest protection) was chosen and it was decided that this coding scheme would not change (no link adaptation).

NOTE:	No retransmissions are supposed to happen. The sensitivity or decoding performance of the terminal is not measured – no fading channel is specified – the purpose of the tests in this document is to establish the power consumption of the mobile equipment on an ideal (and easily reproducible) channel. In view of this and the relatively high receive signal strength, retransmissions are not expected.
