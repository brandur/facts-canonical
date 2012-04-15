Concepts
========

** **DO NOT UPDATE CONTENT BELOW THIS LINE** **

Common Subexpression Elimination
--------------------------------

* Compiler optimization that searches for instances of identical expressions (i.e. all evaluating to the same value), and analyses whether it is worthwhile replacing them with a single varaible holding the computed value.
* e.g. expressions `a = b * c + g` and `d = b * c * d`. The compiler may add `tmp = b * c` and replace `b * c` in each expression with the value of `tmp`. It must also perform a cost/benefit analysis and decide whether the cost of the store to `tmp` is less than the cost of the multiplication.

Memoization
-----------

* Optimization technique used primarily to speed up computer programs by having function calls avoid repeating the calculation of results for previously-processed inputs.

NP-complete
-----------

* A decision problem L is NP-complete if it is in the set of NP problems so that any given solution to the problem can be verified in polynomial time.
* Solutions can be verified quickly, but there is no known efficient way to locate a solution in the first place.
* The time required to solve even moderately large versions of many of these problems easily reaches into the billions or trillions of years using any amount of computing power available today.

NP-hard
-------

* NP-hard (non-deterministic polynomical-time hard), is a class of problems that are at least as hard as the hardest problems in NP.
* Problems need not be in NP; indeed, they may not even be decision problems.

NP-intermediate
---------------

* If P &neq; NP then there exists problems in NP that are neither P nor NP-complete, and these are called NP-intermediate. For now, it is not known whether they are P or NP-complete.
* Examples are the graph isomorphism problem, the discrete logarithm problem, and the integer factorization problem.

Name Binding
------------

* Association of objects (data/code) with identifiers. An identifier bound to an object is a _reference_ to that object.
* **Static** (or early): bindings performed before a program runs. e.g. A function call in C.
* **Dynamic** (or late, or virtual): bindings performed as the program runs. e.g. _Dynamic dispatch_, as in a virtual method call in C++.
* **Late static**: somewhere between static and dynamic. e.g. A static field reference in PHP can be changed in a class by redefining that field in a derivation of that class.

P Versus NP Problem
-------------------

* Major unsolved problem in computer science. Informally, it asks whether every problem whose solution can be efficiently checked by a coputer can also be efficiently _solved_ by a computer.
* One of the seven Millenium Prize Problems selected by the Clay Mathematics Institute to carry a US$ 1,000,000 prize for the first correct solution.
* The class of questions for which some algorithm can provide an answer in polynomial time is called P. The class of questions for which an answer can be verified in polynomial time is called NP.

Referencial Transparency
------------------------

* An expression is said to be referentially transparent if it can be replaced with its value without changing the program (same output given same input).
* Importance is that it allows the programmer and the compiler to reason about program behavior.
* Can help in proving correctness, simplifying an algorithm, assisting in modifying code without breaking it, or optimizing by means of memoization, common subexpression elimination, or parallelization.
* If all functions involved in an expression are pure functions, then the expression is referentially transparent. Impure functions can be included if their values are discarded and their side effects are insignificant.
* All functions in the mathematical sense are referentially transparent (e.g. `5*5` or `sin(x)`).

Time Complexity
---------------

* Quantifies the amount of time taken by an algorithm to run as a function of the size of the input of the problem.

