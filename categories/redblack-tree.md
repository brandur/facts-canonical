Red-black Tree
--------------

* Average time complexity: space `O(n)`, search `O(log n)`, insert `O(log n)`, delete `O(log n)`. Worst case time complexity: the same.
* Type of self-balancing binary search tree, typically used to implement associative arrays.
* The Completely Fair Scheduler used in current Linux kernels uses red-black trees.
* Leaf nodes do not contain data. These leaves need not be explicit in memory, a null pointer can be used, but having explicit leaves simplifies some algorithms. Sometimes a single sentinel node is used to perform the roll of all leaf nodes.
* Properties: (1) a node is either red or black, (2) the root is black, (3) all leaves are black, (4) both children of every red node are black, (5) every simple path (no repeated nodes) from a given node to any of its descendant leaves contains the same number of black nodes.
* Basic properties enforce a critial and complex one: the path from the root to the furthest leaf is no more than twice as long as the path from the root to the nearest leaf.
