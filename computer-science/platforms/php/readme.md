PHP
===

* Installed on more than 20 million websites.
* PHP is a recursive algorithm for _PHP: Hypertext Preprocessor_. Before PHP 3, it represented _Personal Home Page_.
* Written by Danish/Greenlandic programmer Rasmus Lerdorf to maintain his personal homepage. He released it in 1995.
* Israeli developers Zeev Suraski and Andi Gutmans rewrote the parser that formed PHP 3 in 1997, and launched it in 1998.
** **DO NOT UPDATE CONTENT BELOW THIS LINE** **

Magic Quotes
------------

* Single quotes, double quotes, backslashes, and null characters would have a backslash prepended in any data accessed from `$_GET`, `$_REQUEST`, `$_POST`, or `$_COOKIE`.
* Used `addslashes` in the backend, which wasn't unicode aware and still subject to SQL injection vulnerabilities in some multi-byte character encodings.

Opcode Cache
------------

* Cache the compiled form of PHP scripts (opcodes) in shared memory to avoid parsing and compilation overhead every time the script runs.
* APC (Alternative PHP Cache) will be included in a future version of PHP.

