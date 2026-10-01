---
tags:
  - Definition
---
**Intuition.** One of the natural ways to analyze finite (and some infinite) [[Partial Order|posets]] is to look at the height and width of their [[Hasse Diagram|Hasse diagram]]. Here we develop an idea of a width of an order, independent of the chosen Hasse diagram representation. Height idea is developed [[Height|here]].
In case of [[Rank Hasse Diagram]] the width is lower bounded by the maximum size of a [[Rank|rank]] level, which is also a lower bound for the size of the [[Maximal Antichain|maximal antichain]], because all the elements of the same rank are incomparable. It is one of the intuitions for the following definition.

**Definition.** Let $\mathbb{P} = (P, \leq)$ be a poset. We call <u>width</u> of $\mathbb{P}$ the size of the largest [[Antichain|antichain]] in $\mathbb{P}$, if antichains of arbitrary size exist, we consider $\mathbb{P}$ to be of infinite width. We denote width by $w(\mathbb{P})$.

**Examples.**
1. ![[Width Example 01.png|200]]
2. ![[Width Example 02.png|250]]
3. ![[Width Example 03.png|200]]
4. $\mathbb{N}$ with a natural ordering has $w = 1$
5. ![[Width Example 04.png|200]]
6. $(\mathbb{N}, |)$ has a $w=\infty$, for instance $\{p \in \mathbb{N}\ |\ p - \text{prime}\}$ is an infinite antichain

**Intuition.** Width and antichains can't produce the analog for a rank: some horizontal ranking, because an antichain, unlike a [[Linear Order (Chain)|chain]], has no hierarchy on its elements.