---
tags:
  - Statement
---
**Statement.** Let $\mathbb{W} = (W, \leq)$ be a [[Well-Founded Order|well-founded order]], $f: W \to W$ is a [[Strict Order Homomorphism|strict endomorphism]]: $x < y \to f(x) < f(y)$. Then $\forall w \in W$ $w \leq f(w)$.
$\blacktriangle$ By induction principle for well-founded sets it suffices to show $x \leq f(x)$ under assumption $\forall y < x$ $y \leq f(y)$. Assume the opposite: $f(x) < x$ then by condition on $f$ we have $f(f(x)) < f(x)$, but $f(x) < x$ so by assumption $f(x) \leq f(f(x))$ – contradiction. $\boxtimes$

**Intuition.** Alternatively we could prove by saying $x > f(x) > f(f(x)) > \ldots$ is an
infinite descending sequence.

**Statement.** The same wouldn't work in the case of arbitrary [[Partial Order|poset]]. For instance, consider $\mathbb{Z}$ with a natural ordering and [[Order Automorphism|automorphism]] $f:n \mapsto n - 1$, $f$ is a strict homomorphism, but $\forall z \in Z\ z > f(z).$