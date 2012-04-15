Referencial Transparency
========================

* An expression is said to be referentially transparent if it can be replaced with its value without changing the program (same output given same input).
* Importance is that it allows the programmer and the compiler to reason about program behavior.
* Can help in proving correctness, simplifying an algorithm, assisting in modifying code without breaking it, or optimizing by means of memoization, common subexpression elimination, or parallelization.
* If all functions involved in an expression are pure functions, then the expression is referentially transparent. Impure functions can be included if their values are discarded and their side effects are insignificant.
* All functions in the mathematical sense are referentially transparent (e.g. `5*5` or `sin(x)`).

