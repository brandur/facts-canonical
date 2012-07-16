GiST
----

* GIST (or Generalized Search Tree), is a data structure and API used to build a variety of disk-based search trees. It is a genearalization of the B+tree, and provides a concurrent and recoverable height-balanced search tree without making assumptions about the data type stored.
* Allows easy development of specialized indexes for new data types.
* PostgreSQL implementation provides support for variable length keys, composite keys, and concurrency control and recovery. Implementations are PostGIS and BioPostgres bioinformatics.
