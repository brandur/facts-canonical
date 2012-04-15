Time Complexity
===============

* Quantifies the amount of time taken by an algorithm to run as a function of the size of the input of the problem.

** **DO NOT UPDATE CONTENT BELOW THIS LINE** **

Big O Notation
--------------

* Used to describe the limiting behavior of a function when the argument tends towards a particular value or infinity, usually in terms of simpler functions.
* Usually only describes an upper bound on the growth rate of a function. Several other related notations describe other kinds of bounds on asymptotic growth rates: o, Ω, ω, and Θ.
* Rules: (1) if f(x) is the sum of several terms, the one with the largest growth rate is kept, and all others are omitted; and (2) if f(x) is a product of several factors, any constants are omitted.
* Ignoring lower order terms and coefficients has a negligible effect on the expression's value for most purposes.
* Number of steps in an algorithm varies between machine types, but only by a constant factor, keeping a Big O approximation accurate.

Examples
--------

* **Constant time** `O(1)`: determining if a number is even or odd.
* **Logarithmic time** `O(log n)`: binary search.
* **Linear time** `O(n)`: finding the smallest item in an unsorted array.
* **Linearithmic time** `O(n log n)`: fastest possible comparison sort; Fast Fourier transform.
* **Quadratic time** `O(n^2)`: bubble sort; insertion sort; naive multiplication of two `n`-digit numbers.
* **Cubic time** `O(n^3)`: naive multiplication of two `n×n` matrices.
* **Exponential time** `2^{O(n)}`: solving the traveling salesman problem using dynamic programming.
* **Factorial time** `O(n!)`: solving the traveling salesman problem via brute-force search.

