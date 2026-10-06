---
source: "TS.09_v13.docx"
chunk_id: 012
section_path:
  - "2.2 Common Parameters"
---

## 2.2 Common Parameters

There are certain parameters that are common to all modes of operation as shown in the table below.

| Item | Parameter |
| --- | --- |
| Ambient Temperature | 18-25 Celsius |
| PLMN | Home |
| Backlight | Default setting<br>Measurements in (any) Idle Mode should be taken after the backlight went off.<br>Measurements for video, browsing, streaming etc., the backlight should be on.<br>Measurements for music etc., the backlight should be off. |
| SIM | Supporting clock stop |
| Keypad | No activity except for browsing |
| Cell Broadcast | Not used |
| Cell Reselection | No |
| System Information 13 | Is an optional message which allows for more efficient decoding of BCCH. This is an important message for GPRS; although optional, it is almost universally used, therefore it has been added to the scenario. |
| Display Contrast/Brightness | Default (as delivered by factory) |
| Test Environment Lightning | Office conditions with no direct sun shine on the DUT |
| Audio Volume | Middle of available range |

: Common parameters to all modes of operations

The following external resources provide input files for the tests described in this specification. The files have to be downloaded onto a dedicated media or streaming server before using them for the tests.

The files can be found on GitHub public repository at the following link: https://github.com/GSMATerminals/Battery-Life-Measurement-Test-Files-Public/tree/master

All relative paths listed in what follows refer to the repository top path.

VoLTE Call:

. ./reference_files/audio/call/volte/volte.wav

Audio stream:

. ./reference_files/audio/streaming/audio_only_stream_aac.3gp

Browsing:

./reference_files/browsing/textimage.htm

Music:

. ./reference_files/audio/playback/music.mp3

Progressive Video Streaming:

. ./reference_files/video/streaming/progressive/video_stream_480p_30fps_a.mp4
. ./reference_files/video/streaming/progressive/video_stream_720p_30fps_a.mp4
. ./reference_files/video/streaming/progressive/video_stream_720p_30fps_b.mp4
. ./reference_files/video/streaming/progressive/video_stream_720p_30fps_c.webm
. ./reference_files/video/streaming/progressive/video_stream_1080p_30fps_a.mp4
. ./reference_files/video/streaming/progressive/video_stream_1080p_30fps_b.mp4
. ./reference_files/video/streaming/progressive/video_stream_1080p_30fps_c.webm
. ./reference_files/video/streaming/progressive/video_stream_1080p_60fps_b.mp4
. ./reference_files/video/streaming/progressive/video_stream_2160p_30fps_c.webm

DASH (Dynamic Adaptive Streaming over HTTP) Video Streaming:

. ./reference_files/video/streaming/dash/dash_720p.html

Video Playback application:

. ./reference_files/video/playback/video_player_01.3gp
. ./reference_files/video/playback/video_player_02.3gp
. ./reference_files/video/playback/video_player_03.3gp
. ./reference_files/video/playback/video_player_04.3gp
. ./reference_files/video/playback/video_player_05.3gp
. ./reference_files/video/playback/video_player_06.mpg
. ./reference_files/video/playback/video_player_07.mpg
. ./reference_files/video/playback/video_player_08.mpg

Camera:

. ./reference_files/camera/photo.gif
