---
source: "TS.26_v15.1.docx"
chunk_id: 018
section_path:
  - "6.2 Core Required NFC Features"
---

## 6.2 Core Required NFC Features

| TS26_NFC_REQ_006 | The NFC controller SHALL support SWP (Single Wire Protocol) interface with the UICC as per ETSI TS 102 613. |
| --- | --- |
| TS26_NFC_REQ_173 | A device MAY be shipped with an eSE for NFC services. |
| TS26_NFC_REQ_173.1 | The NFC controller SHALL support an interface with the eSE.<br>Note: The interface can be SWP or any other interface. |
| TS26_NFC_REQ_007 | The NFC controller SHALL support HCI with the UICC as per ETSI TS 102 622. |
| TS26_NFC_REQ_164 | For devices with more than one UICC slot, the NFC controller SHALL support SWP and HCI interface with at least one UICC slot of the device as per ETSI TS 102 613 and ETSI TS 102 622. |
| TS26_NFC_REQ_164.1 | For devices with more than one NFC capable UICC slot, there SHALL only be one NFC capable UICC slot active at any one time. |
| TS26_NFC_REQ_164.2 | Each NFC capable UICC slot SHALL be indicated to the user. |
| TS26_NFC_REQ_164.3 | For devices with more than one NFC capable UICC slot, a menu SHALL give the option to the user to select on which NFC capable UICC slot, NFC is active. |
| *TS26_NFC_REQ_165 | If the device has both an eUICC and a UICC slot the device SHALL implement the NFC card emulation on both. |
| TS26_NFC_REQ_166 | The device SHALL send the Terminal Capability command to the UICC indicating that the UICC-CLF interface (SWP) is supported as per ETSI TS 102 221. |
| TS26_NFC_REQ_008 | Contactless tunnelling (CLT=A) mode SHALL be supported for SWP (per ETSI TS 102 613). |
| TS26_NFC_REQ_009 | VOID |
| TS26_NFC_REQ_009.1 | Contactless tunnelling (CLT=F) mode SHALL be supported for SWP (per<br>ETSI TS 102 613). |
| TS26_NFC_REQ_010 | The device interface with UICC SHOULD support Class B. |
| TS26_NFC_REQ_011 | The device interface with UICC SHALL support Class C. |
| TS26_NFC_REQ_012 | VOID |
| TS26_NFC_REQ_137 | The NFC controller interface with UICC SHALL use ETSI TS 102 613 full power mode when the device is in battery operational mode. |
| TS26_NFC_REQ_013 | VOID |
| TS26_NFC_REQ_154 | The NFC controller interface with UICC MAY use ETSI TS 102 613 full power mode when the device is in battery low mode. |
| TS26_NFC_REQ_138 | The NFC controller interface with UICC MAY use ETSI TS 102 613 full power mode in battery power-off mode. |
| TS26_NFC_REQ_139 | If the NFC controller interface with UICC is not supporting ETSI TS 102 613 full power mode in battery low mode, then the NFC Controller SHALL support ETSI TS 102 613 low power mode when the device is in battery power-low mode. |
| TS26_NFC_REQ_140 | If the NFC controller interface with UICC is not supporting ETSI TS 102 613 full power mode in battery power-off mode, then the NFC Controller SHALL support ETSI TS 102 613 low power mode when the device is in battery power-off mode. |
| TS26_NFC_REQ_107 | The device manufacturer SHALL provide information to the user about the position of the NFC antenna reference point.<br>Examples: a marker on the device, a removable sticker, a device user manual or a tutorial that is started when activating NFC for the first time. |
| TS26_NFC_REQ_014 | The device interface with UICC SHALL support DEACTIVATED followed by subsequent SWP interface activation in full power mode. |
| TS26_NFC_REQ_015 | The NFC controller SHOULD support both windows size set to 3 and set to 4. |
| TS26_NFC_REQ_016 | VOID |
| TS26_NFC_REQ_017 | The NFC controller SHALL ensure that the UICC SWP/HCI initialization is finished before deactivating the SWP without full power down UICC.<br><br>Note: The SWP/HCI specification is not integrating a recovery mechanism so in case of SWP line deactivation in the middle of the activation, it may lead to blocking situation, with SWP-UICC interface not usable until the next device boot. |
| TS26_NFC_REQ_018 | VOID |
| TS26_NFC_REQ_019 | The NFC Controller SHALL support configuration of the listen mode routing for Card Emulation, by the device manufacturer or operator, for at least ISO DEP, NFCA, NFCB & NFCF. |
| TS26_NFC_REQ_020 | If NFC was enabled, when the mobile device is automatically switched off, and enters battery low mode, the mobile device SHALL be able to perform 15 transactions in card emulation within the following 24 hours. |
| TS26_NFC_REQ_174 | If NFC was enabled when the device is switched off by the user, the device SHALL be able to perform card emulation transactions. |
| TS26_NFC_REQ_021 | If NFC is enabled, NFC transactions SHALL be possible in battery low mode.<br>Note: This is important for public transport services. |
| TS26_NFC_REQ_167 | The NFC controller SHALL support at least 16 AIDs of 16 bytes in the routing table. |
| TS26_NFC_REQ_167.1 | The NFC controller SHOULD support at least 40 AIDs of 16 bytes in the routing table. |
| TS26_NFC_REQ_175 | In case the NFC Controller receives a RF parameters configuration request from a CEE enabling a Mifare Classic service with either UID 4 or 7 bytes, the corresponding RF parameters profile “Profile 2 ” as defined in chapter 3.1.2.2 of GSMA SGP.12 SHALL apply |
| TS26_NFC_REQ_176 | In case the NFC Controller receives a RF parameters configuration request from a CEE enabling a Mifare DESFire service, the RF parameters profile “Profile 3” as defined in chapter 3.1.2.2 of GSMA SGP.12 SHALL apply |
| TS26_NFC_REQ_177 | In other cases, the RF parameters profile “Profile 1” as defined in chapter 3.1.2.2 of GSMA SGP.12 SHALL apply |
