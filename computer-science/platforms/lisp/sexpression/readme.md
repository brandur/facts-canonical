S-expression
============

* List-based data structures that represent semi-structured data. May be a nested list of smaller S-expressions. e.g. `(= 4 (+ 2 2))`
* Popular use in Lisp and its derivation, and markup in IMAP.
* Lisp uses "prefix notation" or "Cambridge Polish notation", where the first element of every S-expression is an operator and remaining elements are data.
* Lisp constructs S-expressions from **cons pairs** so a list that looks like `(1 2 3)` is actually `(1 . (2 . (3 . nil)))` (where `nil` acts as a list terminator).

