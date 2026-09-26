---
tags:
  - Statement
  - Finite
---
**Notation.** Let $\mathbb{P} = (P, \leq)$ be a *finite* [[Partial Order|poset]] and $X \subseteq P$, then $\# A_\mathbb{P}(X)$ is the number of [[Antichain|antichains]] in $(X, \leq|_{X \times X})$. If $\mathbb{P}$ is the only order in consideration we would write, for simplicity, just $\#A(X)$.

**Statement.** Let $\mathbb{P} = (P, \leq)$ be a *finite* order. Then for any $p \in P$ we have $\#A(P) = \#A(P \setminus \{p\}) - \#A(P \setminus \mathord{\updownarrow} p)$.
$\blacktriangle$ Let's call $n := \#A(P)$, $n_1 := \#A(P \setminus \{p\})$ and $n_2 := \#A(P \setminus \mathord{\updownarrow} p)$.
Now let's go through every subset of $X \subseteq P$ and see how it contributes to both sides of sides of the equation.
1. If $X$ is not an antichain, it is counted in neither $n$, nor $n_1$, nor $n_2$
2. If $X$ is an antichain it is counted in $n$, but there are different cases about the right side of the equation:
	1. $p \in X$ — counted in neither $n_1$ nor $n_2$, so we must count it somewhere later
	2. $p \notin X$ and $X \cap \mathord{\updownarrow}p = \emptyset$ — counted once in both in $n_1$ and $n_2$, we may say once for $X$ and once is for $X \cup \{p\}$ (which wasn't counted in 2.1.). And $X \cup \{p\}$ should be counted, because it is an antichain, exactly due to the fact $X \cup \mathord{\updownarrow} p = \emptyset$
	3. $p \notin X$ and $X \cap \mathord{\updownarrow}p \neq \emptyset$ — counted only in $n_1$, and we have no need to count $X \cup \{p\}$, because it's not an antichain, which is guaranteed by $X \cap \mathord{\updownarrow}p \neq \emptyset$ $\boxtimes$

**Examples.**
1. ![[Number of Antichains through Subposets Example 01.png|300]]
2. ![[Number of Antichains through Subposets Example 02.png|650]]


**Source.** Exercise 2-25a from @schroderOrderedSetsIntroduction2016.