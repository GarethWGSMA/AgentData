---
source: "TS.09_v13.docx"
chunk_id: 066
section_path:
  - "4.3 Battery Life Calculation - MIoT"
---

## 4.3 Battery Life Calculation - MIoT

The battery life of DUT can be calculated as follows:

1. Record the battery capacity of DUT as C, the unit is mAh
1. Record the frequency of a data event as fDTE, which means fDTE times per Day. The DUT may perform several data events per day. Each data event can be numbered with i (i=1, 2, 3, …. )

NOTE:	If a data event is not happened every day, the value of fDTE can be Decimals less than 1.

1. Calculate the Battery life according to following formula:

Battery life= C / CDay

If PSM is enabled:

CDay = fDTE1IDTE1TDTE1 + fDTE2IDTE2TDTE2 + …+ IIdleT3342*(fDTE1+fDTE2+…+fDTEi)+IPSMTPSM

TPSM = 24*3600 – [fDTE1TDTE1 + fDTE2TDTE2 + …+ fDTEiTDTEi + T3324*(fTDE1 + fTDE2 + … + fTDEi)] (in seconds)

If PSM is disabled:

CDay = fDTE1IDTE1TDTE1 + fDTE2IDTE2TDTE2 + …+ IIdleTidle

Tidle = 24*3600 – [fDTE1TDTE1 + fDTE2TDTE2 + …+ fDTEiTDTEi] (in seconds)
