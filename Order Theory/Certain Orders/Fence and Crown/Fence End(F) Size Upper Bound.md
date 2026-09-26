---
tags:
  - Statement
  - Finite
---
**Statement.** Let $n$ be a natural number and $\mathbb{F}_n = (F_n, \leq)$ be a [[Fence|fence]] of $n$ elements. Then the $End(\mathbb{F}_n) \leq n 3^{n-1}$.
$\blacktriangle$ Let $f_0$ be an [[Fence|endpoint]] of $\mathbb{F}_n$, we would build [[Order Endomorphism|endomorphism]] $\phi$ step by step:
1. First we define $\phi$ on $f_0$ — there are $n$ options
2. If $\phi(f_0) = f_k$, for $\phi$ to be a [[Order-preserving map (Order Homomorphism)|homomorphism]] the only options for $\phi(f_1)$ are $f_{k-1}, f_k$ and $f_{k+1}$
3. The same is on every other step, there are at most 3 options and there are $n-1$ steps, so the total amount of different endomorphisms is bounded by $n3^{n-1} \boxtimes$

**Intuition.** The bound is not exact because at some step we might have $k = 0$ or $k = n - 1$ and, hence, there would be only two options.