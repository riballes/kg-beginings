# Knowledge Graph Beginings

## Introduction

Before starting, we need to have a proper understanding of what a Graph is. A graph is a mathematical object we use to think about networks. It consists of a bunch of points, called __vertices (V)__ (also entities or nodes), and lines joining pairs of vertices, called __edges (E)__ (or relationships).

<p align="center">
  <img src="https://render.githubusercontent.com/render/math?math=\LARGE G = (V, E)">
</p>

Examples:

![image](https://user-images.githubusercontent.com/14939490/135533337-dd14a75b-1d5a-4733-8f7a-53fb8fdbfb53.png)

### Adjacency and Degree

• We say two vertices are __adjacent (or are neighbors)__ if they are joined by an edge, and non-adjacent otherwise.  
![image](https://user-images.githubusercontent.com/14939490/135536310-f6b5399d-2a27-4cdd-96cc-a1fe08c76277.png)

• We say an edge and a vertex are incident if the vertex is one of the endpoints of the edge. The __degree of a vertex 𝑣 is the number of edges incident with 𝑣__.  
![image](https://user-images.githubusercontent.com/14939490/135536401-e0069ec6-7eef-4228-bc21-5e9b50b5c4c5.png) in this case we will have <img src="https://render.githubusercontent.com/render/math?math=deg(v) = 3">
  

## Trees vs Graphs

A Tree is just a restricted form of a Graph.

Trees have direction (parent / child relationships) and don't contain cycles. They fit with in the category of __Directed Acyclic Graphs (or a DAG)__. So Trees are DAGs with the restriction that a child can only have one parent.

One thing that is important to point out. Trees aren't a recursive data structure. They can not be implemented as a recursive data structure because of the above restrictions. But any DAG implementation, which are generally not recursive, can also be used. My preferred Tree implementation is a centralized map representation and is non recursive.

