
----
### Graphs
A graph G is an ordered pair of vertex nonempty set V and edge set E, denoted as G(V,E), where
	V is a finite non-empty set of objects.
	E is a two element subset of V.

This is a simple undirected graph.

#### Order
Number of vertices in a graph.
#### Size
Number of edges in a graph.

----
### Adjacent edges
Vertices $u,v\in V$ are said to be adjacent to each other if edge  $uv\in E$.

### Joined
If $uv\in E$ then vertices u and v are said to be joined by edge uv.

### Neighbours
Vertices $u,v\in V$ are said to be neighbours if they are joined by some edge.

### Incident
If an edge $e\in E$ pairs vertex $v\in V$ with some other vertex then e and v are said to be incident with each other.

### Adjacent edges
If edges are incident on a common vertex then they are said to be ajacent edges.

### Connected vertices
If there exists a path between them.

----
### Trivial graph
A graph with order 1.

### Non-Trivial graph
A graph with order greater than 1.


### Labelled graph
A graph with vertices labelled.
- Used when we are interested with just the structure of the graph.

### Unlabelled graph
A graph with no labelling.


### Subgraph of graph G
$H(V',E')$ such that $V'\subseteq V(G)\ and\ E'\subseteq E(G)$ 
- G contains H shown as $H\subseteq G$.
- Drop some vertices or edges to get H from G or let it be as it is.

#### Proper subgraph
A subgraph $H\subseteq G$ such that either $V(H)\subset V(G)$ or $E(H)\subset E(G)$.
- Drop some vertices or edges to get H from G.

### Spanning subgraph of G
A subgraph $H\subseteq G$ such that $V(H)=V(G)$ and $E(H)\subset E(G)$.
- Drop some edges from G to get H.
- G is a spanning subgraph of G+e, for some new edge e.

### Induced subgraph of G
A subgraph $F\in G$ such that for vertices $u,v\in V(F)$ if $uv\in E(G)$ then $uv\in E(F)$.

#### Vertex induced subgraph of G
If S is a nonempty subset of V(G), then the induced subgraph of G by S is an induced subgraph with vertex set S and is denoted as G\[S] or $<S>_G$
- For $U\subseteq V(G)$, G-U is the induced subgraph of G, induced by V(G)-U.

#### Edge induced subgraph of G
If X is a nonempty subset of E(G) then induced subgraph of G denoted as G\[X] or $<X>_G$ will have $E( G[X])=X$ and V(G\[X]) consists of all vertices of G that are incident with at least one edge in X.
-  For $X\subseteq E(G)$ G-X = spannig subgraph of G induced by E(G)-X.


### Connected graph
If every two vertices of G are connected, or G contains a u-v path for every vertices pair {u,v} of V(G).

### Disconnected graph
Which is not connected.

### Component of G
A connected subgraph of G which is not a proper subset of any another connected subgraph of G.
- Number of components of G is denoted as k(G).
- Connected graph G has k(G)=1.
- Every graph is union of its components.

----
### Walk
Sequence of vertices W such that consecutive vertices in the sequence are adjacent.
It can be expressed as: $W=\{u=v_0,v_1,v_2,...,v_k=v\}$ which is a u-v walk.

#### length of a walk
Number of edges in a walk.
#### Trivial walk
If the length of walk is 0.
#### Closed walk
If the first and the last vertices of walk are same, then it is a closed walk.
#### Open walk
If the first and the last vertices of walk are not same, then it is an open walk.

### Trail
A walk where edges doesnt repeat.

### Path
A walk where vertices doesnt repeat.

### Circuit
A closed trail.
- Begins and ends at the same vertex.
- In a simple graph it will have $length\geq3$

### Cycle
A circuit where no vertex repeats except the first and the last.
#### k-cycle
A cycle of length k.
#### Triangle
A 3-cycle.
#### Odd cycle
A cycle of odd length.
#### Even cycle
A cycle of even length.


----
Points:
- V and E are also represented as V(G) and E(G) respectively.
- $V\not=\phi$  => Order of every graphs is at least 1.
- Graphs G and H are equal if $V(G)=V(H) and E(G)=E(H).
- Word graph of the Set of Words: is a graph model G whose vertices are the words and two words are adjacent if they can be transformed into each other by any of following rules:
	1.  Interchanging two letters.
	2. Replacing a letter by another letter.
-  $paths\subseteq trail \subseteq walk$.
-  $cycle\subseteq circuit\subseteq trail \subseteq walk$.
- The vertices and edges of trail, path, circuit or cycle in G forms a subgraph.
