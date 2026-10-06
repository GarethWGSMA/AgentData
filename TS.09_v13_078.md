---
source: "TS.09_v13.docx"
chunk_id: 078
section_path:
  - "8.1 HTML Browsing"
---

## 8.1 HTML Browsing

Description

The GSMA have created a web page containing text and an image that automatically refreshes every 20 s. By ‘refreshes’ it is meant that the page contains appropriate HTML instructions so as to force the browser to completely reload the page and image every 20 s.

Initial configuration

To execute the test download the HTML test page and its associated files from the GSMA website as described in section 2 and load it onto your own local web server that is accessible to the terminal. The test should not be run from the GSMA web server because it is not configured to act as a test server.

Test procedure

To run the test, enter the URL of the web page into the browser. The complete test page and image should now be automatically refreshed by the browser every 20 s until the browser is closed.

For the duration of this test, the backlight shall be lit. If this does not happen automatically because of the page update then it must be forced by other means. For example it may be possible to set this in the options, or it can be achieved by manually pressing a key. The method used must be indicated in the test results.

Measure the current for five minutes as defined in section 3

NOTE:

- Using HTML <meta> tags to control the browser caching is not a reliable way. Some browsers may ignore the <meta> tags for cache control.
- When using HTML <meta> tags to control the refresh timer the timer will start counting from the time when the page is loaded. Since the page loading time is a variable for different solutions, the number of page loading iterations in the 5 min measurement time is not fixed.
- If the test is performed in a WCDMA network, the refresh duration of 20 s might not be long enough to allow the HSPA modem to ramp down from DCH to FACH to IDLE (for certain network configurations)
