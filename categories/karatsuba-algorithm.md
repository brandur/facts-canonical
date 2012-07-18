Karatsuba Algorithm
-------------------

* Fast multiplication algorithm discovered by Anatolii Alexeevitch Karatsuba in 1960 and published in 1962.
* First asymptotically fast multiplication algorithm.
* Reduces the multiplcation of two n-digit numbers to at most \( 3n^{log_2{3}} =~ 3n^1.585 \) single-digit multiplications. Exactly \( n^{log_2{3}} \) when n is a power of 2. Classical algorithm requies \( n^2 \) single-digit products.
* The Toom-Cook algorithm is a faster generalization of this algorithm. For sufficiently large \( n \), the Schonhage-Strassen algirthm (another generalization) is even faster.
