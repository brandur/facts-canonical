Karatsuba Algorithm
-------------------

* Fast multiplication algorithm discovered by Anatolii Alexeevitch Karatsuba in 1960 and published in 1962.
* First asymptotically fast multiplication algorithm.
* Reduces the multiplcation of two n-digit numbers to at most <math>3n^{log_2{3}} =~ 3n^1.585</math> single-digit multiplications. Exactly <math>n^{log_2{3}}</math> when n is a power of 2. Classical algorithm requies <math>n^2</math> single-digit products.
* The Toom-Cook algorithm is a faster generalization of this algorithm. For sufficiently large <math>n</math>, the Schonhage-Strassen algirthm (another generalization) is even faster.
