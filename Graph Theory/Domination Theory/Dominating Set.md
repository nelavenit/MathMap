---
tags:
  - Graph-Theory
  - Definition
---
**Definition.** Let $\mathbb{G} = (G, E)$ be a [[Graph|graph]], then $D \subseteq G$ is called a <u>dominating set of </u>$\mathbb{G}$ if every vertex from $G \setminus D$ is adjacent with some vertex of $D$. In other words, if $\bigcup\limits_{d \in D} N[d] = G$.

**Definition.** Let $\mathbb{G} = (G, E)$ be a graph, then $D \subseteq G$ – a dominating set of $\mathbb{G}$ is called <u>minimal</u> if there is no $D'$ such that $D \subsetneq D' \subseteq G$ and $D'$ is a dominating set of $\mathbb{G}$. In other words, $D$ is a [[Minimal and Maximal Elements|minimal element]] in the order of all the dominating sets of $\mathbb{G}$ ordered by inclusion.

**Remark.** Minimal dominating set need not be minimal in cardinality.


TODO Examples