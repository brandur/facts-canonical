Tree
====

** **DO NOT UPDATE CONTENT BELOW THIS LINE** **

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

Binary Tree
-----------

* Tree in which each node has at most 2 child nodes.
* The **depth** of a node is the length of the path from it to root.
* The **height** of a tree is the depth of the deepest node.
* **In-degree** of a node is the number of edges arriving at it, and its **out-degree** is the number of edges leaving it.
* A **full binary tree** (AKA proper binary tree, 2-tree, or strictly binary tree) is a tree in which every node other than the leaves has 2 children.
* A **perfect binary tree** is a full binary tree in which all leaves are at the same depth.
* A **complete binary tree** is a binary tree in which every level, except possibly the last, is completely filled, and all nodes are as far left as possible.
* A **balanced binary tree** is one in whichthe height of the 2 subtrees of every node never differ by more than 1.
* A **degenerate binary tree** is a tree where for each parent node, there is only one child. Performance-wise, this tree will behave like a linked list.

Suffix Tree
-----------

* The suffix tree (AKA _PAT tree_ or _position tree_) presents the suffixes of a given string in a way that allows for fast implementations of many string operatios.
* Edges are labeled with strings, such that each suffix of <math>S</math> corresponds to exactly 1 path from the tree's root to a leaf.
* Constructing a suffix tree is O(n) time and memory.
* Fast operations: locating a substring, locating a substring with mistakes allowed, regular expression matching, and longest common substrings (one of the first O(n) solutions to this problem).

