# Hash Table Analysis Laboratory

## Core goals
Students must implement a hash table that stores key-value pairs using open addressing and quadratic probing.

## Required behaviors
Students must implement:

- insertion with collision handling;
Function hashes and if its taken it does quadratic probing to find an availible position. When the table is full, it rehashes.
- lookup and retrieval;
When key isn't found it is searched thru quadratic probing. Value is returned if the key is found/exists.
- update of existing entries;
Looks for key. when its found it replaces the value.
- deletion while preserving probe correctness;
deleted entries are marked as deleted instead of being made empty. This lets us continue our search.
- capacity growth and rehashing;
Once a threshold is met, the hash table makes itself bigger via rehashing.
- hash function design;
The function has to distribute the keys evenly to avoid collisions.
- complex-key scenarios with many collisions.
Forced to probe, higher lookup cost. Quadratic probing reduces the chance of collisions but doesn't completely stop them from occuring.
## Required analysis
Students should write a short comparison and complexity analysis of:

- average-case insertion, lookup, and removal;
- best-case and worst-case behavior;
- collision resolution strategies;
- load factor and rehashing costs;
- open addressing vs. chaining;
- how clustering can affect performance.

## Big-O expectations
Students should identify and explain the Big-Oh for:

- `insert` average is O(1) | Worst O(n)
- `remove` average is O(1) | Worst O(n)
- `get` average is O(1) | Worst O(n)
- `update` average is O(1) | Worst O(n)
- `rehash` average is O(n) | Worst O(n)
- `contains` average is O(1) | Worst O(n)

Expected average-case: O(1) for insert, lookup, and update under a reasonable load factor; worst case can degrade to O(n) when many collisions occur or the table becomes badly loaded.
