---
source: "TS.26_v15.1.docx"
chunk_id: 038
section_path:
  - "6.8 Card Application Toolkit Support"
---

## 6.8 Card Application Toolkit Support

The following requirements list the minimum letter classes’ support for NFC device.

| TS26_NFC_REQ_087 | A device which implements Rel-11 or earlier of ETSI TS 102 223 SHOULD support the letter class “c” with the following command and events:<br>Proactive command: LAUNCH BROWSER<br>Event download: Browser termination event<br>Event download: Browsing status event |
| --- | --- |
| TS26_NFC_REQ_087.1 | A device which implements Rel-12 or later of ETSI TS 102 223 SHOULD support the letter class “ab” with the following command:<br>Proactive command: LAUNCH BROWSER |
| TS26_NFC_REQ_088 | The device SHALL support the letter class “e” with the following commands and events:<br>Proactive command: OPEN CHANNEL (UICC in client mode and with the support of UDP/TCP bearer)<br>Proactive command: CLOSE CHANNEL<br>Proactive command: RECEIVE DATA<br>Proactive command: SEND DATA<br>Proactive command: GET CHANNEL STATUS<br>Event download: Data available<br>Event download: Channel status |
| TS26_NFC_REQ_088.1 | For OPEN CHANNEL related to Default (network) Bearer, the device SHALL also support an optional Network access name (APN) occurring after the Buffer size.<br>If supplied, the Network Access Name provides information to the device necessary to identify the Gateway entity which provides interworking with an external packet data network. |
| TS26_NFC_REQ_089 | The device SHALL support the letter class “l” with the following command:<br>Proactive command: ACTIVATE |
| TS26_NFC_REQ_090 | The device SHOULD support the letter class “m” with the following command and event:<br>Event download: HCI connectivity event |
| TS26_NFC_REQ_091 | The device SHOULD support the letter class “r” with the following commands and events:<br>Proactive command: CONTACTLESS STATE CHANGED<br>Event download: Contactless state request |
