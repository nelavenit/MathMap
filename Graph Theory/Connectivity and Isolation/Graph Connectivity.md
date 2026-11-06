---
tags:
  - Graph-Theory
  - Definition
---
**Definition.** A [[Graph|graph]] $\mathbb{G} = (G, E)$ is called to be <u>connected</u> if $G \neq \emptyset$ and for every vertices $u,v \in G$ there is a [[Path|path]] in $\mathbb{G}$ with $u,v$ as its endpoints. Else it's called to be disconnected.

**Definition.** Let $\mathbb{G} = (G, E)$ be a graph, then $S \subseteq G$ is called to be <u>connected in </u>$\mathbb{G}$ if [[Induced Subgraph|induced subgraph]] $\mathbb{G}|_S$ is connected.

**Definition.** Let $\mathbb{G} = (G, E)$ be a graph. A set $S \subseteq G$ is called a <u>connected component of </u>$\mathbb{G}$ if it's maximal by inclusion among the sets connected in $\mathbb{G}$.

TODO Verify paths of length 0 are correct
TODO Verify endpoints are defined
TODO the Poset connectivity in similar way (combine two notes)