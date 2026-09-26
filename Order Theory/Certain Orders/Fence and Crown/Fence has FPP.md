---
tags:
  - Finite
  - Statement
---
**Statement.** Every [[Fence|fence]] has a [[Fixed Point Property|fixed point property]].
$\blacktriangle$ (Pr.2.39. from @schroderOrderedSetsIntroduction2016)
Let $\mathbb{P} = \{p_{0}, p_{1}, p_{2}, \ldots, p_{n} \}$ be a fence. Suppose $f : P \to P$ is a [[Fixed Point and Fixed-Point-Free|fixed-point-free]] [[Order Endomorphism|endomorphism]]. For each $k \in \{0, \ldots, n \}$, let $g ( k )$ be the number $l$ such, that $f ( p_{k} )=p_{l}$. Then, for $\left|k_{1}-k_{2} \right| \leq1$, we have $| g ( k_{1} )-g ( k_{2} ) | \leq1$, because points in $\mathbb{P}$ are comparable iff their indices are adjacent. Moreover, if $| k-g ( k ) | \leq1$, then $p_{k} \sim f ( p_{k} )$ and $f$ can't be FPF by [[Finite Height FPF Endomorphism Criterion|this]]. Thus $| k-g ( k ) | \geq2$ for all $k$.
Let $m$ be the smallest number such that $g ( m ) \, \leq\, m$. Then $g ( m ) \leq m-2$ and $g(m - 1) \geq m + 1$  — a contradiction to $|g(m) - g(m - 1)| \leq 1$. Thus $\mathbb{P}$ cannot have any fixed-point-free endomorphism $f.$ $\boxtimes$
