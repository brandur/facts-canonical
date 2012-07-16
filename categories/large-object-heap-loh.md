Large Object Heap (LOH)
-----------------------

* For objects >= 85k. An array needs ~10,000 elements before it goes to the LOH.
* Garbage collector generally tries to reclaim space from other heaps before tackling the LOH.
* Large objects can't reliably be moved, and therefore no compaction occurs in the LOH.
* .NET tries to allocate new objects in holes left behind by old objects, and expands the heap if no hole is large enough. However, if the heap doesn't need to be expanded, .NET prefers to put new objects at the end of the heap so that it doesn't need to look for a hole.
* LOH eventually becomes fragmented and can cause even programs with no memory leaks to fail with an **OutOfMemoryException**.
