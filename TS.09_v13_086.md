---
source: "TS.09_v13.docx"
chunk_id: 086
section_path:
  - "10.2 Video Playback"
---

## 10.2 Video Playback

Description

UEs do support a variety of different Video Playback formats. Most common use is the H.264 media format. If this is not supported, MPEG4 Visual Simple Profile Level 0 media format or H.263 Profile 0 Level 10 shall be used to perform this test. The codecs and resolution used for the test shall be specified in the test results.

| Filename | Bit Rate (kbps) | fps | Resolution / Size | Video Part | Audio Part |
| --- | --- | --- | --- | --- | --- |
| video_player_06.mpg | 4000 | 30 | 640x480 (VGA) | H.264 | AAC |
| video_player_07.mpg | 8000 | 30 | 1280x720 (HD 720p) | H.264 | AAC |
| video_player_08.mpg | 10000 | 30 | 1920x1080 (HD 1080p) | H.264 | AAC |

: Set of reference local video formats

Initial configuration

The media file shall be stored onto the handset on the external memory and played back from there. If the DUT does not support an external memory card, the media file shall be stored in the internal phone memory and played from there.

The pre-installed Media Player of the DUT shall be used for Video playback. Background illumination shall be enabled. Screensaver shall be disabled.

The original stereo cable headset or original Bluetooth headset (or one recommended by the terminal manufacturer) shall be used. Full Screen shall be enabled, if supported by the DUT.

Test procedure

1. Save the media file on the phone
1. The actual playing time should be 5 minutes
1. Set the volume to mid-level and start watching the video media clip
1. Start Power Consumption Measurement
