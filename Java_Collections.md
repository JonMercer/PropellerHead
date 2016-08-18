# Collection
http://docs.oracle.com/javase/tutorial/collections/index.html

- **Collection**: Stores stuff
	- **Set**: can't contain duplicates
		- *Hash Set*: stores elements in hash tables. No order, high performance
		- *Tree Set*: store elements in red-black tree. Orders elements base one value. Slower than hash set. 
		- *Linked Hash Set*: a hash table with a linked list running through it. Insertion order
		- **SortedSet**: elements in ascending order
	- **List**: ordered by user and can contain duplicates
		- *ArrayList*:   
		- *LinedList*: 
	- **Queue**: ordered by a certain rule
	- **DeQueue**: kind of like queue, but can access the end as well
- **Map**: KV store
	- *HashMap*: no order, high performance
	- *TreeMap*: 
	- *LinkedHashMap*:
	- **SortedMap**: elements in ascending order

- Vector: like an array, but can shrink and grow
- HashTable

Questions:
- What is a linked hash set
- What is TreeMap
- LinkedHashMap

## Traversing Collections
1. Aggregate operations: lambda functions and parallellized task
2. For each
3. Iterators