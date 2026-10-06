---
source: "TS.26_v15.1.docx"
chunk_id: 066
section_path:
  - "11 Android Wear Operating System"
---

## 11 Android Wear Operating System

Document Management
Document History

| Ver. | Date | Brief Description of Change | Approval Authority | Editor / Company |
| --- | --- | --- | --- | --- |
| 1.0 | July 2011 | First draft submitted to DAG and PSMC for approval | PSMC and NFC (Rejected at PSMC level) | Sameer Tiku, Vodafone |
| 2.0 | November 2011 | Second draft incorporating PSMC feedback submitted to DAG and PSMC for approval | PSMC and NFC (V2.0 Approved and published) | Sameer Tiku, Vodafone |
| 3.0 | 03 October 2012 | Submitted to DAG and PSMC for 7 day Committee Email approval | PSMC and NFC | Sameer Tiku, Vodafone |
| 4.0 | 17 September 2013 | Re-Submitted to DAG and PSMC for approval following comments received from PSMC | PSMC and NFC | Sameer Tiku, Vodafone |
| 4.1 | 6 November 2013 | Corrected and updated namespace to <com.gsma.services.nfc>.<br>Impacted sections: 4.9, 4.10 | Terminal Steering Group | Katrin Jordan,<br>DT / TSG |
| 5.0 | 12th  March 2014 | Implemented updates to: Title, Introduction, Abbreviations, Terms of Definitions, References, Doc. structure, Figures, Requirements across the document and API specifications. Added a new numbering scheme and provided editorial updates. Marked requirements still work in progress. Removed Annexes and requirements/references as applicable. | Terminal Steering Group | K.Jordan (DT) |
| 6.0 | 21 July 2014 | Implemented updates to: Introduction, Abbreviations, Definitions of Terms, References, Figures, Core Required NFC Features, Secure Element Access & Multiple Secure Elements Management, UI Application triggering requirements, UICC Remote Management, Security, SCWS support, Card Application Toolkit Support, Platform Dependent Properties, Android and Blackberry OS specific sections.<br>Removed majority of yellow markings where req. could be confirmed.<br>Removed Android API details and provided updated API details as separate Javadoc with Readme file.<br>Implemented further formatting and quality updates. | Terminal Steering<br>Group | K.Jordan, G.Printemps, DT |
| 7.0 | 23 March 2015 | Extra document release to address 2 critical issues: 1) ambiguity of the requirement 114 and 2) full AID routing table issue when installing new application on Android devices. | Terminal Steering Group | Radomír Věncek, DT |
| 8.0 | 13 October 2015 | General update based mainly on feedback from the NFC Handset Test Book, changes across the whole document. Includes also initial changes related to transport industry – accepted NFC Forum specifications as a baseline for device testing. Added new requirements as well as modified existing ones. | Terminal Steering Group | Radomír Věncek, DT |
| 9.0 | 01 April 2016 | General update fixing some known issues, removing empty OS sections (Blackberry, Windows Phone), adding few new requirements. | Terminal Steering Group | Radomír Věncek, DT |
| 10.0 | 05 December 2016 | General update amending some existing requirements and adding few new requirements. | Terminal Steering Group | Ruben Rico, Vodafone |
| 11.0 | 12 June 2017 | General update, adding eSE and Wearables as part of the document. GSMA API is marked as deprecated from this version. | Terminal Steering Group – TSG#28 | Anders Olsson, Sony Mobile |
| 12.0 | 05 December 2017 | General update, next step in deprecating GSMA APIs. Adding clarifying requirements for Dual SIM and eSE. | Terminal Steering Group – TSG#30 | Anders Olsson, Sony Mobile |
| 13.0 | 04 June 2018 | This version includes the following changes:<br>Android 9 impacted requirements have been updated and some new requirements have been introduced to support the Android 9 implementation.<br>Single CEE (Card Emulation Environment) requirements have been Voided as this is not relevant anymore.<br>Multiple UICC “slots” – 1 updated requirement on NFC capability for multiple UICC/eUICC slots.<br>GSMA APIs: Requirements updated to reflect deprecated GSMA APIs have been made optional and changed from SHOULD to MAY. | Terminal Steering Group | Anders Olsson, Sony Mobile |
| 14.0 | 4th December 2018 | This version is implementing the following changes:<br>NFC Forum Type 5 Tag requirement is introduced.<br>NFC Forum Type 1 Tag requirement is removed.<br>NFC transaction in Battery Power-Off Mode is removed.<br>AID Routing Table Overflow support in device menu made optional if more than 40 AIDs are supported.<br>Requirements for GSMA API are removed (Void). (Previously they were MAY and deprecated). The property to return version numbering removed.<br>Document Cross Reference updated with reference to newer specifications.<br>Including reference to NFC Forum Technical Specification Release which identifies the version of specific NFC Forum specifications.<br>References to SIMalliance specifications in relation to OMAPI are changed to GlobalPlatform. | Terminal Steering Group | Anders Olsson, Sony Mobile |
| 15.0 | 19 June 2019 | This version is implementing the following changes:<br>6 new requirements<br>2 updated requirements<br>12 removed requirements.<br>Summary of changes:<br>Android 10 supported by TS.26.<br>5 new Android 10 related requirements introduced:<br>1. New Android 10 related requirements for registering NFC services to a specific SE for AID based services (REQ_094.3, REQ_094.4, REQ_094.5).<br>2. New Android 10 related requirements for the Device to declare support of Card Emulation for UICC and eSE (REQ_193, REQ_194). Supporting new Android 10 API.<br>Requirements for devices implementing Android versions before Android 9 have been removed. Devices shall implement Android 9 or later version of Android.<br>Transaction Event: Clarification of expected behaviour for Transaction Event (New REQ_084.1).<br>AID naming: Clarification how the AID in NFC transaction events is specified in relation to lower/upper case hexadecimal usage (Section 7.4).<br>Document Cross References updated with reference to newer specifications including. | TSG | Anders Olsson, Sony Mobile |
| 15.1 | Sept 2024 | Updated with CR1019 v01<br>Non Substantial Change | TSG#57 | Andras Talas Comprion |
