Small Object Heap (SOH)
=======================

* Objects are allocated to the SOH consecutively (contiguous heap), with .NET maintaining a next object pointer.
* GC runs when memory usage reaches some threshold.

