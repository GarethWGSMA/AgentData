---
source: "TS.09_v13.docx"
chunk_id: 072
section_path:
  - "6.1 General"
---

## 6.1 General

The set-up is described for UEs having a standard headset audio jack as described in [10]. If such interface is not available, another headset interface may be used.

To simulate a call with a 40/40/20 voice activity pattern (40% talk / 40% listen / 20% silence), 4 s audio followed by silence is sent on the uplink via the UE audio jack to the test equipment. The test equipment loops back the packets introducing a 5 s end to end delay. It is tolerated that the jitter of audio packet loopback delays can reach up to 2 ms maximum (measured at the LTE simulator).

A 10 second long reference audio file is provided (see the “Common Parameters” section); it contains a 4 s audio activity followed by silence. This reference audio file is repeatedly injected into the DUT audio input while the current drain is being measured.

This methodology yields to a global “40% talk / 40% listen / 20% silence” voice activity pattern (Figure below).

The DUT current drain is measured during 10 minutes (The UE display shall be OFF).

: Voice Activity Pattern
