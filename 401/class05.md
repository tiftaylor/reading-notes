# Class 05 \| Implementation: Linked Lists
Article: [Linked Lists](https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-05/resources/singly_linked_list.html)     
Article: [What is a Linked List Anyway Part 1](https://medium.com/basecs/whats-a-linked-list-anyway-part-1-d8b7e6508b9d)  
Article: [What is a Linked List Anyway Part 2](https://medium.com/basecs/whats-a-linked-list-anyway-part-2-131d96f71996)   


## Linked Lists

Biggest takeaway is that Linked Lists aren't that hard to conceptually understand. The hardest part, is understanding when to use them. 

### What the Linked List essentially is
- Similiar to array, but different! Below explains how. 
- LL's don't need to reserve a specific linear groups amount of memory like an array and are therefore dynamic and can grow and shrink as the program needs. 
- The dynamic aspect of the LL is because the bits of memory it needs can be seperated from each other and live anywhere. 
- The List consists of nodes that have 2 main objectives: **data** and **reference**
    - The **data** is the value the node is holding
    - The **reference** points to either the *next* node address or both the *next* and *previous* node address
- You can use a **Singly** or **Doubly** linked list. The latter refers to the case when the **reference** points to 2 locations (previous and next).

### How to use the Linked List
- When traversing the LL, use a `while()` as opposed to `for` style loops for continious checking
- When traversing, the `current` node is the most useful
- Here is a code example from Code Fellows: 
```
ALGORTIHM Includes (value)
		// INPUT <-- integer value
		// OUTPUT <-- boolean
			
			Current <-- Head

			WHILE Current is not NULL
				IF Current.Value is equal to value
					return TRUE

				Current <-- Current.Next

			return FALSE
```
- The point is to rearrange the pointers when manipulating the LL
- Following these three steps from the article above is the best suggestion: 
<image src="../images/401-5.png" style="width: 400px">

> Ideally, you'll use the Linked List for adding and remove, but is slow for search and find of a single thing

### Big O note:
- Big O concept is about time and space effeciency of an algorithm. 
    - O(1) is constant time and the best result
    - O(n) is linear, which means input grows linearly
    - O(n2) is the worst which takes exponentially more time


[Back to Home](/README.md)