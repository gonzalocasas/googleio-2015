User reaction to notification permissions:
 - 53% ignored permission requests on Chrome
 - 25% dismissed it

Some new Chrome APIs:
 - notifications
 - background sync
 - bluetooth for web (!)

What Chrome is doing about permissions:
 - Permission requests were made easier to spot and find. Instead of grey bar, now a 'permission bubble' that hangs offs of the lock in the URL bar.
 - Easier to *Undo* permissions granting/blocking (both mobile and desktop Chrome)

How to ask for permission:
 - Use HTTPS! Access to new APIs will ONLY be available via HTTPS to prevent abuse
 - Ask the permission in context
 - New API to check permission status coming to Chrome
 - Handle user rejection, people change their minds (e.g. grey out mic icon if user rejected permission). Two ways to do it:
   - Check API callbacks for success/failure
   - Or, use the new permissions API and listen for failure
 - Ask with a document, i.e. don't ask permissions on background tasks.

More info: 
 - html5rocks.com - permissions API for the web
 - TLS all the things on youtube