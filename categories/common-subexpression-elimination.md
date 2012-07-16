Common Subexpression Elimination
--------------------------------

* Compiler optimization that searches for instances of identical expressions (i.e. all evaluating to the same value), and analyses whether it is worthwhile replacing them with a single varaible holding the computed value.
* e.g. expressions `a = b * c + g` and `d = b * c * d`. The compiler may add `tmp = b * c` and replace `b * c` in each expression with the value of `tmp`. It must also perform a cost/benefit analysis and decide whether the cost of the store to `tmp` is less than the cost of the multiplication.
