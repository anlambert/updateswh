# Update Software Heritage browser extension for Chrome and Firefox

This browser extension checks if a repository visited by the user is archived
and uptodate in Software Heritage.

### What the extension does

A color button on the right of the browser indicates if it is uptodate (green),
in which case clicking on the button opens a tab on the corresponding page of
the archive, missing (grey) or not up to date (yellow), in which case clicking
on the button triggers a save code now request.

A red color indicates that the API request of information for the repository
did not succeed: this happens typically when one is visiting a repository
that is not publicly accessible, and that naturally cannot be archived.

### Getting the extension for your browser

For accessing the latest published version of the extension on the FireFox
Add-ons and on the Chrome Web Store, see the webpage at
https://www.softwareheritage.org/browser-extensions/

### Credits

Many thanks to the Unpaywall extension developers (see
https://unpaywall.org/products/extension): their work has been an essential
starting point for designing and developing this extension.

### Developer information

The code base is meant to be identical between FireFox and Google Chrome.
Due to the ongoing transition to manifest version 3, there is currently
one difference: for FireFox a manifest.json version 2 is provided, but
for Google Chrome one needs to create a package using the version 3
format provided in manifest-v3.json.
