# journal-redirector
Redirect journal websites to the proxy server of your institution in Chrome. E.g., https://onlinelibrary.wiley.com/doi/10.3982/ECTA15510 → https://onlinelibrary-wiley-com.ezproxy.bu.edu/doi/10.3982/ECTA15510.

When you Google or click on a link to a paper (e.g., http://www.aeaweb.org/articles.php?doi=10.1257/mic.3.2.114), more often than not, you are unable to download it directly even though your institution has a subscription (worse still, Institutional Login/Access through your Institution option often won't work). This method saves you the hassle of searching it again on your institution's library or proxy server.

- Step 1: Download the Redirector extension from the Chrome web store: https://chrome.google.com/webstore/detail/redirector/ocgpenflpmgnfapjedencafcfakcekcd (Add to Chrome).
- Step 2: Download Redirector.json from this repo.
- Step 3: Replace all "ezproxy.bu.edu" with the suffix of your institution, e.g., "libproxy.berkeley.edu," which can be found by browsing the journal website from your institution's library.
- Step 4: Import this JSON file to the Redirector extension by clicking on it (located at the top-right corner) and then choosing "Edit Redirect" and "Import."

Finally, Try clicking on some links given above and see if they are redirected properly.

Currently, it can redirect papers on all AEA journals, JPE, RES and QJE (Academic OUP), ECTA (Wiley), and NBER. Elsevier Journals (e.g., JET, GEB) are not included because the "Access through your institution" option works well.

