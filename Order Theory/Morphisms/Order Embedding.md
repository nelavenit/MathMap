---
tags:
  - Definition
---
**Definition.** Let $\mathbb{P} = (P, \leq_P)$ and $\mathbb{Q} = (Q, \leq_Q)$ be [[Partial Order|posets]], $f: P \rightarrow Q$ is called an <u>order embedding</u> if $\forall p_1, p_2 \in P$ we have $$p_1 < p_2 \iff f(p_1) < f(p_2)$$ 
**Statement.** Let $\mathbb{P} = (P, \leq_P)$ and $\mathbb{Q} = (Q, \leq_Q)$ be posets, $f: P \rightarrow Q$. The following three conditions are equivalent:
1. $f$ is an order embedding
2. $\forall p_1, p_2 \in P$ we have $p_1 \leq p_2 \iff f(p_1) \leq f(p_2)$
3. $f$ is an isomorphism between $\mathbb{P}$ and $(f[P], \leq_Q|_{f[P]\times f[P]})$
$\color{red}\text{Proof}$ is a not very hard of an exercise.

**Example.** 
1. Every order [[Order Isomorphism|order isomorphism]], including [[Order Automorphism|order automorphisms]]

**Statement.** Being an order embedding is [[Self-dual Properties|self-dual]], i.e. $f$ is an order embedding from $\mathbb{P}$ to $\mathbb{Q}$ iff $f$ is an order embedding from $\mathbb{P}^d$ to $\mathbb{Q}^d$.
$\color{red}\text{Proof}$ is a trivial exercise.

TODO Examples (some finite self-drawn and look into "Introduction into order theory")