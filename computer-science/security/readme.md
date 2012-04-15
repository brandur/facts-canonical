Security
========

** **DO NOT UPDATE CONTENT BELOW THIS LINE** **

Cross-site Request Forgery (CSRF)
---------------------------------

* Malicious exploity whereby unauthorized commands are transmitted from a user that the website trusts. Unlike XSS, which exploits the trust a user has for a site, CSRF exploits the trust that a site has in a user's browser.
* About 18 million users of eBay's Auction.co.kr in Korea lost personal information in February of 2008 due to a CSRF attack.
* Example: (1) Bob is browsing a chat forum, (2) Mallory has posted a message including an HTML image element that references the withdraw action on Bob's bank's website, and (3) if Bob's authentication is still valid, the withdraw executes as he loads the image.
* Limitations: (1) must target either a site that doesn't check referrer header (common), or a victim with a browser or plugin that allows referrer spoofing, (2) attacker must find a form submission or URL with side effects, (3) attacker must determine the right values for all the form/URL's inputs, if any are secret authentication values or unguessable, the attack fails, and (4) the victim must be lured to a site with malicious code injected while the victim is authenticated for the target site.

Cross-site Scripting (XSS)
--------------------------

* By injecting malicious scripts into web pages, an attacker can gain elevated access privileges to sensitive page-content, session cookies, and data maintained by the browser on behalf of the user.
* Types are (1) **non-persistent**: data provided by a client through HTTP parameters or form submission, is used immediately by server-side scripts within the rendered page without sanitization, and (2) **persistent**: data provided by an attacker is saved by the server, and then permanently displayed on "normal" pages seen by other users.
* Example of non-persistent attack: (1) Alice often visits a website hosted by Bob that stores sensitive data, (2) Mallory observes an XSS vulnerability in Bob's site, (3) Mallory crafts a URL to exploit the vulnerability and e-mails it to Alice, enticing her to click the link, (4) Alice visits the URL while logged into Bob's site, and (5) payload executes in Alice's browser as if it came directly from Bob's server, sending Alice's session cookie to Mallory.
* Example of persistent attack: (1) Mallory posts a message with malicious payload to a social network, (2) Bob reads the message, Mallory's XSS steals Bob's cookie, and (3) Mallory can now hijack Bob's session.
* XSS carried out on websites accounted for roughly 80% of all security vulnerabilities documented by Symantec as of 2007.

Kerckhoff's Principle
---------------------

* A cryptosystem should be secure even if everything about the system, except the key, is public knowledge.
* Stated by Auguste Kerckhoffs, a Dutch linguist and cryptographer, in the 19th century.

Stuxnet
-------

* First discovered work that spies on and reprograms industrial systems, specifically SCADA (Supervisory Control And Data Acquisition) systems and PLCs (Programmable Logic Controllers).
* Attacks Windows first, and spreads to Siemens' WinCC SCADA software. Once inside a system, it uses default passwords to command the software.
* Includes four zero-day attacks for Windows.
* Represents many man-months and maybe man-years of work. Probably built by a team.
* Digitally signed with two authentic certificates which were stolen from authorities JMicron and Realtek.
* Can upgrade itself via peer to peer if the control server is disabled.
* There has been speculation that it was designed to target nuclear reactors in Iran.

