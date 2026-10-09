---
tags:
  - Statement
  - Graph-Theory
---
**Statement (finite case).** Let $\mathbb{G} = (G, E)$ be a finite [[Graph|graph]], $v \in G$, then the following are equivalent:
1. $v$ is a [[Simplicial Vertices and Cliques|simplicial vertex]], i.e. $N[v]$ is a [[Complete Graph (Clique)|clique]]
2. $N[v]$ is a maximal clique of $\mathbb{G}$
3. The [[Neighborhood of Vertex|open neighborhood]] $N(v)$ is a clique of $\mathbb{G}$
4. $v$ belongs to exactly one maximal clique of $\mathbb{G}$
5. $v$ is not the middle vertex of any induced subgraph path on three vertices. 
$\blacktriangle$ **(1 $\boldsymbol{\Rightarrow}$ 2)** trivial
**(2 $\boldsymbol{\Rightarrow}$ 3)** $N(v)$ is a clique $\implies$ $N[v]$ is a clique (and a simplicial one) $\implies$(by [[Simplicial Clique is Maximal|here]]) $N[v]$ is a maximal clique. Assume there is another $C \subseteq G$ – maximal clique of $\mathbb{G}$ with $v \in C$. Then $C \subseteq N[v]$, else it's not a clique, because $v$ wouldn't be adjacent to some vertex of $C$, then either $C = N[v]$ or $C$ is not maximal.
**(3 $\boldsymbol{\Rightarrow}$ 1)** 

**Statement (General case in ZF).** 
**Statement (General case in ZFC).** 

TODO Link to PATH