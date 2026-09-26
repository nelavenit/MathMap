---
tags:
  - Definition
---
**Definition.** Let $\mathbb{P} = (P, \leq)$ be a [[Partial Order|poset]], $f: P \rightarrow P$ be a self-map. Then $p \in P$ is called a <u>fixed point of f</u> if $f(p) = p$.

**Notation.** Let $\mathbb{P} = (P, \leq)$ be a poset and $f$ be a self-map on P. The set of all fixed points of $f$ is denoted by $\operatorname{Fix}_\mathbb{P}(f)$ or just $\operatorname{Fix}(f)$ if the order in consideration is obvious from the context.

**Definition.** If a self-map $f$ doesn't have any fixed points it is called <u>fixed-point-free</u>.

**Notation.** For brevity we would often write <u>FPF</u> instead of "fixed-point-free".

**Examples.**
1. Lets consider $\mathbb{N}$ with the natural ordering:
	1. $f \equiv c$ has a single fixed point of $c$
	2. $f = id$ has every $n \in \mathbb{N}$ as a fixed point
	3. $f: n \mapsto n+1$ is fixed-point-free

**Remark.** In some literature (e.g. @schroderOrderedSetsIntroduction2016) considering fixed points of $f$ already involve $f$ being an [[Order Endomorphism|order endomorphism]].