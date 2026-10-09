---
tags:
  - Graph-Theory
  - Definition
---
**Definition.** Let $\mathbb{G} = (G, E)$ be a [[Graph|graph]]. A vertex $v \in G$ is called a <u>simplicial vertex</u> if $N[v]$, the [[Neighborhood of Vertex|closed neighborhood]] of $v$, is a [[Complete Graph (Clique)|clique]] of $\mathbb{G}$.

**Definition.** Let $\mathbb{G} = (G, E)$ be a [[Graph|graph]], $C \subseteq G$ – a clique of $\mathbb{G}$, $v \in G$. Then $C$ is called a <u>simplicial clique of </u>$v$ if $C = N[v]$.

**Definition.** Let $\mathbb{G} = (G, E)$ be a [[Graph|graph]], $C \subseteq G$ – a clique of $\mathbb{G}$. Then $C$ is called a <u>simplicial clique</u> if there exists a vertex $v \in G$ s.t. $C = N[v]$.

TODO Examples

**Statement.** A same clique can be a simplicial clique of different vertices. For example, consider a [[Complete Graph (Clique)|complete graph]] on 5 vertices $\mathbb{K}_5 = (K, E)$ – here for any $v \in K$ we have the whole $K$ as a simplicial clique of $v$.