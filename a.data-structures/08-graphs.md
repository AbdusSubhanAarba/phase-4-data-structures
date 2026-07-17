# Graphs

## Overview

A graph is a **non-linear data structure** that consists of **vertices (nodes)** connected by **edges**. Unlike trees, graphs have no fixed hierarchy. Any node can connect to one or many other nodes, making graphs ideal for representing relationships and networks.

Graphs are used in many real-world applications, including social media, navigation systems, computer networks, recommendation engines, and search algorithms.

---

## Why It Matters

Graphs are important because they:

- Represent relationships between objects
- Model complex networks
- Help find the shortest path between locations
- Support route planning and navigation
- Power recommendation systems
- Are widely used in artificial intelligence and networking

Many modern applications rely heavily on graph data structures.

---

## How a Graph Works

A graph consists of:

- **Vertices (Nodes)** → The objects or points.
- **Edges** → The connections between those objects.

Example:

```text
      A
     / \
    B---C
     \
      D
```

In this graph:

- A, B, C, and D are **vertices**.
- The lines connecting them are **edges**.

---

## Graph Terminology

### Vertex (Node)

A vertex is an individual point in a graph.

Example:

```text
A
```

Every graph contains one or more vertices.

---

### Edge

An edge connects two vertices.

Example:

```text
A ------- B
```

The line represents an edge.

---

### Neighbor (Adjacent Vertex)

Two vertices connected by an edge are called **neighbors**.

Example:

```text
A ------- B
```

A and B are neighbors.

---

### Path

A path is a sequence of connected vertices.

Example:

```text
A → B → C → D
```

---

### Cycle

A cycle occurs when a path starts and ends at the same vertex.

Example:

```text
A
| \
|  \
C---B
```

Starting at A:

```text
A → B → C → A
```

This forms a cycle.

---

## Types of Graphs

### Undirected Graph

Connections work in both directions.

Example:

```text
A ----- B
```

If A connects to B, then B also connects to A.

---

### Directed Graph

Connections have a direction.

Example:

```text
A -----> B
```

Here, the connection goes only from A to B.

Directed graphs are often used to represent one-way relationships.

---

### Weighted Graph

Each edge has a value or cost.

Example:

```text
A ----5---- B
 \          /
  \3      2/
    \     /
      C
```

The numbers may represent:

- Distance
- Time
- Cost
- Traffic
- Network latency

---

## Graph Traversal

Traversal means visiting every vertex in a graph.

Two common graph traversal algorithms are:

### Breadth-First Search (BFS)

Visits nearby vertices first before moving farther away.

Example:

```text
A

↓

B, C

↓

D, E
```

BFS is useful for finding the shortest path in many unweighted graphs.

---

### Depth-First Search (DFS)

Explores one path as deeply as possible before backtracking.

Example:

```text
A

↓

B

↓

D

↓

Back to B

↓

C
```

DFS is useful for searching, maze solving, and graph analysis.

---

## Graph Representation

Graphs are commonly stored in two ways.

### Adjacency List

Stores each vertex along with its neighboring vertices.

Example:

```text
A → B, C

B → A, D

C → A

D → B
```

This method is memory-efficient for sparse graphs.

---

### Adjacency Matrix

Uses a table to show whether two vertices are connected.

Example:

```text
      A B C

A     0 1 1

B     1 0 0

C     1 0 0
```

A value of **1** indicates a connection.

---

## Advantages of Graphs

Graphs provide several benefits:

- Represent complex relationships
- Model real-world networks
- Support efficient pathfinding
- Flexible structure
- Highly scalable

---

## Disadvantages of Graphs

Graphs also have some limitations:

- More complex than linear data structures
- Traversal algorithms can be challenging
- Large graphs may require significant memory
- Some graph algorithms are computationally expensive

---

## Real-World Examples

Graphs are used in countless applications.

### Google Maps

Cities are vertices.

Roads are edges.

Graph algorithms calculate the fastest route.

---

### Social Media

Users are vertices.

Friendships or followers are edges.

Platforms like Facebook, LinkedIn, and Instagram use graph structures.

---

### Computer Networks

Devices are vertices.

Network connections are edges.

Graphs help determine the best route for data.

---

### Flight Routes

Airports are vertices.

Flights between airports are edges.

Airline systems use graphs to plan routes.

---

### Recommendation Systems

Streaming platforms connect:

- Users
- Movies
- Music
- Products

Graphs help recommend content based on relationships.

---

## Time Complexity

The performance of graph operations depends on the algorithm used.

Common traversal algorithms:

| Operation | Time Complexity |
|-----------|----------------:|
| Breadth-First Search (BFS) | O(V + E) |
| Depth-First Search (DFS) | O(V + E) |

Where:

- **V** = Number of vertices
- **E** = Number of edges

---

## Trees vs Graphs

| Trees | Graphs |
|-------|--------|
| Hierarchical structure | Network structure |
| One root node | No required root |
| No cycles | Cycles may exist |
| One path between nodes | Multiple paths may exist |
| Parent-child relationships | General relationships |

A tree is actually a special type of graph.

---

## Common Mistakes Beginners Make

Beginners often:

- Confuse graphs with trees.
- Assume every graph has a root node.
- Forget that graphs can contain cycles.
- Think every graph is directed.
- Ignore the difference between vertices and edges.

Understanding relationships between nodes is the key to mastering graphs.

---

## Key Takeaways

- A graph is a non-linear data structure made of **vertices** and **edges**.
- Graphs represent relationships between objects.
- Graphs can be directed, undirected, or weighted.
- Common traversal algorithms are **BFS** and **DFS**.
- Graphs are widely used in navigation, networking, social media, and recommendation systems.

---

## Summary

Graphs are one of the most versatile and powerful data structures in computer science. They model relationships between objects and enable efficient pathfinding, networking, and data analysis. From Google Maps and social media to airline routes and computer networks, graphs are used extensively in modern software engineering to solve complex real-world problems.
