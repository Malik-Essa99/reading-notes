### Hash Tables

The Basics of hash tables:

1. Hash Function: A hash function is a mathematical function that takes a key as input and computes a hash code, which is a numeric value. The hash code is used to determine the index or bucket where the corresponding value will be stored in the hash table. An ideal hash function should distribute the keys uniformly across the array or buckets to minimize collisions.

2. Array or Buckets: A hash table typically uses an array or a collection of buckets to store the key-value pairs. The size of the array or the number of buckets is determined during the initialization of the hash table.

3. Index Calculation: Once the hash code is computed using the hash function, the next step is to map it to an index within the array or bucket. This can be achieved by performing a modulo operation on the hash code with the size of the array. The result of the modulo operation gives the index where the value will be stored.

4. Collision Handling: Collisions occur when two or more keys produce the same hash code and map to the same index. Hash tables employ collision resolution techniques to handle such situations. Two common approaches are separate chaining and open addressing. In separate chaining, each index in the array contains a linked list of key-value pairs with the same hash code. In open addressing, when a collision occurs, an alternative location within the array is searched using a probing sequence until an empty slot is found.

5. Insertion, Retrieval, and Deletion: The basic operations performed on a hash table are insertion (adding a new key-value pair), retrieval (finding the value associated with a given key), and deletion (removing a key-value pair). To insert a key-value pair, the key is hashed to determine the index and the pair is stored at that index. For retrieval, the key is hashed to find the corresponding index, and the value is returned if it exists. Deletion involves finding the key, typically by hashing it, and removing the corresponding key-value pair from the hash table.

6. Load Factor and Resizing: The load factor of a hash table is the ratio of the number of key-value pairs stored to the size of the array or number of buckets. A high load factor can increase the likelihood of collisions and degrade performance. To maintain efficient operations, hash tables often employ resizing strategies. When the load factor exceeds a certain threshold, the hash table is resized by creating a larger array or increasing the number of buckets, and the existing key-value pairs are rehashed and reinserted into the new structure.