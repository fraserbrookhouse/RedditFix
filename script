// ==UserScript==
// @name        Hello World
// @namespace   http://notrealdomain.info
// @include     https://*.reddit.com/*
// @version     1
// ==/UserScript==

(function() {
  // (1) Old Reddit Redirect
  var url = location.href;
  if (/(?:new|www)\.reddit\.com\//.test(url)) {
    location.href = url.replace(/(?:new|www)\./, 'old.');
    return;
  }

  // (2) Delete the cookie message
  var x = document.getElementsByClassName("infobar-toaster-container");
  for (var y of x) {
    y.remove();
  }
})();
