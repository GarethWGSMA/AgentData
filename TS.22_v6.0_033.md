---
source: "TS.22_v6.0.docx"
chunk_id: 033
section_path:
  - "1.1.2. (U)SIM based EAP methods error handling"
---

## 1.1.2. (U)SIM based EAP methods error handling

The (U)SIM based EAP methods (EAP-SIM, EAP-AKA and EAP-AKA’) define various error codes for terminal authentication, as AT Notification Codes [RFC 4186/RFC 4187]. The following table defines terminal behaviour for these codes:

| AT Notification Code | Description | Terminal Behaviour |
| --- | --- | --- |
| 0 | General failure after authentication | Advise user about error indicating that authentication has succeeded but error occurred afterwards. User is advised to check with service provider about their subscription. |
| 1026 | User has been temporarily denied access | Advise user about error and prompt for retry or automatically retry within MAX_RETRY_VALUE. The default value shall be “Retry every 20 seconds up to 3 attempts”. |
| 1031 | User has not subscribed to the requested service | Advise user about error, for example remediation, and provide assistance about their subscription. Also see section 7.3. |
| 16384 | General failure | Advise user about error. |
| 32768 | Success | Authentication is successful. |
