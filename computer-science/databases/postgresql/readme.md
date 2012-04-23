PostgreSQL
==========

* Evolved from the Ingres project at the the University of California, Berkeley. Michael Stonebraker returned to Berkeley in 1985 and started a post-Ingres project to address problems with contemporary databases systems that had become clear in the early 1980s.
* Stored procedures can execute blocks of code other than SQL and C. Standard supported languaes: PL/pgSQL (resembles Oracle's PL/SQL), PL/Tcl, PL/Perl, and PL/Python.
* Built-in support for B+-tree, hash, GiST, and GiN indexes. **Expression indexes** can be created with the result of an expression or function, rather than a simple column value. **Partial indexes** can be created by adding a `WHERE` clause to `CREATE INDEX`. The Postgres planner can use multiple indexes together to satisfy complex queries using temporary in-memory bitmap index operations.
* Triggers can follow the actions of SQL DML statements. Triggers are supported in tables, but not views, and are fired in alphabetical order.
* Concurrency managed through Multi-Version Concurrency Control (MVCC), which gives each user a snapshot of the DB, allowing changes to be made that are invisible to other users until a transaction is committed.
* Native data types include text search, geometric primitives, IPv4 and IPv6 addresses, CIDR blocks and MAC addresses, XML, and UUID.
* Tables can inherit characteristics from a parent table. Data in child tables will appear to exist in parent tables unless the `ONLY` keyword is used. Inheritance can be used to implement partitioning.
* Uses **write-ahead logging** to implement **continuous arching** and **point-in-time recovery** for any database that has it enabled.
* **TOAST** (The Oversized-Attribute Storage Technique) is used to transparently store large table attributes (such as big MIME attachments or XML messages) in a separate area with automatic compression.

