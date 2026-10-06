---
source: "TS.09_v13.docx"
chunk_id: 091
section_path:
  - "11.2 Headset – Talk Time"
---

## 11.2 Headset – Talk Time

- This scenario shall be run on top of a Talk Time scenario (ref. sections 4 or 5).
- The test shall be run with a commercially available Bluetooth certified headset.

When measuring talk time, a voice signal shall be sent in both directions of the Bluetooth connection. Reasoning: This approach prevents a Bluetooth device to enter sniff mode during silence periods.

The test setup simulates a regular call situation with the headset connected to the terminal under test and a regular voice call open to a second terminal. The baseband role (Master\Slave) of the Phone when connected with a Bluetooth headset is another factor that can affect the power consumption. It is recommended that this parameter is reported (typically Phone is Master of the connection).
