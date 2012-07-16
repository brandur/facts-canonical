Generational Garbage Collection
-------------------------------

* Newest objects die quickly while older objects stay around longer, therefore objects are grouped into generations: short-lived (gen 0), medium lived (gen 1), and long-lived (gen 2)
* When an objects survives a garbage collection, it is promoted to the next generation.
* Garbage collector runs when gen 0 objects reach ~256k, when gen 1 objects reach ~2M, when gen 2 objects reach ~10M, or when system memory is low.
