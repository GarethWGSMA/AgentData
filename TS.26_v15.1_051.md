---
source: "TS.26_v15.1.docx"
chunk_id: 051
section_path:
  - "7.3.3.1 Multiple Active CEE model"
---

## 7.3.3.1 Multiple Active CEE model

| TS26_NFC_REQ_094 | When a mobile application is registering an AID-based or non AID-based service (statically or dynamically) it SHALL be able to state the target CEE using an OS mechanism (manifest, API, …). |
| --- | --- |
| TS26_NFC_REQ_094.1 | Before Android 10, the following extension SHALL be supported in the manifest<br><br><extensions xmlns:android="http://www.gsma.com" android:description="@string/servicedesc"><br>     <se-ext-group><br>          <se-id name="XXX" /><br>     </se-ext-group><br><AID-based>boolean</AID-based><br></extensions><br><br>Where:<br>se-id name SHALL be set as described in TS26_NFC_REQ_069 and TS26_NFC_REQ_070 ; the uniqueness of the naming SHALL be ensured by the OS as described in TS26_NFC_REQ_144.<br>-	For se-id name field, following values SHALL be accepted by the device:<br>	-	“SIM” and “SIM1” for SIM slot 1<br>-	“eSE” and “eSE1” for embedded Secure Element 1<br>AID-based SHALL be set to true in case a SE application is compliant with ISO 7816-4 and false in all other cases<br>Note: When a mobile application is declaring a se-id name that is not existing on the device the registration shall be ignored. |
| TS26_NFC_REQ_094.2 | Before Android 10, if the extension is not declared in the manifest of the application, then the following default values SHALL apply (for backward compatibility):<br><se-id name=”SIM1”/><br><AID-based>true</AID-based> |
| TS26_NFC_REQ_094.3 | From Android 10 onwards, it SHALL support the definition of the target Offhost CEE from the manifest of the application<br>Note: In Android 10 this is achieved using the following tag in the OffHostApduService description<br><attr name="secureElementName"/><br><br>Note: See Annex B for documented usage the feature name may change in any future release of Android, please check Android developer documentation for updates. |
| TS26_NFC_REQ_094.4 | From Android 10 onwards, if the tag  is not declared in the service declaration of the manifest of the application, then it SHALL be interpreted as SIM1 (for backward compatibility) |
| TS26_NFC_REQ_094.5 | From Android 10 onwards, it SHALL be possible to define (set & unset) the target Offhost CEE using APIs defined by Android<br><br>Note: In Android 10 the APIs are named like stated below but the naming may change in any future release of Android, please check Android developer documentation for updates.<br>CardEmulation.setOffHostForService(serviceName, offhostName)<br>CardEmulation.unsetOffHostForService (serviceName) |
| TS26_NFC_REQ_133 | The device SHALL support an OS mechanism that allows applications to statically register NFC application by list of AIDs.<br>Note: this requirement fulfils the generic requirement TS26_NFC_REQ_061. |
| TS26_NFC_REQ_127 | VOID |
| TS26_NFC_REQ_127.1 | VOID |
| TS26_NFC_REQ_127.2 | VOID |
| TS26_NFC_REQ_128 | VOID |
| TS26_NFC_REQ_128.1 | VOID |
| TS26_NFC_REQ_128.2 | VOID |
| TS26_NFC_REQ_128.3 | VOID |
| TS26_NFC_REQ_134 | The device SHALL provide an additional menu entry in “Settings” in order to enable/disable group of AIDs (as defined by Android) belonging to the category “Other”.<br>A group of AIDs SHALL only be enabled/disabled as a single unit.<br><br>This requirement is optional if TS.26_NFC_REQ_167.1 is supported. |
| TS26_NFC_REQ_134.1 | When there is an overflow in the NFC router table, the menu entry SHOULD display:<br>A banner representing the groups of AIDs belonging to the category “Other” (and optionally the group description) with its current status (enabled/disabled) and a way for disabling/enabling it<br>A visual indication representing the NFC Controller capacity and showing<br>The space used by the selected group<br>If enablement of the selected group can fit with the remaining space of the NFC Controller routing table |
| TS26_NFC_REQ_134.2 | The menu entry SHOULD be hidden to the end user until the first time a NFC Service cannot be added in the NFC Controller routing table |
| TS26_NFC_REQ_134.3 | When the menu entry is opened, the status of NFC services group displayed by the menu entry SHALL reflect the actual status of the current NFC Controller routing table. |
| TS26_NFC_REQ_134.4 | When there is no overflow in the NFC routing table and if the menu entry is available to the end user, the menu SHOULD not allow the end user to disable the AID groups. |
| TS26_NFC_REQ_172 | The device SHALL consider that non-AID based services are conflicting as soon as they are associated to different Off-Host entities. |
| TS26_NFC_REQ_170 | In case the device detects a conflict between non-AID based contactless services (see TS26_NFC_REQ_172), the device SHALL display a menu entry in “Settings” in order to list impacted contactless services and the user SHALL be directed to the menu. |
| TS26_NFC_REQ_170.1 | The menu entry SHALL present the conflicting services to the end user with an option to select which service(s) to be active. Only one set of service(s) (which are not conflicting with each other) SHALL be active at any one time. |
| TS26_NFC_REQ_170.2 | The menu entry SHOULD be hidden to the end user in case there is no conflicting services. |
| TS26_NFC_REQ_170.3 | VOID |
| TS26_NFC_REQ_171 | VOID |
| TS26_NFC_REQ_180 | If the end user changes the default non-AID based contactless service via the menu described in TS26_NFC_REQ_170, the device SHALL reconfigure the NFC Controller with the contactless parameters configured in the Off-Host linked to the newly activated service. |
| TS26_NFC_REQ_135 | When an application is trying to register new AIDs belonging to the category “Other” and there is no automatic solution to solve any routing table overflow (as defined in REQ_143), the device SHALL:<br>Inform the end user that some NFC Services proposed by the application cannot be used. A message SHALL provide the description of the group(s) of AIDs (android:description) which cannot be activated<br>Propose the end user should disable some previously installed NFC services using the feature described in TS26_NFC_REQ_134 in order to free some NFC Controller routing table space to be able to register all AIDs needed by the current application<br>When one AID from a group of AIDs cannot be added in the NFC Controller routing table, the entire group of AIDs SHALL not be enabled. |
| TS26_NFC_REQ_136 | When a customer is selecting a service from the “Tap&Pay” menu and there is no automatic solution to solve any routing table overflow (as defined in REQ_143), the device SHALL:<br>Inform the end user that activation of the selected NFC services cannot be performed<br>Propose the end user should disable some previously installed NFC services using the feature described in TS26_NFC_REQ_134 in order to free some NFC Controller routing table space<br>If the end user doesn’t disable enough NFC services to allow activation of the selected “Tap&Pay” menu, previous “Tap&Pay” entry SHALL stay active and the end users selection is cancelled.<br>This requirement is optional if TS.26_NFC_REQ_167.1 is supported. |
| TS26_NFC_REQ_147 | In the “Tap&Pay” menu, the user selection has precedence and the behaviour of the device is consistent across different handset states.<br>The following scenarios SHALL be applied.<br><br>Note 1: If Android is changing the behaviour then this requirement will change accordingly.<br><br>Note 2: GSMA strongly recommend that service providers register the Off-Host AIDs in the Android OS as defined by Android. |
| TS26_NFC_REQ_148 | The device SHALL not change the default AID route in response to changes in device state (such as screen off, power off). |
| TS26_NFC_REQ_148.1 | The same behaviour SHALL be implemented when the mobile device is set in Flight Mode with NFC ON. |
