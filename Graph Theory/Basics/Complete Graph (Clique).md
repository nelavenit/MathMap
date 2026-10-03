---
tags:
  - Definition
---
**Definition.** Let $\mathbb{G} = (G, E)$ be a [[Graph|graph]], it is called a <u>complete</u> graph or a <u>clique</u> if for any $x,y \in G$ we have $(x,y) \in E$.

**Notation.**  Let $\mathbb{G} = (G, E)$ be a graph, $S \subseteq G$ and the [[Induced Subgraph|subgraph induced by]] $S$ is complete. Then $S$ is called a <u>clique of </u>$\mathbb{G}$ or a <u>complete subgraph of </u>$\mathbb{G}$. 

**Statement.** For every set $G$, only a single relation gives a complete graph.
$\color{red}\text{Proof}$ is obvious.

**Notation.** An $n$-element clique is denoted as $K_n$.

**Examples.** 
1. A one point with empty relation is a complete graph – an only one-element clique – $K_1$
2. ![[K2.png|185]] – $K_2$
3. ![[K3.png|144]] – <u>triangle</u> – $K_3$
4. ![[K5.png|176]] – $K_5$
5. ![[K7.png|212]] – $K_7$
6. ![[P6.png|284]] – not a clique

**Remark.** Sometimes (for example @mcmorrisBoundGraphsPartially1982) a "clique" means "complete subgraph, that is maximal by inclusion"(i.e. can't be extended to a bigger complete subgraph). 