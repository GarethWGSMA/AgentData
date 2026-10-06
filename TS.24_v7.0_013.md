---
source: "TS.24_v7.0.docx"
chunk_id: 013
section_path:
  - "2.4 Operator Antenna Performance Acceptance Values for 5G NR FR1"
---

## 2.4 Operator Antenna Performance Acceptance Values for 5G NR FR1

The following tables list the Operator Antenna Performance Values per test scenario and frequency band for 5G NR FR1.

Requirements are defined for EN-DC (NSA) and 5G SA.

If a device supports both NSA and SA it’s up to the MNO to request which configuration they would like to test the device.

However, it is recommended for test optimization perspective to perform the full OTA test (TRP and TRS) in SA mode and in addition to test TRP at a mid-channel in EN-DC mode.

TRP requirements for PC3 are defined for all NR bands listed in this document.

Although 3GPP has not yet defined PC2 conducted values for the FDD bands, TRP requirements have been defined for PC2 in all FDD bands listed in this document.

Test scenario:

Head and Hand (BHH):

Relevant for devices that support voice (e.g., VoIP, VoNR). The relevant hand phantom is to be used according to the device’s width:

PDA hand is used for testing devices with widths 56 – 72 mm.

Wide Grip hand is used for testing devices with widths >72 - 92 mm.

The values are relevant for left or right hand.

Browsing (HL or HR):

Relevant for devices where the display is visible to the end user for data usage and relevant hand phantom to be used according to the device’s width:

PDA hand is used for testing devices with widths 56 – 72 mm.

Wide Grip hand is used for testing devices with widths >72 - 92 mm.

The values are defined considering one-hand only and are relevant for left or right hand.

Note 4: Head and hand phantoms used for 2G/3G/LTE bands can also be used for the defined NR bands in this document.

Free Space:

Relevant for any device that embeds an antenna and supports voice (e.g., VoIP, VoNR) and /or data.

These acceptance values include measurement uncertainty.

Settings during testing

TRP:

Single antenna transmitting.

Option A: Max Tx power on NR, min Tx power on LTE (10 dBm regardless of device’s PC for NR band).

Option B: Tx Power equally shared between LTE and NR (EPS).

TRS:

All receivers/antennas active.

Bandwidth: see table

Converting a measured TRS value with BW1 to a TRS value with BW2 is possible:

= 10*log(BW2/BW1)

Example:  BW1= 100 MHz; BW2 = 20 MHz

 = 10*log(20/100) = -7 dB

-86 dBm @ (100 MHz)  -93 dBm @ (20 MHz)

| NR FR1 Frequency Band | GSMA Operator Acceptance Values for TRP [dBm] in EN-DC Mode for PC3 | GSMA Operator Acceptance Values for TRP [dBm] in EN-DC Mode for PC3 | GSMA Operator Acceptance Values for TRP [dBm] in EN-DC Mode for PC3 | GSMA Operator Acceptance Values for TRP [dBm] in EN-DC Mode for PC3 | GSMA Operator Acceptance Values for TRP [dBm] in EN-DC Mode for PC3 | GSMA Operator Acceptance Values for TRP [dBm] in EN-DC Mode for PC3 |
| --- | --- | --- | --- | --- | --- | --- |
| NR FR1 Frequency Band | BHH (Note 4) | BHH (Note 4) | Browsing (Note 4) | Browsing (Note 4) | Free Space | Free Space |
| Option | A | B | A | B | A | B |
| N1 | 14 | 12 | 16 | 14 | 18.5 | 16.5 |
| N3 | 14 | 12 | 16 | 14 | 18.5 | 16.5 |
| N5 | 10.5 | 8.5 | 14.5 | 12.5 | 18.5 | 16.5 |
| N7 | 14 | 12 | 16 | 14 | 18.5 | 16.5 |
| N8 | 10.5 | 8.5 | 14.5 | 12.5 | 18.5 | 16.5 |
| N20 | 10.5 | 8.5 | 14.5 | 12.5 | 18.5 | 16.5 |
| N26 | 10.5 | 8.5 | 14.5 | 12.5 | 18.5 | 16.5 |
| N28 | 10.5 | 8.5 | 14.5 | 12.5 | 18.5 | 16.5 |
| N40 | 14 | 12 | 16 | 14 | 18.5 | 16.5 |
| N77 | 14 | 12 | 16 | 14 | 18.5 | 16.5 |
| N78 | 14 | 12 | 16 | 14 | 18.5 | 16.5 |
