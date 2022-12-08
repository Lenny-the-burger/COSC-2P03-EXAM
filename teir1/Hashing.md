# Hashing

-   Chapter 5 covers the topic of hashing.
-   Understand the definitions and properties of hashing, including collisions, collision resolution policies, and the load factor.
-   Be familiar with the concept of separate chaining and buckets.
-   Know how to implement open addressing, including linear and quadratic probing and double hashing.
-   Understand the concept of rehashing and know when and how to do it.
-   Be familiar with the concept of extendible hashing.

Hashing is a technique for storing and retrieving data from a collection (such as a hash table or hash map) using a hash function to map the data items to indices in the collection. Hashing is used to implement efficient data structures such as dictionaries, sets, and associative arrays.

## Definitions

There are several key terms that are used when discussing hashing:

-   Hash function: a hash function is a function that maps data items to indices in the collection. A good hash function will distribute the data items evenly across the indices in the collection, so that the data can be efficiently stored and retrieved.
-   Hash table: a hash table is a data structure that stores data items using a hash function to map the items to indices in the table. A hash table can be implemented using an array or a linked list, and it allows for efficient insertion, deletion, and retrieval of data items.
-   Collision: a collision occurs when two data items are mapped to the same index in the collection by the hash function. Collisions can be resolved using collision resolution policies, such as chaining or open addressing.
-   Load factor: the load factor of a hash table is the ratio of the number of data items stored in the table to the number of indices in the table. A high load factor can increase the number of collisions and decrease the efficiency of the hash table.

## Collision resolution policies

There are several different strategies for resolving collisions in a hash table, including:

-   Chaining: chaining is a collision resolution policy that stores multiple data items at the same index in the table using a linked list or some other data structure. Chaining allows for efficient insertion and deletion of data items, but it can increase the amount of memory used by the hash table.
-   Open addressing: open addressing is a collision resolution policy that uses the hash function to find an empty index in the table to store a data item that has collided with another item. There are several different strategies for open addressing, including linear probing, quadratic probing, and double hashing. Open addressing can be more memory-efficient than chaining, but it can suffer from clustering, where many items are stored at the same index in the table.

## Rehashing

Rehashing is the process of increasing the size of the hash table and remapping the data items to the new indices in the table. Rehashing is necessary when the load factor of the hash table reaches a certain threshold (such as 0.75), to prevent the table from becoming too full and inefficient.

## Extendible hashing

Extendible hashing is a variation of hashing that uses a dynamic hash function to adjust the number of bits used to map data items to indices in the table. The dynamic hash function can split and merge indices in the table to maintain a good balance between the number of items stored at each index and the size of the table. Extendible hashing allows for efficient insertion and deletion of data items, and it can adapt to changes in the data distribution over time.

## Examples

There are several different methods for implementing hashing, including:

-   Separate chaining: in separate chaining, each index in the hash table is a linked list or some other data structure that stores the data items that have been mapped to that index by the hash function. To insert or retrieve a data item, the hash function is used to compute the index in the table, and then the item is added to or searched for in the linked list at that index. This method is simple to implement and allows for efficient insertion and deletion of items, but it can use more memory than other methods.
-   Open addressing: in open addressing, each index in the hash table is a single data item. When a collision occurs, the hash function is used to find another index in the table where the colliding item can be stored. There are several different strategies for open addressing, including linear probing, quadratic probing, and double hashing. Linear probing uses a fixed increment (such as 1 or the size of the table) to find the next index to check for an empty slot, while quadratic probing uses a quadratic function (such as the square of the increment) to find the next index. Double hashing uses a second hash function to compute the increment to use for probing. Open addressing can be more memory-efficient than chaining, but it can suffer from clustering, where many items are stored at the same index in the table.
-   Extendible hashing: in extendible hashing, the hash function is dynamic and can adjust the number of bits used to map data items to indices in the table. The hash function splits and merges indices in the table to maintain a good balance between the number of items stored at each index and the size of the table. This method allows for efficient insertion and deletion of items, and it can adapt to changes in the data distribution over time.
