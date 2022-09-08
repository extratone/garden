---
{"dg-publish":true,"permalink":"/snippets/remove-facebook-sponsored-js/","dgHomeLink":true,"dgPassFrontmatter":false}
---

# remove-facebook-sponsored.js

---
// ==UserScript==
// @name         Remove Facebook Sponsored Elements
// @namespace    http://tampermonkey.net/
// @version      0.1.1
// @description  Remove Facebook Sponsored Elements
// @author       You
// @match        https://www.facebook.com/
// @icon         https://www.google.com/s2/favicons?sz=64&domain=tampermonkey.net
// @grant        none
// @run-at       document-idle

// ==/UserScript==

(function() {
    'use strict';

    // Your code here...
    // get all elements with href that container fbclid
    const getFbAdElementsAndBlock = () =>{
        const elements = document.getElementsByTagName('a');
        const adElements = [];
        for (const element of elements) {
            if (element.href.indexOf('fbclid') > -1 || element.href.indexOf('l.php') > -1) {
                adElements.push(element);
            }
            const isMainPageSponsored = (element) => element.href.indexOf('fbclid') > -1;
            const isMarketplaceSponsored = (element) => window.location.href.indexOf('marketplace/') > -1 && element.href.indexOf('l.php') > -1;
            if (isMainPageSponsored(element) || isMarketplaceSponsored(element)) {
                adElements.push(element);
            }

        }
        for (const element of adElements) {
            element.style.display = 'none';
        }
        setTimeout(getFbAdElementsAndBlock, 3000);

    }

    getFbAdElementsAndBlock();
})();

Tags:
  block, js, snippets, userscripts