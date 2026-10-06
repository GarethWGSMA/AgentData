---
source: "TS.09_v13.docx"
chunk_id: 082
section_path:
  - "9.2 Dynamic Adaptive Streaming over HTTP (DASH)"
---

## 9.2 Dynamic Adaptive Streaming over HTTP (DASH)

Description

Dynamic Adaptive Streaming over HTTP or DASH video content can be played by loading the provided web page through a web browser. The reference content for DASH Video Streams can be retrieved from the GSMA website.

Initial configuration

The bearer used shall be the most efficient one, and bearer parameters used shall be stated in the test results.

| Filename | Bit Rate (kbps) | fps | Resolution / Size | Video Part | Audio Part |
| --- | --- | --- | --- | --- | --- |
| dash_720p.html | 3000 | 30 | 1280x720 (HD) | H.264 | AAC |

: Set of reference DASH streaming formats

The pre-installed Web Browser of the DUT shall be used for DASH Video Streaming. Full Screen shall be enabled, if supported by the DUT.

The Video Stream shall be played using the inbuilt (hands free) speaker of the DUT. If this is not available, the original stereo cable headset or original Bluetooth headset (or one recommended by the terminal manufacturer) shall be used.

Test procedure

1. Connect to the Reference Content Portal to obtain the web page content
1. Start the download by selecting the appropriate video stream. After the connection is successfully established with the streaming server and the download has started, start watching the movie.
1. After 30 s of the start of the video download above, start the power consumption measurement.
1. The video content shall be downloaded to the DUT as fast as possible with the selected radio profile to reflect how videos are streamed to UEs from public video portals in practice.
1. Stop the power consumption measurement after 10 minutes (total duration between the time stamps of the first and last power samples).
