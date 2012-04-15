Concepts
========

** **DO NOT UPDATE CONTENT BELOW THIS LINE** **

Common Table Expressions
------------------------

* Temporary named result set, derived from a simple query and dfined within the execution scope of a `SELECT`, `INSERT`, `UPDATE`, or `DELETE`.
* Looks like `WITH [RECURSIVE] with_query [, ...] SELECT ...` where the CTE is able to reference itself within its own body.

Data Domain
-----------

* Refers to all the unique values which a data element may contain. Maybe be as simple as a data type or enumerated list of values.

Embedded SQL
------------

* SQL statements written inline with the program source code of a host language. The embedded SQL statements are parsed by an embedded SQL preprocessor and replaced by host-language calls to a code library and compiled.

Savepoints
----------

* Way of implementing subtransactions (i.e. nested transactions) in an RDMS. Multiple savepoints can exist within a single transaction, so an application can recover from an error by rolling back to a savepoint rather than aborting an entire transaction.
* Declared by using `SAVEPOINT name`. `ROLLBACK TO SAVEPOINT name` does so, and `RELEASE SAVEPOINT name` discards it.

Tablespaces
-----------

* Storage mechanism where database objects can be kept. It provides a layer of abstraction between physical and logical data, and allocates storage for all DBMS managed segments (a segment is an object that occupies physical space like a table or index).
* Using tablespaces, the disk layout of an installation can be controlled. A heavily used index can be placed on a fast SCSI disk while a rarely accessed table could be put on a slow IDE disk.

