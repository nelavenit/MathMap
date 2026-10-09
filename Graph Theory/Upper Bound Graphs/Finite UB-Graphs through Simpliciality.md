---
tags:
  - Statement
  - Finite
  - Graph-Theory
---
**Definition.** Let $\mathbb{G} = (G, E)$ be a finite [[Graph|graph]], $\mathcal{K} = \{K_1, K_2, \ldots, K_k\}$ be a family of subsets of $G$. We say $\mathcal{K}$ <u>edge covers</u> $\mathbb{G}$ if for every edge $(u,v) \in E$ we have $K_i \in \mathcal{K}$ s.t. both $u \in K_i$ and $v \in K_i$. In other words, every edge is fully inside of at least one set of the family.

**Statement.** Let $\mathbb{G} = (G, E)$ be a finite graph. Then $\mathbb{G}$ is an [[Upper Bound Graph|upper bound graph]] iff every edge $e \in E$ lies in some [[Simplicial Vertices and Cliques|simplicial clique]] of $\mathbb{G}$.
$\blacktriangle$ **($\boldsymbol{\implies}$)** Let $\mathbb{P} = (G, \leq)$ be a [[Partial Order|poset]] s.t. $\mathbb{G} = \operatorname{UB}(\mathbb{P})$. Consider $M := \operatorname{Max}(\mathbb{P})$. Let's show that any $m \in M$ is a [[Simplicial Vertices and Cliques|simplicial vertex]] of $\mathbb{G}$ with $\downarrow_{\mathbb{P}}{m}$ as its simplicial clique:
1. $\downarrow_{\mathbb{P}} m$ is a [[Complete Graph (Clique)|clique]] of $\mathbb{G}$, because any two distinct elements of it have $m$ as their [[Lower and Upper Bounds|upper bound]], hence, are [[Graph|adjacent]] in $\mathbb{G} := \operatorname{UB}(\mathbb{P})$.
2. $m$ is maximal, so it has a common upper bound with another element $v \in G$ iff $v \leq m$. This is exactly $N_{\mathbb{G}}[m] = {\downarrow_{\mathbb{P}}m}$, hence $m$ is a simplicial vertex. 
Now consider an edge $(u,v) \in E$. By the definition of $E$ we have some upper bound of $\{u,v\}$, now take any maximal element $m$ that is above this upper bound. It exists by finiteness of $G$ and is also an upper bound of $\{u,v\}$. Hence, edge $(u,v)$ lies in $\downarrow_{\mathbb{P}}{m}$, which is a simplicial clique, as proved before.
$(\impliedby)$ Same idea of $\mathrm{Max}(\mathbb{P}) = \{\text{some simplicial vertices}\}$, but in reverse.
Let $\mathcal{K}$ be the family of all distinct simplicial cliques of $\mathbb{G}$. By assumption, $\mathcal{K}$ edge covers $\mathbb{G}$. It also covers $G$, since every non-isolated vertex belongs to an edge and every isolated vertex forms a simplicial clique.
For each $K \in \mathcal{K}$, choose a representing simplicial vertex $m_K$, and put $M := \{m_K : K \in \mathcal{K}\}.$ 
Each $m_K$ belongs to no other member of $\mathcal{K}$, (consider [[Simplicial Vertex Criterion|simplicial vertex criterion]] (2) + (4)).
Define $\leq$ on $G$ by
$$
u < v
\overset{\mathrm{def.}}{\iff}
v \in M \land u \in N_{\mathbb{G}}(v).
$$
$$u \leq v \overset{\mathrm{def.}}{\iff} u < v\ \lor \ u = v$$
This relation is [[Reflexivity|reflexive]]. By the representative property above, every strict comparison goes from $G \setminus M$ to $M$. Thus reverse strict comparisons and consecutive strict comparisons are impossible. Consequently, $\leq$ is [[Antisymmetry|antisymmetric]] and [[Transitivity|transitive]], so $\mathbb{P} := (G,\leq)$ is a poset.
Now let's show $\mathbb{G} = \mathrm{UB}(\mathbb{P})$. 
$(\subseteq)$ Let $(u,v) \in E$. Then, by assumption, there exists a simplicial clique $K \in \mathcal{K}$ s.t. $u,v \in K$. Hence, $m_K \in M$, hence $u \leq m_K$ and $v \leq m_K$, by definition of $\leq$, and this means $m_K$ is an upper bound of $u$ and $v$. So these vertices are adjacent in $\mathrm{UB}(\mathbb{P})$ too.
$(\supseteq)$ Let $(u,v)$ be an edge of $\mathrm{UB}(\mathbb{P})$, then $u \neq v$ by irreflexivity of a graph. Then they have an upper bound $m$, $(u \neq v)$ + $(u \leq m)$ + $(v \leq m)$ gives us that at least one of $u < m$ and $v < m$ is true. Consequently, by the definition of $<$ we have $m$ being a representative of some $K$ – simplicial clique of $\mathbb{G}$. Hence, $u$ and $v$ both lie in $K$ by def. of $\leq$. Hence $(u,v) \in E$. $\boxtimes$

**Equivalent formulation 1.** Let $\mathbb{G} = (G, E)$ be a finite graph. Then $\mathbb{G}$ is a UB-graph iff there exists a family $\mathcal{K} = \{K_1, K_2, \ldots, K_k\}$ of simplicial cliques of $\mathbb{G}$ s.t. $\mathcal{K}$ edge covers $\mathbb{G}$. 
$\blacktriangle$ This is simply an unwind of the "lies in some simplicial clique".

**Equivalent formulation 2.** Let $\mathbb{G} = (G, E)$ be a finite graph. Then $\mathbb{G}$ is a UB-graph iff there exists a family $\mathcal{K} = \{K_1, K_2, \ldots, K_k\}$ of cliques of $\mathbb{G}$ s.t.:
1. $\mathcal{K}$ edge covers $\mathbb{G}$
2. For every $K_i \in \mathcal{K}$ exists such $x_i \in K_i$ that it is not present in any other clique of $\mathcal{K}$. In other words, $\forall i=1\ldots k\ \exists x_i \in K_i \setminus \bigcup\limits_{j \neq i} K_j$.
$\blacktriangle$ This is an equivalent formulation 1 with [[Simplicial Clique Criterion|simplicial clique criterion]] applied.

**Remark.** The theorem is simply a paraphrase of Th.1 from @mcmorrisBoundGraphsPartially1982 in the terms of the simpliciality  and applying [[Simplicial Clique Criterion|simplicial clique criterion]]. The equivalent formulation 2 is exactly the original result.

TODO Reference to Isolated vertex