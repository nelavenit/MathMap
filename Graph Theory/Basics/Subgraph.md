---
tags:
  - Definition
  - Graph-Theory
---
**Definition.** Let $\mathbb{G} = (G, \leftrightarrow)$ be a [[Graph|graph]], $S \subseteq G$. Then a graph $(S, \leftrightarrow_S)$ is called a <u>subgraph</u> of $\mathbb{G}$, if ${\leftrightarrow_S} \subseteq {\leftrightarrow}|_{S \times S}$, i.e. it is a subset of $G$ with some edges of $\leftrightarrow$ and no other edges.

**Examples.** Consider the following graph ![[Subgraph Example 01.png|103]], here are its different subgraphs
1. ![[Subgraph Example 02.png]]
2. ![[Subgraph Example 03.png|139]]
3. ![[Subgraph Example 04.png]]
4. ![[Subgraph Example 05.png]]
5. Every induced subgraph is a subgraph

**Remark.** Different from induced subgraph and [[Subposet|subposet]], where no relations/edges removal is allowed.