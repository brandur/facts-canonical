B-tree
======

* Average time complexity: space `O(n)`, search `O(log n)`, insert `O(log n)`, delete `O(log n)`. Worst case time complexity: the same.
* Generalization of a binary search tree in that a node can have more than two children.
* Unlike self-balancing binary search trees, the B-tree is optimized for systems that read and write large blocks of data. It is commonly used in databases and filesystems.
* Internal (non-leaf) nodes can have a variable number of child nodes (depending on the implementation). In order to maintain that range, nodes may be joined or split.
* Because a range of child nodes is permitted, B-trees do not need re-balancing as frequently as other self-balancing search trees, but may waste some space, since nodes are not entirely full.
* Usually the number of keys chosen varies between `d` and `2d`, the factor of 2 guarantees that nodes can be split or combined.The number of branches from a node will be _more_ than the number of keys stored in the node. e.g. In a 2-3 B-tree, nodes store either 1 key with 2 child nodes, or 2 keys with 3 child nodes.
* Keeps balanced by requiring that all leaf nodes are at the same depth. Increases in overall depth are infrequent.
* B-trees have substantial advantages when node access times far exceed access times within nodes, because the node access cost can be amortized over multiple node operations.
** **DO NOT UPDATE CONTENT BELOW THIS LINE** **

B+ Tree
-------

* All records are stored at the leaf level of the tree; only keys are stored in the interior nodes.
* Primary value of a B+ tree is storing data for efficient retrieval in a block-oriented storage context&mdash;in particular, filesystems. This is due to high fanout, which reduces the number of I/O operations required for search.
* Usage in filesystems: NTFS, ReiserFS, NSS, XFS, and JFS. Usages in RDMSes: DB2, SQL Server, Oracle 8, PostgreSQL, Firebird, MySQL, and SQLite. Usage in NoSQL: CouchDB, Tokyo Cabinet.
* Leaves in a B+ tree are oftened linked with a linked list; this makes range queries on the blocks simpler and more efficient. This does not substantially increase space consumption or maintenance. This illustrates a significant advantage of a B+ tree over a B-tree (in a B+tree, all records are in the leaf nodes).
* The number of children for an internal node is constrainted by the order (or branching factor) of the tree.

