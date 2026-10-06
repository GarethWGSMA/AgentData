---
source: "TS.09_v13.docx"
chunk_id: 079
section_path:
  - "8.2 HTML Browsing For DUTs with Full Web Browsers"
---

## 8.2 HTML Browsing For DUTs with Full Web Browsers

Description

For smartphones with full desktop web page rendering capabilities, the small web page used in section 8.1 is not suitable. This test case therefore uses ETSI’s “Kepler reference page”, which is an approximation of a full web page with pictures and content resembling a representative full web page.

Initial configuration

- Download the ZIP file of the “Kepler reference web page” from http://docbox.etsi.org/STQ/Open/Kepler.
- For the execution of this test case, place the content of the ZIP file in five different folders of a web server so the page and its contents are reloaded instead of taken from the cache of the  DUT during the test.
- Ensure that the web browser’s cache is empty to prevent from locally loading the pages.
- Ensure that the DUT can load the web page in less than 60 s. If the  DUT can’t load the page in this timeframe this test cannot be performed.

Test procedure

1. Open the “index.html” file in the first of the five folders on the web server in the web browser of the DUT. Ensure that the full page is downloaded, including the pictures and the content of the frames.
1. Ensure that the page is fully loaded before proceeding. Afterwards, scroll down the web page, e.g. by using the touch screen, scroll keys, etc.
1. After 60 s after the start of the download, open the “index.html” file at the next location on the web server and ensure that the full page is downloaded, including the pictures and the content of the frames.

NOTE:	By starting the timer at the beginning of the request and NOT after the page has been fully downloaded, it is ensured that the overall test duration is constant, independent from the  DUT’s and the network’s capabilities to deliver the page at a certain speed.

1. Repeat steps 2 and 3 until the page has been loaded five times. The total test time is therefore five minutes.
1. Measure the current for five minutes as defined in section 3.4 or 3.5.
