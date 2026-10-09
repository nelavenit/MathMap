---
tags:
  - Definition
---
**Definition.** Let $\mathbb{P}=(P,\leq)$ be an [[Partial Order|order]], $m \in P$ is called <u>minimal</u> (<u>maximal</u>) element of $\mathbb{P}$ iff $\nexists p \in P$ s.t. $p < m$ ($p > m$). We denote the set of all minimal (maximal) elements of $\mathbb{P}$ as $\operatorname{Min}(\mathbb{P})$ ($\operatorname{Max}(\mathbb{P})$).
**Notation.** Let $Q \subseteq P$, if we want to address the set of all minimal (maximal) elements of [[Subposet|subposet]] $(Q,\leq|_{Q\times Q})$ we would write $\operatorname{Min}_\mathbb{P}(Q)$ ($\operatorname{Max}_\mathbb{P}(Q)$). Note: by this definition $\operatorname{Min}(\mathbb{P})=\operatorname{Min}_\mathbb{P}(P)$.
**Examples.** 
1. ![[Minimal and Maximal Elements Example.png|300]]
2. Every [[Least is Minimal|least element is minimal]] so the examples from [[Least and Greatest Elements]] are relevant here
3. ℤ with the natural ordering has no greatest, least, minimal or maximal elements

**Statement.** Being a maximal element and being a minimal element are [[Dual Properties|dual properties]]. I.e. if $m$ is a minimal (maximal) element of $\mathbb{P}$, then $m$ is maximal (minimal) element of $\mathbb{P}^d$.
$\color{red}\text{Proof}$ is a trivial exercise.

**Remark.** Let $\mathbb{P} = (P, \leq_P)$ and $X \subseteq P$, when the subposet in consideration is obvious from the context we would, for brevity, say "minimal element of $X$" instead of "minimal element of $(X, \leq|_{X \times X})$".