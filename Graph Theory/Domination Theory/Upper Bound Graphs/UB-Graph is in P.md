---
tags:
  - Graph-Theory
  - Computatuional-Complexity
  - Finite
  - Statement
---
**Statement.** Class of finite [[Upper Bound Graph|UB-graphs]] is recognized in polynomial time.
$\blacktriangle$ Let $\mathbb{G} = (G, E)$ be a finite UB-graph. Then, by [[Finite UB-Graphs through Simpliciality|criterion]] we need to verify that every edge is in some [[Simplicial Vertices and Cliques|simplicial clique]]. We can find all the [[Simplicial Vertices and Cliques|simplicial vertices]] by $O(n^3)$ time directly following a definition. Now for every [[Graph|edge]] $(u,v)$ we look through all the simplicial vertices $s$ to find the one with $u,v \in N[s]$. If such found, then edge is covered by a simplicial clique, move to the next. Else return false. The total time is $O(n^3)$, the total memory is $O(n^2)$ including the adjacency matrix. $\boxtimes$

TODO add references to computational complexity
TODO add reference to the adjacency matrix