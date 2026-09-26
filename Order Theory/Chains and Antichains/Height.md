---
tags:
  - Definition
---
**Intuition.** One of the natural ways to analyze finite (and some infinite) [[Partial Order|posets]] is to look at the height and width of their [[Hasse Diagram|Hasse diagram]]. Here we develop an idea of a height of an order, independent of the chosen Hasse diagram representation. Width idea is developed [[Width|here]].
In case of [[Rank Hasse Diagram]] the height is exactly the number or [[Rank|rank]] levels, i.e. maximal rank of an element + 1, and even in a general diagram case the height is lower-bounded by the maximal rank + 1, i.e. maximal rank reflects the smallest height of a diagram.

**Definition.** Let $\mathbb{P}$ be a poset. The <u>height</u> of $\mathbb{P}$ is the number of elements in the longest chain in $\mathbb{P}$. (in other words it's the ([[Chain Length|length]] of the longest chain in $\mathbb{P}$) + 1). We will denote it as $h(\mathbb{P})$. If for every natural number $n$, $\mathbb{P}$ has a chain of size $n$, then we will say $\mathbb{P}$ is of an infinite height.

**Statement.** Let $\mathbb{P} = (P, \leq)$ be a *finite* poset, then $h(\mathbb{P}) = \max\limits_{p \in P}(rank(p)) + 1$. 
$\blacktriangle$ Follows directly from an [[Rank|equivalent definition of an element rank]]. 

**Examples.**
1. ![[Order Height Example 01.png|315]]
2. ![[Order Height Example 02.png|368]]

**Statement.** Having a certain height is [[Self-dual Properties|self-dual]].

**Remark.** In some literature an order height is called a <u>length</u>.
**Remark.** Sometimes the height is defined as the [[Chain Length|length]] of the longest chain, i.e. $(\text{our height}) - 1.$ This may remove +1/-1 in some formulas, but add them in others.
Usually in literature it depends on the topic, for example if we discuss the pair of [[Dilworth's Chain Decomposition Theorem|Dilworth's chain]] and Mirsky antichain decompositions it would be nice to have "$w(\mathbb{P}) = n \implies n \text{ chains}$" and "$h(\mathbb{P}) = n \implies n \text{ antichains}$" pair. But, for example, while considering finite [[Powerset Lattice|powerset (boolean) lattices]] it may be more convenient to do the other convention for $h(B_n) = n$.
Here are some cases:

| Feature                                     |    $h_{elem}$ |  $h_{step}$ |
| ------------------------------------------- | ------------: | ----------: |
| Singleton / nonempty antichain              |           $1$ |         $0$ |
| 2-chain                                     |           $2$ |         $1$ |
| $n$-chain                                   |           $n$ |       $n-1$ |
| Powerset (boolean) lattice $B_n$            |         $n+1$ |         $n$ |
| Highest rank, when ranks start at $0$       |         $h-1$ |         $h$ |
| Number of rank levels                       |           $h$ |       $h+1$ |
| Mirsky: minimum # antichains in a partition |           $h$ |       $h+1$ |
| $P\times Q$                                 | $h(P)+h(Q)-1$ | $h(P)+h(Q)$ |
| $\dim\Delta(P)$, the order complex          |         $h-1$ |         $h$ |
TODO Add link to Mirsky antichain decomposition