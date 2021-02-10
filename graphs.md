# Graphs

## Introduction
**_Graph_ is one the common used data structure which basely used in the Google Map or Apple Map. So the idea of it is that it's non-linear, each node has a different length.**

## Terminology
- **_Vertex_** is a node in the graph and it's an object data.
- **_Edge_** is the connection or link between each node in the graph.
- **_Neighbor_** is the nodes that are connected by the edge.
- **_Degree_** is the number of the edges that are connected to the vertex.

## Graph Types
- Undirected Graphs
***Means that the edge of the graph is bi-directional with 2 edges linked to it.***
![Undirected Graphs](https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-35/resources/assets/UndirectedGraph.PNG)

- Directed Graphs
***Means that each vertex has a completed edges in all the directions.***
![Directed Graphs](https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-35/resources/assets/DirectedGraph.PNG)

- Complete Graphs
***Means all the verices of the graph are connected to each other.***
![Complete Graphs](https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-35/resources/assets/CompleteGraph.PNG)

- Connected
***Means at least each vertex has a one edge.***
![Connected](https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-35/resources/assets/ConnectedGraph.PNG)

- Disconnected
***Where some of the vertices are not having an edge.***
![Disconnected](https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-35/resources/assets/DisconnectedGraph.PNG)

## Graph Representation
- Adjacency Matrix : the row axis will define a certain vertex and the column axis will show the connection between this vertex and the rest by giving it a value of one, those who are not connected, they will be giving it a zero.
![Adjacency Matrix](https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-35/resources/assets/AdjMatrix.PNG)

- Adjacency List : Best practice in the graph data structure and would take a less time and space by only passing for each vertex, their connected vertices.
![Adjacency List](https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-35/resources/assets/AdjList.PNG)