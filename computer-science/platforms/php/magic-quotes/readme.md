Magic Quotes
============

* Single quotes, double quotes, backslashes, and null characters would have a backslash prepended in any data accessed from `$_GET`, `$_REQUEST`, `$_POST`, or `$_COOKIE`.
* Used `addslashes` in the backend, which wasn't unicode aware and still subject to SQL injection vulnerabilities in some multi-byte character encodings.
** **DO NOT UPDATE CONTENT BELOW THIS LINE** **

