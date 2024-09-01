# Graph and Heap Data Structures in Java

## Overview

This project implements a graph data structure and a custom generic heap in Java. It is designed to perform various operations on graphs, including the computation of the shortest path using Dijkstra's algorithm. The custom heap structure is used to optimize the priority queue operations required by the Dijkstra algorithm.

## Features

### Graph_M.java
- **Graph Representation**: The graph is represented using an adjacency list.
- **Dijkstra's Algorithm**: Computes the shortest path between two nodes in the graph. The algorithm is implemented using a priority queue backed by a custom heap.
- **Vertex and Edge Management**: Supports adding vertices and edges to the graph.

### Heap.java
- **Generic Heap Implementation**: A generic heap that supports basic operations such as `add`, `remove`, `updatePriority`, and `get`.
- **Priority Queue Operations**: The heap is used to efficiently manage priority queues for algorithms like Dijkstra's.

## Usage

1. **Graph Operations**: 
   - You can add vertices and edges to the graph, and then compute the shortest path between any two vertices using Dijkstra's algorithm.
   - Example operations include:
     - Adding a vertex: `addVertex(String vname)`
     - Adding an edge: `addEdge(String v1, String v2, int cost)`
     - Running Dijkstra's algorithm: `dijkstra(String src, String des, boolean nan)`

2. **Heap Operations**:
   - Use the heap to manage a collection of elements with priority.
   - Operations include:
     - Adding an element: `add(T item)`
     - Removing the highest priority element: `remove()`
     - Updating the priority of an element: `updatePriority(T pair)`

## Code Example

```java
// Example of using the Graph and Heap classes

Graph_M graph = new Graph_M();
graph.addVertex("A");
graph.addVertex("B");
graph.addEdge("A", "B", 5);

int shortestPath = graph.dijkstra("A", "B", false);
System.out.println("Shortest Path from A to B: " + shortestPath);
# Metro-Graph-Navigator
