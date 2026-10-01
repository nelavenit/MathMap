---
tags:
  - Definition
---
**Intuition.** [[Partial Order|Ordering]] is a "hierarchy" structure on a set, so it is natural to consider "hierarchy levels" of elements, similar to set ranks in set theory — we define an element rank. The properties we want from rank are:
1. If $p_1 < p_2$, then $rank(p_1) < rank(p_2)$, i.e. rank is a [[Strict Order Homomorphism|strict homomorphism]] from $\mathbb{P}$ to $\mathbb{N}$ with a natural ordering.
2. Rank is minimized. Else, for example, for an every finite or countable order we can give every element unique rank by considering a [[Linear Order (Chain)|linear]] extension of an order, which is always possible by [[Every Poset can be Extended to Linear One]], and then no two elements would be on the same "hierarchy level", which is very different from what we usually see in specific [[Hasse Diagram|Hasse diagrams]].

**Definition.** Let $\mathbb{P}=(P,\leq)$ be a *finite* poset, $p \in P$. We define the rank of $p$ (denoted as $\text{rank}_\mathbb{P}(p)$) recursively as follows:  
1. If $p$ is [[Minimal and Maximal Elements|minimal]] then $\text{rank}_\mathbb{P}(p) := 0$  
2. If the elements of $rank_\mathbb{P}$ $<n$ have been determined and $p$ is minimal in $P \setminus \{q \in P \mid \text{rank}_\mathbb{P}(q) < n\},$ then $\text{rank}_\mathbb{P}(p) := n$

**Notation.** If the order in consideration is obvious from the context we would denote rank $rank(p)$ instead of $rank_\mathbb{P}(p)$ for simplicity of notation.

**Statement (Equivalent definition of a rank).** Let $P=(P,\leq)$ be a *finite* poset and $p\in P$.
The rank of $p$ is the [[Chain Length|length]] of the longest [[Linear Order (Chain)|chain]] in $P$ that has $p$ as its [[Least and Greatest Elements|greatest element]].
$\color{red}\text{Proof idea:}$ induction on $\text{rank}(p)$.

**Examples.** 
1. ![[Rank Example 01.png|200]]
2. ![[Rank Example 02.png|300]]

**Intuition.** Rank can be used to
1. Somewhat standardize the Hasse diagram of an order, see [[Rank Hasse Diagram]]
2. Prove by induction, as in the proof of equivalent definition of a $rank$

**Remark.** The definition of a rank is also sensible for some *infinite* orders, for those $\mathbb{P} = (P, \leq_P)$, where for all $p \in P$ we have $\exists n \in \mathbb{N}$ s.t. $p$ is the greatest in a chain of $n$ elements, and for every longer chain it is not the greatest.
**Examples.** 
1. $\mathbb{N}$ with a natural ordering
2. ![[Rank Example 04 (on Continuum Order).png|400]]
3. ![[Rank Example 03.png|200]]
4. In $\mathbb{Z}$ with a natural ordering we can't assign ranks, because there are no candidates for $rank = 0$
5. In $\mathbb{Q}_{[0,1]}$ with a natural ordering we can't assign ranks: on a first step we get $rank(0) = 0)$, but there are no candidates for $rank = 1$, because $\mathbb{Q}_{(0,1]}$ has no minimal elements. Note: an order being [[Well-Founded Order|well-founded]] is not enough, consider $\mathbb{N} + \{\infty\}$.