---
source: "TS.09_v13.docx"
chunk_id: 074
section_path:
  - "7.1 General"
---

## 7.1 General

Data transfer tests of various types are defined in later sections; however, the principles indicated in this section are also applicable to some of the later described tests.

It is recommended that the results of all the packet switched data tests be expressed as total amount of data transferred (in Mb) rather than time spent in the mode – the data transfer total is a more useful indication to the user of what the terminal is capable of and will be very roughly the same regardless of the actual duty cycle seen.

The FTP Download shall be started from a dedicated server of the test file. The size of the file must guarantee a continuous transfer so that the file transfer does not run out during the testing (at least 10 minutes).

The bearer used shall be the most efficient one, and bearer parameters used shall be stated in the test results.

In this test we consider a file download to an external device (e.g. laptop) connected with the DUT via

. Cable
. Bluetooth.
. USB port - data modem

During the test using a cable connection, the DUT should not be powered by the external device via the cable connection. If this kind of charging cannot be disabled by an appropriate SW tool, the cable FTP test is not relevant.

Record the USB standard version number used on the results sheet.

For WLAN the following applies:

The test file shall be located on a dedicated server or PC with network sharing enabled to allow the terminal to access the file via the WLAN.

During the test the terminal shall be in GSM standby.
