---
tags:
  - Definition
---
**Definition.** Let $\mathbb{G} = (G, E)$ be a [[Graph|graph]], it is called a <u>complete</u> graph or a <u>clique</u> if for any $x,y \in G$ we have $(x,y) \in E$.

**Statement.** For every set $G$, only a single relation on $G$ gives a complete graph.
$\color{red}\text{Proof}$ is obvious.

**Definition.** Let $\mathbb{G} = (G, E)$ be a graph, $K \subseteq G$ and the [[Induced Subgraph|subgraph induced by]] $K$ is complete. Then $K$ is called a <u>clique of </u>$\mathbb{G}$ or a <u>complete subgraph of </u>$\mathbb{G}$. 

**Definition.** Let $\mathbb{G} = (G, E)$ be a graph, then $K \subseteq G$ – clique of $\mathbb{G}$ is called <u>maximal</u> if there is no $K'$ such that $K \subsetneq K' \subseteq G$ and $K'$ is a clique of $\mathbb{G}$. In other words, $K$ is a [[Minimal and Maximal Elements|maximal element]] in the order of all the cliques of $\mathbb{G}$ ordered by inclusion.

**Notation.** An $n$-element clique is denoted as $K_n$.

**Examples.** 
1. A one point with empty relation is a complete graph – an only one-element clique – $K_1$
2. ![[K2.png|185]] – $K_2$
3. ![[K3.png|144]] – <u>triangle</u> – $K_3$
4. ![[K5.png|176]] – $K_5$
5. ![[K7.png|212]] – $K_7$
6. ![[P6.png|284]] – not a clique
7. $\emptyset$ is a clique of any graph 

TODO Examples of cliques of $\mathbb{G}$

**Remark.** A maximal clique need not be maximal in cardinality.

**Remark.** In some sources (for example @mcmorrisBoundGraphsPartially1982) a "clique" means "maximal clique". 