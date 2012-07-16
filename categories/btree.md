B-tree
------

* Average time complexity: space `O(n)`, search `O(log n)`, insert `O(log n)`, delete `O(log n)`. Worst case time complexity: the same.
* Generalization of a binary search tree in that a node can have more than two children.
* Unlike self-balancing binary search trees, the B-tree is optimized for systems that read and write large blocks of data. It is commonly used in databases and filesystems.
* Internal (non-leaf) nodes can have a variable number of child nodes (depending on the implementation). In order to maintain that range, nodes may be joined or split.
* Because a range of child nodes is permitted, B-trees do not need re-balancing as frequently as other self-balancing search trees, but may waste some space, since nodes are not entirely full.
* Usually the number of keys chosen varies between `d` and `2d`, the factor of 2 guarantees that nodes can be split or combined.The number of branches from a node will be _more_ than the number of keys stored in the node. e.g. In a 2-3 B-tree, nodes store either 1 key with 2 child nodes, or 2 keys with 3 child nodes.
* Keeps balanced by requiring that all leaf nodes are at the same depth. Increases in overall depth are infrequent.
* B-trees have substantial advantages when node access times far exceed access times within nodes, because the node access cost can be amortized over multiple node operations.
