Common Table Expressions
------------------------

* Temporary named result set, derived from a simple query and dfined within the execution scope of a `SELECT`, `INSERT`, `UPDATE`, or `DELETE`.
* Looks like `WITH [RECURSIVE] with_query [, ...] SELECT ...` where the CTE is able to reference itself within its own body.
