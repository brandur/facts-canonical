Suffix Tree
===========

* The suffix tree (AKA _PAT tree_ or _position tree_) presents the suffixes of a given string in a way that allows for fast implementations of many string operatios.
* Edges are labeled with strings, such that each suffix of <math>S</math> corresponds to exactly 1 path from the tree's root to a leaf.
* Constructing a suffix tree is O(n) time and memory.
* Fast operations: locating a substring, locating a substring with mistakes allowed, regular expression matching, and longest common substrings (one of the first O(n) solutions to this problem).

