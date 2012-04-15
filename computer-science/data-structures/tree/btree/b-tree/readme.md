B+ Tree
=======

* All records are stored at the leaf level of the tree; only keys are stored in the interior nodes.
* Primary value of a B+ tree is storing data for efficient retrieval in a block-oriented storage context&mdash;in particular, filesystems. This is due to high fanout, which reduces the number of I/O operations required for search.
* Usage in filesystems: NTFS, ReiserFS, NSS, XFS, and JFS. Usages in RDMSes: DB2, SQL Server, Oracle 8, PostgreSQL, Firebird, MySQL, and SQLite. Usage in NoSQL: CouchDB, Tokyo Cabinet.
* Leaves in a B+ tree are oftened linked with a linked list; this makes range queries on the blocks simpler and more efficient. This does not substantially increase space consumption or maintenance. This illustrates a significant advantage of a B+ tree over a B-tree (in a B+tree, all records are in the leaf nodes).
* The number of children for an internal node is constrainted by the order (or branching factor) of the tree.

