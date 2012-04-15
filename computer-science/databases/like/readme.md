LIKE
====

* Can use an index if there is a prefix before the first wildcard. Only the prefix determines the scanned range and is an access predicate. A postfix filter can only remove records that don't match (filter predicate). A postfix search like `%AND`, or an anywhere search like `%NAN%` will scan the entire index.
* Avoid anywhere `LIKE` searches (e.g. `%TERM%`). If inevitable, try to provide another access path to the selected rows. If no other access path is available, consider using a full text index.
* `LIKE` is no adequate way to implement full text searches. Most databases offer a special purpose index for that (e.g. `MATCH` and `AGAINST` in MySQL, `CONTAINS` in Oracle and SQL Server, and `@@` in PostgreSQL).
** **DO NOT UPDATE CONTENT BELOW THIS LINE** **

