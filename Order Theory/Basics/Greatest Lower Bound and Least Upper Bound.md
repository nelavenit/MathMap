---
tags:
  - Definition
---
**Definition.** Let $\mathbb{P} = (P, \leq)$ be a [[Partial Order|poset]] and $Q \subseteq P$. We say that $l\in P$ is the <u>greatest lower bound</u> of $Q$ (<u>GLB</u> for short) if $g$ is a [[Lower and Upper Bounds|lower bound]] of $Q$ and there is no other lower bound of $Q$ greater than $g,$ in other words $g$ is the [[Least and Greatest Elements|greatest element]] in the [[Subposet|subposet]] of lower bounds of $Q$, i.e.
$$\begin{cases}
\forall q\in Q\ g \geq q \\
\forall g' \leq g\ \exists q\in Q \text{ s.t. } q \geq g'
\end{cases}$$
**Definition.** Same way $l \in P$ is called the <u>least upper bound</u> of $Q$ (<u>LUB</u> for short) if it's an [[Lower and Upper Bounds|upper bound]] and there is no other upper bound of $Q$ less than $l$.

**Notation.** The greatest lower bound of $Q$ is often called the <u>infimum</u> of $Q$ and is denoted by $\inf_\mathbb{P}(Q),$ or just $\inf(Q)$ if the order in consideration is obvious from the context.
**Notation.** The least upper bound of $Q$ is often called the <u>supremum</u> of $Q$ and is denoted by $\sup_\mathbb{P}(Q),$ or just $\sup(Q)$ if the order in consideration is obvious from the context.

**Statement.** Being the greatest lower bound and being the least upper bound are [[Dual Properties|dual properties]].
$\color{red}\text{Proof}$ is a trivial exercise.

**Remark.** Sometimes, especially in the older texts, <u>g.l.b.</u> is used instead of GLB, and <u>l.u.b.</u> instead of LUB.