# summery 

## Graphs
![graph](https://ucarecdn.com/827083d1-3afc-444e-a94a-a8c239b9a76c/)

A graph is a pictorial representation of a set of objects where some pairs of objects are connected by links. The interconnected objects are represented by points termed as vertices, and the links that connect the vertices are called edges. The various terms and functionalities associated with a graph is described in great detail in our tutorial here. In this chapter we are going to see how to create a graph and add various data elements to it using a python program. 

Graphs are networks consisting of nodes connected by edges or arcs. In directed graphs, the connections between nodes have a direction, and are called arcs; in undirected graphs, the connections have no direction and are called edges. We mainly discuss directed graphs. Algorithms in graphs include finding a path between two nodes, finding the shortest path between two nodes, determining cycles in the graph (a cycle is a non-empty path from a node to itself), finding a path that reaches all nodes (the famous "traveling salesman problem"), and so on. Sometimes the nodes or arcs of a graph have weights or costs associated with them, and we are interested in finding the cheapest path.

Graphs are used to represent many real-life applications: Graphs are used to represent networks. The networks may include paths in a city or telephone network or circuit network. Graphs are also used in social networks like linkedIn, Facebook. For example, in Facebook, each person is represented with a vertex(or node). Each node is a structure and contains information like person id, name, gender, and locale. See this for more applications of graph.

**Here is some common terminology used when working with Graphs:**

1. **Vertex** - A vertex, also called a “node”, is a data object that can have zero or more adjacent vertices.
2. **Edge** - An edge is a connection between two nodes.
3. **Neighbor** - The neighbors of a node are its adjacent nodes, i.e., are connected via an edge.
4. **Degree** - The degree of a vertex is the number of edges connected to that vertex.

## Directed and Undirected Graphs

**Undirected graphs** have edges that do not have a direction. The edges indicate a two-way relationship, in that each edge can be traversed in both directions. This figure shows a simple undirected graph with three nodes and three edges.

![undirected](https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-35/resources/assets/UndirectedGraph.PNG)

The undirected graph we are looking at has 6 vertices and 7 undirected edges.

Vertices/Nodes = {a,b,c,d,e,f}

Edges = {(a,c),(a,d),(b,c),(b,f),(c,e),(d,e),(e,f)}

**Directed graphs** have edges with direction. The edges indicate a one-way relationship, in that each edge can only be traversed in a single direction. This figure shows a simple directed graph with three nodes and two edges.

![directed](https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-35/resources/assets/DirectedGraph.PNG)

The directed graph above has six vertices and eight directed edges

Vertices = {a,b,c,d,e,f}

Edges = {(a,c),(b,c),(b,f),(c,e),(d,a),(d,e)(e,c)(e,f)}


**Remark**: Usually, a Python dictionary throws a KeyError if you try to get an item with a key that is not currently in the dictionary. defaultdict allows that if a key is not found in the dictionary, then instead of a KeyError being thrown, a new entry is created. The type of this new entry is given by the argument of defaultdict. 

```python
from collections import defaultdict
 
# function for adding edge to graph
graph = defaultdict(list)
def addEdge(graph,u,v):
    graph[u].append(v)
 
# definition of function
def generate_edges(graph):
    edges = []
 
    # for each node in graph
    for node in graph:
         
        # for each neighbour node of a single node
        for neighbour in graph[node]:
             
            # if edge exists then append
            edges.append((node, neighbour))
    return edges
 
# declaration of graph as dictionary
addEdge(graph,'a','c')
addEdge(graph,'b','c')
addEdge(graph,'b','e')
addEdge(graph,'c','d')
addEdge(graph,'c','e')
addEdge(graph,'c','a')
addEdge(graph,'c','b')
addEdge(graph,'e','b')
addEdge(graph,'d','c')
addEdge(graph,'e','c')
 
# Driver Function call 
# to print generated graph
print(generate_edges(graph)) 

```
Outpuy:

```
[('a', 'c'), ('c', 'd'), ('c', 'e'), ('c', 'a'), ('c', 'b'), 
('b', 'c'), ('b', 'e'), ('e', 'b'), ('e', 'c'), ('d', 'c')]
```

