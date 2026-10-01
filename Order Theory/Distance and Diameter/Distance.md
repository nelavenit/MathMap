---
tags:
  - Definition
---
**Definition.**  Let $\mathbb{P} = (P, \leq)$ be a [[Partial Order|poset]], $p,q \in P$. The <u>distance</u> between $p$ and $q$, denoted by $\operatorname{dist}(p,q),$ is the [[Fence|length]] of the shortest [[Fence|fence]] in $\mathbb{P}$ with $p$ and $q$ as [[Fence|endpoints]]. If $p$ and $q$ are in different [[Connected component|connected components]] of $\mathbb{P}$, we will say the distance is infinite.

**Notation.** When there are multiple orders in consideration we may write $\operatorname{dist}_{\mathbb{P}}(p,q)$ for an unambiguity.

**Intuition.** Same as in the definition of the connected component here we use fence, not a [[Linear Order (Chain)|chain]], because else:
1. It wouldn't relate to the distance in the Hasse diagram
2. For most pairs the distance would be $\infty$
3. Triangle inequality wouldn't work
I.e. fence is an analog of the "simple path" in graph theory.


TODO Examples
TODO link to the graph simple path