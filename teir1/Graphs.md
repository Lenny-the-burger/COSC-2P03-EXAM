# Graphs

```
  a --- b
  |     |
  |     |
  c --- d
```

- Chapter 9 covers the topic of graphs.
-   Understand the definitions and properties of graphs, including directed and undirected graphs, and weighted and unweighted graphs.
-   Know how to represent graphs, including the appropriate representation to use in different situations.
-   Be familiar with depth-first search and breadth-first search and know how to implement them.
-   Understand the concept of a topological sort and know how to implement it.
-   Be familiar with Euler circuits and paths.
-   Know how to find the shortest path in a graph using unweighted and weighted algorithms (BFS and Dijkstra's algorithm, respectively).
-   Understand the concept of connectivity in a graph.
-   Know how to find a minimum spanning tree using Prim's and Kruskal's algorithms.

A graph is a data structure that consists of a set of nodes (also called vertices) and a set of edges that connect the nodes. Graphs are useful for representing and modeling many different types of real-world systems, such as networks of roads, social networks, and communication networks.

## Definitions

There are several key terms that are used when discussing graphs:

-   Node: a node (or vertex) is a point in the graph that represents an object or entity. A node may have zero or more edges that connect it to other nodes in the graph.
-   Edge: an edge is a connection between two nodes in the graph. An edge may be directed (i.e. it has a specific starting and ending node) or undirected (i.e. it has no specific starting or ending node). An edge may also be weighted (i.e. it has a numeric value associated with it) or unweighted (i.e. it has no numeric value associated with it).
-   Path: a path is a sequence of nodes and edges that connects two nodes in the graph. A path may be simple (i.e. it does not visit the same node more than once) or it may be a cycle (i.e. it visits the same node more than once).

-   Connectedness: a graph is connected if there is a path between every pair of nodes in the graph. Otherwise, the graph is said to be disconnected.

## Representation of graphs

There are several different ways to represent a graph, including:

-   Adjacency matrix: an adjacency matrix is a two-dimensional array that represents the edges in the graph. Each row and column of the matrix corresponds to a node in the graph, and the value at a given row and column indicates whether there is an edge between the two nodes. This representation is useful when the number of edges in the graph is large and the graph is dense (i.e. there are many edges relative to the number of nodes).
-   Adjacency list: an adjacency list is a list of nodes, where each node has a list of its neighboring nodes (i.e. the nodes it is connected to by an edge). This representation is useful when the number of edges in the graph is small and the graph is sparse (i.e. there are few edges relative to the number of nodes).

## Undirected and directed graphs

A graph is undirected if the edges in the graph do not have a specific starting and ending node. This means that an edge between two nodes in an undirected graph can be traversed in either direction.

A graph is directed if the edges in the graph have a specific starting and ending node. This means that an edge between two nodes in a directed graph can only be traversed in the direction specified by the edge.

## Unweighted and weighted graphs

A graph is unweighted if the edges in the graph do not have a numeric value associated with them. This means that all edges in an unweighted graph have the same "weight" or "cost".

A graph is weighted if the edges in the graph have a numeric value associated with them. This means that different edges in a weighted graph may have different "weights" or "costs". The weight or cost of an edge may represent the distance between the nodes, the time required to traverse the edge, or some other quantity.

## Depth-first search

Depth-first search (DFS) is a graph traversal algorithm that starts at a given node and explores as far as possible along each branch before backtracking. DFS can be implemented using a recursive function or using an explicit stack to keep track of the nodes that have been visited.

## Breadth-first search

Breadth-first search (BFS) is a graph traversal algorithm that starts at a given node and explores the neighbor nodes first, before moving on to the next level neighbors. BFS can be implemented using a queue to keep track of the nodes that have been visited.

## Topological sort

Topological sort is a graph algorithm that arranges the nodes in a directed acyclic graph (DAG) in a linear order such that if there is an edge from node A to node B, then node A appears before node B in the order. This can be useful for scheduling tasks or for determining the dependencies between different items in a system.

## Euler circuits and paths

An Euler circuit is a path in a graph that visits every edge exactly once and ends at the starting node. An Euler path is a path in a graph that visits every edge exactly once, but does not necessarily end at the starting node. Both Euler circuits and paths can only exist in graphs that are connected and have no more than two nodes with an odd degree (i.e. an odd number of edges connected to the node).

## Shortest path

The shortest path between two nodes in a graph is the path with the minimum total weight or cost. There are two main algorithms for finding the shortest path in a graph:

-   Unweighted shortest path: the unweighted shortest path can be found using breadth-first search (BFS) on an unweighted graph. This algorithm is efficient because it explores the nodes in the graph in increasing order of distance from the starting node, so the first time a given node is visited is when the shortest path to that node has been found.
-   Weighted shortest path: the weighted shortest path can be found using Dijkstra's algorithm on a weighted graph. This algorithm is more complex than BFS, but it can handle graphs with weighted edges and can find the shortest path even if there are negative edge weights.

## Connectivity

A graph is strongly connected if there is a directed path between every pair of nodes in the graph. A graph is weakly connected if there is an undirected path between every pair of nodes in the graph.

## Minimum spanning trees

A minimum spanning tree (MST) is a subset of the edges in a graph that connects all the nodes in the graph with the minimum total weight. There are two main algorithms for finding the minimum spanning tree in a graph:

-   Prim's algorithm: Prim's algorithm is a greedy algorithm that starts at a given node and adds the minimum-weight edge to the MST at each step, until all the nodes in the graph are included in the MST. This algorithm can be implemented using a priority queue to keep track of the edges that have not yet been added to the MST.
-   Kruskal's algorithm: Kruskal's algorithm is a greedy algorithm that adds the minimum-weight edge to the MST at each step, as long as the edge does not form a cycle with the edges already in the MST. This algorithm can be implemented using a disjoint-set data structure to keep track of the nodes that have been included in the MST.
