---
tags:
  - Statement
  - Finite
---
**Statement.** The $n$<sup>th</sup> [[Dedekind Numbers|Dedekind number]] is at least $2^{\displaystyle \binom{n}{\lfloor \frac{n}{2} \rfloor}}$.
$\blacktriangle$ Let's just consider elements of the same [[Rank|rank]] in the [[Powerset Lattice|powerset lattice]], they all are incomparable, so for any $k$ any subset of $\{p \in \mathcal{P}(\{1,\ldots,n\})|rank(p) = k\}$ is an [[Antichain|antichain]]. This way we get a lower bound of $\max\limits_{k \in \mathbb{N}} (2^{\text{number of elements of the rank }k})$. By [[Rank in Finite Powerset Lattice]] we know the $k$-th layer is exactly all the subsets of the size $k$, and there are exactly $\displaystyle \binom{n}{k}$ of them. Then it's a simple exercise to see the maximum is when $k = \lfloor n \rfloor$. $\boxtimes$

**Intuition.** It gives the lower bound of a double exponent, which is huge, and we didn't count "plentiful" of antichains.