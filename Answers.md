## Data Structures Fu Questions

### 1. What are the order of insertions/removals for the following data structures?
* **Stack:** A stack data structure is much like a stack of books: you're able to add and remove data from only one side of the stack. As such, it follows LIFO (Last In, First Out) ordering - meaning that the last thing placed on the stack will be the first thing removed from the stack.
* **Queue:** It's easiest to think of a queue as a line at a store: data that was placed earliest in a queue will be the first data taken out of the queue. As such, this would be a FIFO (First In, First Out) order.

### 2. What is the retrieval time complexity for the following data structures?
* **Linked List:** The retrieval time increases at the same rate as the amount of input data. As such, this would be considered O(n), or linear time complexity.

* **Hash Table:** Retrieving data from hash tables will always take the same amount of time, regardless of input data. This makes it a constant time operation, or O(1).

* **Binary Search Trees:** Since a binary search tree pretty much cuts itself in half with every check (never needing to dig through half of the data each time), it will move through searches very rapidly at the beginning, and then performance will begin to level off the further into the tree a search needs to go. As such, O(log n), or logarithmic time complexity, can be expected on average, though in the worst case scenario performance can drop down to linear time complexity, or O(n).


### 3. What are some advantages to using Hash Tables over arrays in JavaScript?
* Efficient data retrieval and removal with large data sets, as these operations have O(1) time complexity with hash tables, and typically O(n) time complexity in arrays due to the need for iteration (unless you know in advance exactly which index to check).
* Hashing lends itself well to cryptography, as opposed to just a list of clear values.