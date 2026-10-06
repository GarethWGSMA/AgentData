---
source: "TS.26_v15.1.docx"
chunk_id: 065
section_path:
  - "11 Android Wear Operating System"
---

## 11 Android Wear Operating System

Requirements for Android Wear will be added in a later version of this document.

Implementation/usage help of REQ 94.1 for multi eSE on Android

OffHost Service definition in Android Manifest

<service android:name=".MyserviceOffHost"

android:exported="true"

android:permission="android.permission.BIND_NFC_SERVICE" >

<intent-filter>

<action android:name="android.nfc.cardemulation.action.OFF_HOST_APDU_SERVICE"/>

<category android:name="android.intent.category.DEFAULT"/>

</intent-filter>

<meta-data android:name="android.nfc.cardemulation.off_host_apdu_service" android:resource="@xml/offhost_aid"/>

<meta-data android:name="com.gsma.services.nfc.extensions" android:resource="@xml/nfc_se"/>

</service>

Note: the bold line is a GSMA extension.

com.gsma.services.nfc.extensions = see REQ 094.1

nfc_se XML file content example

<extensions xmlns:android="http://www.gsma.com" android:description="@string/servicedesc">

<se-ext-group>

<se-id name="XXX"/>

</se-ext-group>

<AID-based>boolean</AID-based>

</extensions>

XXX can be : SIM/SIM1, SIM2, eSE/eSE1, eSE2, … (as per requirements TS26_NFC_REQ_070 and 071)

AID-based is set to:

true for Application defining service using AID based (compliant with ISO 7816-4)
false for Application defining service using non AID based (i.e. Mifare, Felica, …)
Implementation/usage hint of REQ 94.3 for multi SE from Android 10

<service android:name=".MyserviceOffHost"

android:exported="true"

android:permission="android.permission.BIND_NFC_SERVICE" >

<intent-filter>

<action android:name="android.nfc.cardemulation.action.OFF_HOST_APDU_SERVICE"/>

<category android:name="android.intent.category.DEFAULT"/>

</intent-filter>

<meta-data android:name="android.nfc.cardemulation.off_host_apdu_service" android:resource="@xml/ apduservice"/>

</service>

XML apduservice content:

<offhost-apdu-service android:description="@string/servicedesc" android: android:secureElementName ="SIM1” xmlns:android="http://schemas.android.com/apk/res/android" />

Note: the bold line is the way to specify the target CEE
