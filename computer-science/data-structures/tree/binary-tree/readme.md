Binary Tree
===========

* Tree in which each node has at most 2 child nodes.
* The **depth** of a node is the length of the path from it to root.
* The **height** of a tree is the depth of the deepest node.
* **In-degree** of a node is the number of edges arriving at it, and its **out-degree** is the number of edges leaving it.
* A **full binary tree** (AKA proper binary tree, 2-tree, or strictly binary tree) is a tree in which every node other than the leaves has 2 children.
* A **perfect binary tree** is a full binary tree in which all leaves are at the same depth.
* A **complete binary tree** is a binary tree in which every level, except possibly the last, is completely filled, and all nodes are as far left as possible.
* A **balanced binary tree** is one in whichthe height of the 2 subtrees of every node never differ by more than 1.
* A **degenerate binary tree** is a tree where for each parent node, there is only one child. Performance-wise, this tree will behave like a linked list.
** **DO NOT UPDATE CONTENT BELOW THIS LINE** **

Binary Search Tree
------------------

* Average time complexity: space `O(n)`, search `O(log n)`, insert `O(log n)`, delete `O(log n)`. Worst case time complexity: Space `O(n)`, search `O(n)`, insert `O(n)`, delete `O(n)`.
* Properties: (1) the left subtree of a node contains only nodes with keys less than the node's key, (2) the right subtree has only nodes greater, (3) both left and right subtrees are also binary search trees.
* Major advantage is that sorting algorithms, search algorithms, and in-order traversal can be very efficient.
* Fundamental data structure used to construct more abstract data structures such as sets, multisets, and associative arrays.
* Out of binary search trees, treaps have been found to have the best average performance, while red-black trees have the smallest performance fluctuation.

