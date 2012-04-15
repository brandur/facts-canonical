Cross-site Request Forgery (CSRF)
=================================

* Malicious exploity whereby unauthorized commands are transmitted from a user that the website trusts. Unlike XSS, which exploits the trust a user has for a site, CSRF exploits the trust that a site has in a user's browser.
* About 18 million users of eBay's Auction.co.kr in Korea lost personal information in February of 2008 due to a CSRF attack.
* Example: (1) Bob is browsing a chat forum, (2) Mallory has posted a message including an HTML image element that references the withdraw action on Bob's bank's website, and (3) if Bob's authentication is still valid, the withdraw executes as he loads the image.
* Limitations: (1) must target either a site that doesn't check referrer header (common), or a victim with a browser or plugin that allows referrer spoofing, (2) attacker must find a form submission or URL with side effects, (3) attacker must determine the right values for all the form/URL's inputs, if any are secret authentication values or unguessable, the attack fails, and (4) the victim must be lured to a site with malicious code injected while the victim is authenticated for the target site.
** **DO NOT UPDATE CONTENT BELOW THIS LINE** **

