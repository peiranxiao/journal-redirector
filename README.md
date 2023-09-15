# journal-redirector
Automatically redirect journal websites to access papers through your institution’s proxy. E.g., https://onlinelibrary.wiley.com/doi/10.3982/ECTA15510 → https://onlinelibrary-wiley-com.ezproxy.bu.edu/doi/10.3982/ECTA15510.

## Motivation
When you click on a link to a paper from Google or a PDF, more often than not, you get paywalled even though your institution *has* access to the journal. Worse still, the ``Institutional Login`` option usually won't work, as your institution is somehow not on the list. This redirector automatically redirects you to access the papers through your institution’s proxy. 

## How to use
Initial configuration:
- Step 1: Download the Redirector extension from the Chrome web store (offered by Einar Egilsson): https://chrome.google.com/webstore/detail/redirector/ocgpenflpmgnfapjedencafcfakcekcd (Add to Chrome).
- Step 2: Download ``Redirector.json`` from this repo that contains the journal websites to redirect.
- Step 3: Replace all ``ezproxy.bu.edu`` in the JSON file with the prefix of your institution's proxy server, e.g., ``libproxy.berkeley.edu`` or ``libproxy.mit.edu``, which can be found by accessing the journal website from your institution's library.
- Step 4: Import this JSON file to the Redirector extension by clicking on its icon (located at the top-right corner) and then choosing "Edit Redirect" and "Import."

Try clicking on the links given below to see if they are redirected properly:
https://onlinelibrary.wiley.com/doi/10.3982/ECTA15510, http://www.aeaweb.org/articles.php?doi=10.1257/mic.3.2.114, https://www.journals.uchicago.edu/doi/10.1086/710560, https://www.nber.org/papers/w28583. 

Currently, it can redirect papers on all AEA journals, Academic OUP (e.g., RES, QJE, JEEA), Wiley (e.g., ECTA, RAND), JPE, JSTOR, NBER, etc. Elsevier journals (e.g., JET, GEB) don't need this because the *Access through your institution* option works well.

## Alternative methods
Recently, I found the Zotero extension also does the job, but its configuration is less programmable as it does not support JSON import.

Moreover, the EZProxy Redirect extension (https://chrome.google.com/webstore/detail/ezproxy-redirect/gfhnhcbpnnnlefhobdnmhenofhfnnfhi) works similarly. One needs to configure the institution(s) first and click on the extension *every time* to redirect websites. It is a good complement to Redirector (particularly useful if you have multiple institutional accounts) though, and I use it as an ad hoc method to redirect websites not on my list. 