---
source: "TS.09_v13.docx"
chunk_id: 083
section_path:
  - "9.3 Audio Streaming"
---

## 9.3 Audio Streaming

Description

Audio Streams are usually only supplied on WCDMA – E-UTRA Bearers, i.e. this test only applies to WCDMA – E-UTRA capable UEs only. The reference content for Audio Streams can be retrieved from the GSMA website.

The following core audio streaming formats are defined and available on the streaming server as reference content as follows:

|  | Codec | Bit Rate | Sampling Rate | SBR Signalling |
| --- | --- | --- | --- | --- |
| Audio Stream 1 | AAC+ | 32 kbps | 44.1 kHz | 0 (= implicit) |
| Audio Stream 2 | AAC-LC Stereo | 96 kbps | 44,1 kHz | Not applicable |

: Set of Audio stream formats

Initial configuration

The pre-installed Media Player of the DUT shall be used for Audio Streaming.

The Audio Stream shall be played using the inbuilt (hands free) speaker of the DUT. If this is not available, the original stereo cable headset or original Bluetooth headset (or one recommended by the terminal manufacturer) shall be used.

Test procedure

1. Connect to the Reference Content Portal to obtain the audio content
1. The actual playing time should be 10 minutes
1. After successfully established connection to the streaming server, start listening to the audio clip
1. Start Power Consumption Measurement
