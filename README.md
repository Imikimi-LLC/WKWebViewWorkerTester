# WKWebViewWorkerTester

How can I start a local webworker? I have succeeded by creating a DATAURI and starting a local web-worker that way, but that is inconvenient.

### Details

This project starts up the simplest instance of WKWebView and points it to the local ```index.html``` asset. Index.html has a button which attempts to start the webworker specified by ```echo_worker.js```.

If you attach Safari to the WKWebView before pressing the "start worker" button, you can see the following error:

> SecurityError: DOM Exception 18: An attempt was made to break through the security policy of the user agent.

If you click the second button.

> XMLHttpRequest cannot load file:///Users/[...]/WKWebViewTester.app/www/echo_worker.js. Cross origin requests are only supported for HTTP.

#### Local Assets

* www/index.html
* www/echo_worker.js
