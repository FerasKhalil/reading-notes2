# Read 15: Trees
- Node:  A Tree node is a component which may contain it’s own values, and references to other nodes
- Root: The root is the node at the beginning of the tree
- K: A number that specifies the maximum number of children any node may have in a k-ary tree. In a binary tree, k = 2.
- left: A reference to one child node, in a binary tree
- Right: A reference to the other child node, in a binary tree
- Edge: The edge in a tree is the link between a parent and child node
- Leaf: A leaf is a node that does not have any children
- Height: The height of a tree is the number of edges from the root to the furthest leaf
	- [from](https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-15/resources/Trees.html)


- we have 2 categrories of traversals in trees:
- the  common way to traverse through a tree is with recursion
	1. Depth first: it's where we prioritize gong through the height of the tree and there are three methods for it:
		1. Pre-order: root >> left >> right
		2. In-order: left >> root >> right
		3. Post-order: left >> right >> root
	2. Breadth first: is to traverse through one entire level of children nodes first, before moving on to traverse through the grandchildren nodes


## Adding a node
- Because there are no structural rules for where nodes are “supposed to go” in a binary tree, it really doesn’t matter where a new node gets placed.
	- [from](https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-15/resources/Trees.html)
- one other way to add a node is to use traversal to see which node doesn't have all children complete and add the new node there.

### Big O
- The Big O time complexity for inserting a new node is O(n)
- the big O for searching for a specific node will also be O(n)
- the Big O for space using traversal is O(w). 
	- w is the largest width of the tree

- **A perfect binary tree** is when all non-leaf nodes have only 2 children
- The maximum width for a perfect binary tree, is 2^(h-1),  **h** is the height and it's calculated as **log n**, n is the number of nodes.

## Binary Search Trees (BST)
- It's organized making all smaller values on the left and all greater values on the right. and that's not only for the root,
	- this technique applies on all children nodes too.
- the big(O) of time for binary search trees is o(h) which means it depends on the height knowing that'h' stands for height
- The Big O space complexity of a BST search would be O(1). During a search, we are not allocating any additional space.
- In a "balanced" or "perfect" tree, the height of the tree is log(n).
	- [from](https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-15/resources/Trees.html)