---
tags:
  - Statement
---
**Statement.** Let $\mathbb{P} = (P, \leq)$ be a [[Partial Order|poset]] with an [[Fixed Point Property|FPP]], then $\mathbb{P}$ is [[Connectivity|connected]]. 
$\blacktriangle$ Assume the opposite: $\mathbb{P}$ is disconnected, so there is a pair $p,q \in P$, s.t. there is no [[Fence|fence]] in $\mathbb{P}$ with them as [[Fence|endpoints]]. 
Intuition is "let's map $p$'s [[Connected component|connected component]] to the $q$, and map the rest to the $p$".
Define 
$$ f(r) = 
\cases{
q, \text{there is a fence with p and r as endpoints} \\
p, \text{else}
}$$
Constructed $f$ is an [[Fixed Point and Fixed-Point-Free|FPF]] [[Order Endomorphism|endomorphism]]:
1. Assume it's not an endomorphism, hence there is a relation $a \geq b$ s.t. $f(a) \neq f(b)$, hence, WLOG, $f(a) = q, f(b) = p$. So, by definition of $f$, there is a fence with $a$ and $p$ as endpoints. Combine it with $a \geq b$ and get a fence with $p$ and $b$ as endpoints — contradicts $f(b) = p$.
2. Proving fixed-point-freeness is trivial.  
Contradiction to $\mathbb{P}$ having FPP $\implies$ $\mathbb{P}$ is connected. $\boxtimes$