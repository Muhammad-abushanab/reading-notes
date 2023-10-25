## Anatomy of a Hash Table:
**Hash Function:** The heart of a hash table is the hash function. This function takes a key and transforms it into an array index. The objective of the hash function is to ensure that keys are evenly distributed across the array of buckets. A good hash function minimizes collisions (i.e., two keys producing the same index).

**Buckets:** An array of "slots" or "buckets" makes up a hash table. One or more key-value pairs may be stored in each bucket. The real data is kept in buckets.
Key-Value Pairs: Data is stored in hash tables as key-value pairs. The value is indexed using the key. For instance, the name may serve as the key and the age as the value if you wanted to record a person's name and age.

**Collisions:** When two distinct keys generate the same hash (that is, map to the same bucket), a collision occurs. Many hash tables utilize a method called chaining to deal with collisions. A linked list (or equivalent data structure) of key-value pairs that map to the same index is contained in each bucket in a chained system.

### Common Operations:
**Insertion:** The hash function determines the key's index, and the pair is then inserted into the appropriate bucket in a hash table. Chaining is used to add the new pair to the linked list in the bucket in the event of a collision.

**Retrieval:** To retrieve a value, the hash function is applied to the key, which tells you the bucket where the value is stored. If there are collisions, you search the linked list in that bucket for the specific key.

**Deletion:** To delete a key-value pair, the hash function is used to find the correct bucket, and then the key is searched in the linked list. The pair is deleted if it is located.

### Time Complexity:

Hash table operations (insertion, retrieval, and deletion) are usually O(1), or have constant time complexity, under ideal circumstances, when the hash function distributes keys equally and there are no collisions.
However, in the worst scenario, operations might become O(n), where n is the total number of key-value pairs, when many keys collide and end up in the same bucket. Although this is uncommon in real life, it is important to be aware of it.
Content Ratio:
The ratio of the number of key-value pairs saved to the number of buckets in the hash table is known as the load factor. Overly high load factors raise the risk of accidents, which can lead to performance degradation. You can resize the hash table to lessen this.


### Features of Hashtable

- It is similar to HashMap, but is synchronized.
- Hashtable stores key/value pair in hash table.
- In Hashtable we specify an object that is used as a key, and the value we want to associate to that key. The key is then hashed, and the resulting hash code is used as the index at which the value is stored within the table.
- The initial default capacity of Hashtable class is 11 whereas loadFactor is 0.75.
- HashMap doesn’t provide any Enumeration, while Hashtable provides not fail-fast Enumeration.