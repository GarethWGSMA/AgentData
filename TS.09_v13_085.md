---
source: "TS.09_v13.docx"
chunk_id: 085
section_path:
  - "10.1 Music Playback"
---

## 10.1 Music Playback

Description

UEs support a variety of different music playback formats. The most common one in use is the mp3 media format. A reference file in this format is supplied on the GSMA web page (see references section). If this format is not supported, a reference file shall be transcoded from this file. The following information shall be noted in the test results.

- Codec used
- Data rate
- Use of internal or external memory
- Radio technology used

The volume used during the test shall also be described in the test results and shall be set to a middle volume level (e.g. 5 out of 10 possible levels). The DUT shall be connected to a WCDMA or E-UTRA network.

Initial configuration

The following parameters are used for the media file:

- Bit Rate: 128 kbps
- Sampling Rate: 44.1 kHz (Stereo)
- Download the reference music file from the GSMA website and store it onto the terminal. The media file shall be stored on the external memory card and played back from there. If the DUT does not support an external memory card, the media file shall be stored in the internal phone memory and played from there.
- The pre-installed Music Player of the DUT shall be used for music playback. Enabling of screensavers shall be set to the default values as delivered from the factory.
- The original stereo cable headset or original Bluetooth headset (or one recommended by the terminal manufacturer) shall be used.

Test procedure

1. Save the media file on the phone (memory selection see above)
1. The actual playing time should be 5 minutes
1. Set the volume to mid-level and start listening to the audio media clip
1. Start Power Consumption Measurement
