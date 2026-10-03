---
tags:
  - Statement
  - Finite
  - Graph-Theory
---
**Definition.** Let $\mathbb{G} = (G, E)$ be a graph, $\mathcal{K} = \{K_1, K_2, \ldots, K_k\}$ be a family of subsets of $G$. We say $\mathcal{K}$ <u>edge covers</u> $\mathbb{G}$ if for every edge $(u,v) \in E$ we have $K_i \in \mathcal{K}$ s.t. both $u \in K_i$ and $v \in K_i$. In other words, every edge is fully inside of at least one set of the family.

**Definition.** Let $\mathbb{G} = (G, E)$ be a finite [[Graph|graph]]. Then $\mathbb{G}$ is [[Upper Bound Graph|upper bound graph]] iff there exists a family $\mathcal{K} = \{K_1, K_2, \ldots, K_k\}$ of [[Complete Graph (Clique)|cliques]] of $\mathbb{G}$ s.t.:
1. $\mathcal{K}$ edge covers $\mathbb{G}$
2. 