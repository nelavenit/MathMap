---
tags:
  - Statement
---
**Statement.** Let $\mathbb{P} = (P, \leq)$ be a [[Partial Order|poset]]. If $\mathbb{P}$ has a [[Fixed Point Property|FPP]], it is not [[Fixed-Point-Free Automorphic Order|FPF automorphic]].
$\color{red}\text{Proof}$ is a trivial exercise.

**Intuition.** The inverse is not right. Order $\mathbb{P}$ might have no [[Fixed Point and Fixed-Point-Free|FPF]] [[Order Automorphism|automorphisms]], but have some FPF [[Order Endomorphism|endomorphisms]]. For example (Pr.1.25. from @schroderOrderedSetsIntroduction2016), consider:
![[Order without FPP Example 01.png|200]]
The FPF endomorphism is shown by blue arrow, so it doesn't have a FPP.
At the same time it's not FPF automorphic: this order has exactly one element with exactly one [[Lower and Upper Covers, Adjacence|upper cover]]. So this element must be fixed under any automorphism.