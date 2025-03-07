# 🖥️ 👨‍🔬 Algorithm Analysis (PAA)
## Minimum Spanning Tree (MST) Problem 🌲
## 📌 Definition:
### A Minimum Spanning Tree (MST) is a subset of edges in a weighted, connected, and undirected graph that connects all vertices with the minimum possible total edge weight and without cycles. MSTs are essential in network design, clustering, and approximation algorithms.

## 🔍 Applications:
  - Network Design – Laying out telecommunication, electrical, or computer networks with minimal cost.
  - Image Processing – Used in image segmentation.
  - Cluster Analysis – Helps in organizing datasets into hierarchical clusters.
  - Shortest Path Problem 🛤️
## 📌 Definition:
### The Shortest Path Problem finds the minimum-cost path between two vertices in a weighted graph. This problem is fundamental in fields like navigation, routing, and AI pathfinding.

## 🔍 Applications:
  - GPS and Navigation Systems – Finding the fastest route between two locations.
  - Network Routing – Optimizing data transfer in communication networks.
  - AI Pathfinding – Used in robotics and game development.
  -  Kruskal’s Algorithm 🔗
## 📌 Definition:
### Kruskal’s algorithm is a greedy algorithm used to find an MST. It sorts edges by weight and adds the smallest edge while ensuring no cycles are formed.

## ⚡ Steps:
  - Sort all edges in ascending order of weight.
  - Start with an empty MST and process each edge in order:
  - If the edge does not create a cycle, add it to the MST.
  - Otherwise, discard it.
  - Repeat until the MST has (V - 1) edges (where V is the number of vertices).
## ⏳ Time Complexity:
  - O(E log E), where E is the number of edges (sorting step dominates).
## Prim’s Algorithm 🏗️
## 📌 Definition:
### Prim’s algorithm is another greedy algorithm to find an MST. Unlike Kruskal’s, Prim’s starts with a single vertex and grows the MST one edge at a time by adding the smallest adjacent edge.

## ⚡ Steps:
  - Choose any starting vertex and mark it as visited.
  - Find the smallest edge that connects a visited vertex to an unvisited one.
  - Add the edge to the MST and mark the new vertex as visited.
  - Repeat until all vertices are included in the MST.
## ⏳ Time Complexity:
  - Using a binary heap: O(E log V)
  - Using a simple adjacency matrix: O(V²)
