---
source: "TS.09_v13.docx"
chunk_id: 064
section_path:
  - "4.1 General"
---

## 4.1 General

This methodology is given so that the actual capacity of a battery sold with the DUT can be determined.

- The DUT and battery shall be at room temperature prior to making this measurement and charging and discharging shall be performed in a room temperature environment. (UE switched-on)
- The battery pack used in this test shall be new, not previously used. The battery shall be prepared per section 4.
- The battery pack shall be fully charged using the DUT or charger provided with the DUT, following the manufacturer’s charging instructions stated in the user manual.
- If charging is being done in the DUT itself, the DUT shall be camped to the network, see section 7 and otherwise not used.
- It is not strictly required that the charging be stopped exactly when the DUT’s battery meter says that charging is complete but is strongly recommended.
- The battery shall be removed from the terminal and discharged to its End-of-Life at a discharge rate of “C/5”.
- The “End-of-Life voltage” is the voltage below, which the phone will not operate. This voltage will vary with the characteristics of the UE so the UE manufacturer must report this value.

C/5 discharge rate refers a discharge current which is one-fifth that of C where C is the approximate capacity of the battery. For example, a battery of approximately 1000 mAh (milliamp – hour) capacity, C, will be discharged at 200 mA or C/5. If then, the duration of the discharge period is measured to be 4.5 hours, the actual capacity of the battery is 4.5 hours x 200 mA = 900 mAh. The most accurate way to achieve a C/5 discharge rate is to use a programmable current sink. Other means are possible. However, note that if a fixed resistor is used then the current will have to be monitored and integrated (as the battery voltage falls so will the current).
