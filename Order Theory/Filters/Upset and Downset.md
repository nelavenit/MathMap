---
tags:
  - Definition
---
**Definition.** Let $\mathbb{P} = (P, ≤)$ be a [[Partial Order|poset]], $U ⊆ P$ is called an <u>upper set</u> or an <u>upset</u> of $\mathbb{P}$ iff $∀ p,q ∈ P$ we have that $p ∈ U$ and $p ≤ q$ implies $q ∈ U$.
**Definition.** Analogously, $D$ is called a <u>lower set</u> or a <u>downset</u> of $\mathbb{P}$ iff $\forall p,q ∈ P$ we have that $p ∈ D$ and $q ≤ p$ implies $q ∈ D$.

**Notation.** If the poset whose downsets/upsets we are considering is obvious from the context we may omit the phrase "of $\mathbb{P}$".

**Notation.** Sometimes we would refer to a [[Subposet|subposet]] $(U,\leq|_{U\times U})$ as to an upset and the same with a downset.

**Notation.** Let $\mathbb{P} = (P, \leq)$ be a poset and $X \subseteq P$. Analogously to [[Principal Filter and Ideal|principal filters and ideals]] we define $\mathord{\uparrow} X := \bigcup\limits_{x\in X} \mathord{\uparrow} x$ and $\mathord{\downarrow} X := \bigcup\limits_{x\in X} \mathord{\downarrow} x$.
**Statement.** For any $X \subseteq P$ we have $\mathord{\uparrow} X$ is an upset and $\mathord{\downarrow} X$ is a downset.
$\color{red}\text{Proof}$ is a simple exercise.

**Remark.** Sometimes in literature the downset $\mathord{\downarrow} X$ is denoted by $L(X)$ and the upset $\mathord{\uparrow} X$ is denoted by $U(X)$.

**Statement.** Being an upset and being a downset are [[Dual Properties|dual properties]].
$\color{red}\text{Proof}$ is a trivial exercise.