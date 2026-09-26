---
tags:
  - Statement
  - Finite
---
**Notation.** Let $\mathbb{P} = (P, \leq)$ be a *finite* [[Partial Order|poset]] and $X \subseteq P$, then $\#A(\mathbb{P})$ is number of [[Antichain|antichains]] in $\mathbb{P}$ and the $\# A_\mathbb{P}(X)$ is the number of antichains in $(X, \leq|_{X \times X})$. If $\mathbb{P}$ is the only order in consideration we would write, for simplicity, just $\#A(X)$.

**Intuition.** Note that the number of antichains is independent of the choice of an n-element [[Fence|fence]] (there are 4 of them), we may "inverse" the order horizontally (rename the vertices) and vertically (consider [[Dual Order|dual order]]) and get a "canonical" fence without changing number of antichains.

**Notation.** By $\mathbb{F}_n = (F_n, \leq_n)$ we would denote an n-element fence. By $\mathbb{C}_n = (C_n, \leq'_n)$ — n-element [[Crown|crown]].

**Statement 1.** For any natural $n \geq 2$ we have $\#A(\mathbb{F}_n) = \#A(\mathbb{F}_{n-1}) + \#A(\mathbb{F}_{n-2})$.
$\blacktriangle$ We directly use [[Number of Antichains through Subposets]] by fixing $\mathbb{P} := \mathbb{F}_n$ and $p := f_0$, where $f_0$ is an [[Fence|endpoint]] of $\mathbb{F}_n$.
We get $\#A(\mathbb{F}_n) = \#A_{\mathbb{F}_n}(F_{n} \setminus \{f_0\}) + \#A_{\mathbb{F}_n}(F_{n} \setminus \{f_0, f_1\}) = \#A(\mathbb{F}_{n-1}) + \#A(\mathbb{F}_{n-2})$. $\boxtimes$

**Corollary.** $\#A(\mathbb{F}_n)$ is the $(n + 2)$<sup>nd</sup> Fibonacci number.
$\blacktriangle$ $\#A(\mathbb{F}_0) = 1$ and $\#A(\mathbb{F}_1) = 2$ we get by brute force, this are 2<sup>nd</sup> and 3<sup>rd</sup> Fibonacci numbers respectively, then, by the statement 1, we get the desired.

**Statement 2.** $\#A(\mathbb{C}_n) = \#A(\mathbb{F}_{n-1}) + \#A(\mathbb{F}_{n-3})$.
$\blacktriangle$ Again we directly use [[Number of Antichains through Subposets]] by fixing $\mathbb{P} = \mathbb{C}_n$ and $p$ to be an arbitrary element of $C_n$. We get $\#A(\mathbb{C}_n) = \#A_{\mathbb{C}_n}(C_{n} \setminus \{p\}) + \#A_{\mathbb{C}_n}(F_{n} \setminus \mathord{\updownarrow} p) = [\mathord{\updownarrow} p \text{ is a 3-element fence}] = \#A(\mathbb{F}_{n-1}) + \#A(\mathbb{F}_{n-3})$. $\boxtimes$ 
**Source.** Exercise 2.25b-d from @schroderOrderedSetsIntroduction2016
