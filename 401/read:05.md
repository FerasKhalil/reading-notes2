# READ: 05 - Implementation: Linked Lists
##  Linked Lists
- a linked list is a sequence of nodes that are linked/connected to each other
    - from (https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-05/resources/singly_linked_list.html)

- types of Linked Lists: 
    1. singly: Singly refers to the number of references the node has. 
    2. doubly: Doubly refers to there being two (double) references within the node

## What’s a Linked List, Anyway pt1
- Linked lists are linear data structures
	- unlike Trees and graphs which are considered non-linear data structures

- the biggest difference between arrays and lists is the way that they ise memory in machines.
	- arrays take bytes of memory that are next to each other
	- unlike linked lists which use random memory places to store its data
	- the reason to this is because a node doesn't know the length of the list
	- so its stored randomly in memory

- linked lists are made up of a series of nodes.

- the starting point of the list is a reference to the first node which is called "head"

- the end of the list isn't a node, but rather a node that points to null

- a node has to things inside it:
	1. data or information 
	2. and the reference to the next node

### What’s a Linked List, Anyway pt2
- a linked list is not good to use when you have to do a lot of traversal, iteration or quick inedx-level acess
	- from (https://medium.com/basecs/whats-a-linked-list-anyway-part-2-131d96f71996)

#### big O notation
- O(1) has constant time no matter how many elements we actually have

- o(n) function is linear which means as our input grows the space and time it needs to run keeps growing lineary

- o(n^2) function takes the most time and space