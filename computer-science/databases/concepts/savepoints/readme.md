Savepoints
==========

* Way of implementing subtransactions (i.e. nested transactions) in an RDMS. Multiple savepoints can exist within a single transaction, so an application can recover from an error by rolling back to a savepoint rather than aborting an entire transaction.
* Declared by using `SAVEPOINT name`. `ROLLBACK TO SAVEPOINT name` does so, and `RELEASE SAVEPOINT name` discards it.

