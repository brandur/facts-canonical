Travelling Salesman Problem
===========================

* NP-hard problem that states: given a list of cities and their pairwise distances, find the shortest possible tour that visits each city exactly once.
* Has a decision version of the problem which is NP-complete: given a length L, decide whether any tour is shorter than L.
* The nearest neighbor (NN) algorithm (AKA greedy algorithm) lets the salesman choose the nearest unvisited city as his next move. This on average yields a path 25% longer than the shortest possible path. However, there exists some city distributions which make the NN algorithm give the worst route.

