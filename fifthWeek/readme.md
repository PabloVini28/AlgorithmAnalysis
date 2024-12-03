# Algorithm Analysis (PAA) 🖥️ 👨‍🔬 
## Graphs and Graph Traversal Algorithms 🌐
  - Definition:
    - A graph is a collection of nodes (vertices) and edges (connections between nodes). Graphs are widely used to represent networks, such as social networks, computer networks, or routes in maps. Traversing a graph refers to visiting all the vertices in a systematic way, and two common techniques for graph traversal are Breadth-First Search (BFS) and Depth-First Search (DFS).

## Breadth-First Search (BFS) 🌱
  - Definition:
    - BFS is an algorithm used to traverse or search through a graph in a level-by-level manner. It starts at the root (or an arbitrary node) and explores the neighbor nodes at the present depth level before moving on to nodes at the next depth level.
  - Steps:
    - Start at the initial node and enqueue it in a queue.
    - Dequeue a node, visit it, and enqueue all its unvisited neighbors.
    - Repeat the process until the queue is empty.
## Depth-First Search (DFS) 🌲
  - Definition:
    - DFS is an algorithm used to traverse or search through a graph by exploring as far down a branch as possible before backtracking. It starts at the root and explores each branch fully before moving on to another branch.

  - Steps:
    - Start at the initial node and push it onto the stack.
    - Pop a node from the stack, visit it, and push all its unvisited neighbors onto the stack.
    - Repeat the process until the stack is empty.
## Adjacency Matrix Representation of Graphs 🧮
  - Definition:
    - An adjacency matrix is a 2D array used to represent a graph. If there is an edge between vertex j, the matrix entry at 
[i][j] is 1 (or the weight of the edge if it’s a weighted graph), otherwise it’s 0. For an undirected graph, the matrix is symmetric.
  - Properties:
    - Space complexity: 
    - O(V^2), where V is the number of vertices.
    - Adjacency matrices are efficient for dense graphs (many edges), but not ideal for sparse graphs (few edges), as they use up more memory than adjacency lists.
    - Inserting or deleting an edge has constant time complexity: O(1).
