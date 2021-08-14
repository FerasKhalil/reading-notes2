# Read: Stacks & Queues
## Stacks and Queues

- stack is a data structure that consists of Nodes. each node has a 
	value and a reference for the next node.
- Nodes can not reference the node that is before it.
- Push: nodes or items that are put into the stack are pushed
- Pop: nodes or items that are removed from the stack are popped. 
	- if the list is empty and you try to pop, an exception should be raised
- Top: means the top of the stack
- Peek: When you peek you will view the value of the top Node in the stack.
	 When you attempt to peek an empty stack an exception will be raised.
- IsEmpty: returns true when stack is empty otherwise returns false.
- FILO (First In Last Out)
	- This means that the first item added in the stack will be the last item popped out of the stack.

- LIFO (Last In First Out)
	- This means that the last item added to the stack will be the first item popped out of the stack.

- pushing to a stack is o(1)
- When adding a Node, you push it into the stack by assigning it as the new top, with its next property equal to the original top.

- popping from a stack is also O(1)

### Queue
- Enqueue - Nodes or items that are added to the queue.
- Dequeue - Nodes or items that are removed from the queue. If called when the queue is empty an exception will be raised.
- Front - This is the front/first Node of the queue.
- Rear - This is the rear/last Node of the queue.
- Peek - When you peek you will view the value of the front Node in the queue. If called when the queue is empty an exception will be raised.
- IsEmpty - returns true when queue is empty otherwise returns false.


Queues follow these concepts:

- FIFO (First In First Out)
	- This means that the first item in the queue will be the first item out of the queue

- LILO (Last In Last Out)
	- this means that the last item added to the stack will be the first item popped out of the stack


- from (https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-10/resources/stacks_and_queues.html)