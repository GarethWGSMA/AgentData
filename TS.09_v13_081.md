---
source: "TS.09_v13.docx"
chunk_id: 081
section_path:
  - "9.1 Video Progressive Streaming"
---

## 9.1 Video Progressive Streaming

Description

UEs do support a variety of different streaming formats, which makes it difficult to determine one “default” video stream suitable for every UE. Therefore, a set of core video formats is defined and is available on the streaming server as reference content.

| Filename | Bit Rate<br>(kbps) | fps | Resolution / Size | Video Part | Audio Part |
| --- | --- | --- | --- | --- | --- |
| video_stream_480p_30fps_a.mp4 | 1500 | 30 | 854x480 (FWVGA) | H.264 | AAC |
| video_stream_720p_30fps_a.mp4 | 3000 | 30 | 1280x720 (HD) | H.264 | AAC |
| video_stream_720p_30fps_b.mp4 | 10000 | 30 | 1280x720 (HD) | H.265 | AAC |
| video_stream_720p_30fps_c.webm | 1300 | 30 | 1280x720 (HD) | VP9 | VORBIS |
| video_stream_1080p_30fps_a.mp4 | 5800 | 30 | 1920x1080 (HD) | H.264 | AAC |
| video_stream_1080p_30fps_b.mp4 | 12000 | 30 | 1920x1080 (HD) | H.265 | AAC |
| video_stream_1080p_30fps_c.webm | 2300 | 30 | 1920x1080 (HD) | VP9 | VORBIS |
| video_stream_1080p_60fps_b.mp4 | 20000 | 60 | 1920x1080 (HD) | H.265 | AAC |
| video_stream_2160p_30fps_c.webm | 17000 | 30 | 3840x2160 (HD) | VP9 | VORBIS |

: Set of reference streaming formats

Initial configuration

The power consumption measurement shall be carried out by selecting and re-playing the stream with the highest possible bit rate and codec that are supported by the DUT. If the terminal capabilities are unknown, the test shall be started with highest numbered Video Stream in the table. If this stream does not work, the next lower Video Stream shall be used. As per the principles in section 7, the bearer used shall be the most efficient one, and bearer parameters used shall be stated in the test results.

The pre-installed Media Player of the DUT shall be used for Video Streaming. Full Screen shall be enabled, if supported by the DUT.

The Video Stream shall be played using the inbuilt (hands free) speaker of the DUT. If this is not available, the original stereo cable headset or original Bluetooth headset (or one recommended by the terminal manufacturer) shall be used.

Test Procedure

1. Connect to the Reference Portal to obtain the video content.
1. Start the download by selecting the appropriate video. After the connection is successfully established with the streaming server and the download has started, start watching the clip.
1. After 30 s of the start of the video download above, start the power consumption measurement.
1. The video content shall be downloaded to the DUT as fast as possible with the selected radio profile to reflect how videos are streamed to UEs from public video portals in practice.
1. Stop the power consumption measurement after 10 minutes (total duration between the time stamps of the first and last power samples).
: Video Streaming and Power Consumption Measurement

The reference content for Video Streams can be retrieved from the GSMA website. It can be noticed that the filename itself gives some information about the video/audio encoder that applies:

| Filename | Video Codec | Audio Codec |
| --- | --- | --- |
| xxxx_a.* | H264 | AAC |
| xxxx_b.* | H265 | AAC |
| xxxx_c.* | VP9 | VORBIS |

: Progressive Streaming filenames and Video/Audio Codecs
