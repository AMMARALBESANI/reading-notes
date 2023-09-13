# Hash Table (Hash Map)

A Hash Table is a fundamental data structure used in computer science for efficient data storage and retrieval. It relies on the concept of hashing, which involves transforming keys into unique indices in an array or a table, where associated values can be stored and quickly accessed.

## Key Concepts

### Hash Function

- A hash function is a crucial component of a Hash Table. It takes an input (typically a key) and returns a fixed-size numerical value, which is used as an index or address in the table.
- The goal of a good hash function is to distribute keys evenly across the array of indices to minimize collisions. It should produce distinct hash codes for different keys.

### Array or Buckets

- A Hash Table is typically implemented as an array (or an array of linked lists), where each element is called a "bucket."
- The number of buckets determines the size of the Hash Table. The choice of the array size can impact the efficiency of the hash table, especially regarding collision resolution.

### Insertion

- To insert a key-value pair into the Hash Table, you first apply the hash function to the key, which yields an index.
- The key-value pair is then placed into the corresponding bucket at that index.
- If multiple key-value pairs hash to the same index (a collision), different collision resolution techniques can be employed to handle this situation.

### Collision Resolution Techniques

- Collisions occur when two or more keys produce the same hash code (i.e., map to the same index). Various techniques are used to resolve these collisions:
  - **Chaining**: Each bucket contains a linked list or another data structure to store multiple key-value pairs that hash to the same index.
  - **Open Addressing**: When a collision happens, the algorithm searches for the next available slot within the Hash Table to store the key-value pair.
  - **Double Hashing**: This technique uses a secondary hash function to calculate alternative indices for collided keys until an empty slot is found.

### Retrieval

- To retrieve a value associated with a key, you apply the hash function to the key to determine the index.
- If collisions are resolved using chaining, you navigate the linked list in the selected bucket to find the desired key-value pair.

### Load Factor

- The load factor is a measure of how full the Hash Table is. It's calculated as the number of elements stored divided by the number of buckets.
- A high load factor can lead to increased collisions and decreased performance. To maintain efficiency, the table may need to be resized (i.e., more buckets added) when the load factor exceeds a certain threshold.

