---
tags:
  - Definition
---
**Definition.** Let $\mathbb{P} = (P, \leq_P)$ and $\mathbb{Q} = (Q, \leq_Q)$ be [[Partial Order|posets]], $\Phi: P \to Q$ is called an <u>order isomorphism of</u> $\mathbb{P}$ <u>and</u> $\mathbb{Q}$ if: 
1. $\Phi$ is order-preserving
2. $\Phi$ has an inverse $\Phi^{-1}$
3. $\Phi^{-1}$ is order preserving

Alternatively (proof of equivalence is a trivial exercise), $\Phi$ is an order isomorphism if: 
1. $\Phi$ is a bijection
2. $\forall p_1, p_2 \in P \quad p_1 \leq p_2 \Leftrightarrow \Phi(p_1) \leq \Phi(p_2)$

**Examples.**
1. ![[Order Isomorphism Example.png|300]]
2. ![[Bijective Non-Isomorphic Homomorphism Example.png|300]]

**Notation.** If there is an isomorphism between $\mathbb{P}$ and $\mathbb{Q}$ we would say $\mathbb{P}$ and $\mathbb{Q}$ are <u>isomorphic</u> and denote it as $\mathbb{P} \cong \mathbb{Q}$.

**Statement.** Being an order isomorphism is [[Self-dual Properties|self-dual]]:
$f: P \to Q$ is an isomorphism of $\mathbb{P}$ and $\mathbb{Q}$ $\Longleftrightarrow$ $f$ is an isomorphism of $\mathbb{P}^d$ and $\mathbb{Q}^d$.
$\color{red}\text{Proof}$ is a simple exercise.