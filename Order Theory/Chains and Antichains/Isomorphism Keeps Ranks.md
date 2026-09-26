---
tags:
  - Statement
---
**Statement.** Let $\mathbb{P}=(P,\leq_{P})$ and $\mathbb{Q}=(Q,\leq_{Q})$ be *finite* [[Partial Order|posets]] and $\Phi : P \to Q$ be an [[Order Isomorphism|isomorphism]] of $\mathbb{P}$ and $\mathbb{Q}$. Then for all $p \in P$ we have $\text{rank}_{\mathbb{P}}(p) = \text{rank}_{\mathbb{Q}}(\Phi(p))$, i.e. element rank is an invariant.
$\blacktriangle$ 
1. Image of a [[Linear Order and Chain|chain]] under an [[Order-preserving map (Order Homomorphism)|order-preserving map]] is again a chain, thus, because $\Phi$ is injective, the image of a $k$-element chain under $\Phi$ is again a $k$-element chain.
   By [[Rank|alternative rank definition]] $rank(\rho) = k$ means there is a $k$-element chain with $p$ as a [[Least and Greatest Elements|greatest element]] $\implies$ its image is a $k$-element chain in $\mathbb{Q}$ with $\Phi(p)$ as a greatest element $\implies$ $rank(\Phi(p)) \geq rank(p)$. 
2. Let's do the same with $\Phi(p)$ by applying $\Phi^{-1}$: $rank(\Phi(p)) \leq rank(\Phi^{-1}(\Phi(p))) = rank(\rho)$. $\boxtimes$
