Bit Operations
==============

* Check if an integer is even or odd: x & 1 == 0 &rarr; even
* Test if n-th bit is set: x & (1 << n)
* Set n-th bit: y = x | (1 << n)
* Unset the n-th bit: y = x & ~(1 << n)
* Toggle the n-th bit: y = x ^ (1 << n)
* Turn off the rightmost 1-bit (the bit closest to the right that is set to 1): y = x & (x - 1)
* Isolate the rightmost 1-bit (works because of two's complement in which -x is the same as ~x + 1): y = x & (-x)
* Right propagate the rightmost 1-bit: y = x | (x - 1)
* Isolate the rightmost 0-bit: y = ~x & (x + 1)
* Turn on the rightmost 0-bit: y = x | (x + 1)
** **DO NOT UPDATE CONTENT BELOW THIS LINE** **

