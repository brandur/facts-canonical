Cross-site Scripting (XSS)
--------------------------

* By injecting malicious scripts into web pages, an attacker can gain elevated access privileges to sensitive page-content, session cookies, and data maintained by the browser on behalf of the user.
* Types are (1) **non-persistent**: data provided by a client through HTTP parameters or form submission, is used immediately by server-side scripts within the rendered page without sanitization, and (2) **persistent**: data provided by an attacker is saved by the server, and then permanently displayed on "normal" pages seen by other users.
* Example of non-persistent attack: (1) Alice often visits a website hosted by Bob that stores sensitive data, (2) Mallory observes an XSS vulnerability in Bob's site, (3) Mallory crafts a URL to exploit the vulnerability and e-mails it to Alice, enticing her to click the link, (4) Alice visits the URL while logged into Bob's site, and (5) payload executes in Alice's browser as if it came directly from Bob's server, sending Alice's session cookie to Mallory.
* Example of persistent attack: (1) Mallory posts a message with malicious payload to a social network, (2) Bob reads the message, Mallory's XSS steals Bob's cookie, and (3) Mallory can now hijack Bob's session.
* XSS carried out on websites accounted for roughly 80% of all security vulnerabilities documented by Symantec as of 2007.
