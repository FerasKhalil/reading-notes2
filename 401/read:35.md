# Read 35: Graphs 
- A graph is a non-linear data structure that can be looked at as a collection of vertices (or nodes) potentially connected by line segments named edges.
- Terminology used when working with graphs:
	1. Vertex
	-  A vertex, also called a “node”, is a data object that can have zero or more adjacent vertices.
	2. Edge
	- An edge is a connection between two nodes.
	3. Neighbor
	-  The neighbors of a node are its adjacent nodes, i.e., are connected via an edge.
	4. Degree
	-  The degree of a vertex is the number of edges connected to that vertex.
- Undirected graph is a graph where each edge is undirected or bi-directional. This means that the undirected graph does not move in any direction.
- Directed Graphs (Digraph) 
	- A Directed Graph also called a Digraph is a graph where every edge is directed.
	-  a Digraph has direction. Each node is directed at another node with a specific requirement of what node should be referenced next.



- A **connected** graph is a graph that has all of **vertices** / **Nodes** have at least one edge.

- A **disconnected** graph is where some vertices may not have edges.

- A **Acyclic Graph** is a directed graph without cycles.

- A **cycle** is when a node can be traversed through and potentially end up back at itself.
 
- **Cyclic Graphs** is a graoh that has cycles.

- We represent a graph through:
	1. Adjacency Matrix
		- represented through a 2-dimensional array. If there are n vertices, then we are looking at an n x n Boolean matrix.
		- Each Row and column represents each vertex of the data structure. 
		- The elements of both the column and the row must add up to 1 if there is an edge that connects the two, or zero if there isn’t a connection.
	2. Adjacency List
		- An adjacency list is the most common way to represent graphs.
		- An adjacency list is a collection of linked lists or array that lists all of the other vertices that are connected.
		- Adjacency lists make it easy to view if one vertices connects to another.

- Weighted Graphs
	- A weighted graph is a graph with numbers assigned to its edges. These numbers are called weights.
- Traversals
	- Breadth first
	- Depth first



- Source from(https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-35/resources/graphs.html)