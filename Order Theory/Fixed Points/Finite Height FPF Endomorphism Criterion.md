---
tags:
  - Statement
---
**Statement.** Let $\mathbb{P} = (P, \leq)$ be a [[Partial Order|poset]] of the *finite* [[Height|height]], $f: P \rightarrow P$ be an [[Order Endomorphism|endomorphism]]. Then $f$ has a [[Fixed Point and Fixed-Point-Free|fixed point]] $\iff$ $\exists p \in P$ s.t. $p \sim f(p)$.
$\blacktriangle$ $\boldsymbol{(\Longrightarrow)}$ Fixed point is the sought-for $p$
$\boldsymbol{(\Longleftarrow)}$ Assume toward a contradiction that $f$ is [[Fixed Point and Fixed-Point-Free|fixed-point-free]]. Then $p = f(p)$ is impossible, so it's either $p < f(p)$ or $p > f(p)$.
Consider $p < f(p)$. Then apply $f$ to the both sides: we get $f(f(p)) \geq f(p)$, but there can't be $f(f(p)) = f(p)$, because then $f(p) \in \operatorname{Fix}(f)$. So we get $f(f(p)) > f(p) > p$, this way we continue and get a [[Linear Order and Chain|chain]] of elements of $\mathbb{P}$: $f^k(p) > f^{k-1}(p) > \ldots > f(p) > p$ of arbitrary size, so we get a contradiction to the height of $\mathbb{P}$ being finite.
In the case of $p > f(p)$ the same way we would get a chain $f^k(p) < f^{k-1}(p) < \ldots < f(p) < p$. $\boxtimes$

**Corollary 1.** Endomorphism $f$ is fixed-point-free $\iff$ $\forall p \in P$ we have $p \nsim f(p)$. 
$\blacktriangle$ It's just a paraphrase or the statement using contrapositions. 

**Example.** 
![[Order with FPP Example 02.png|200]]
Assume $F$ is fixed-point-free endomorphism, hence $F(b) \nsim b$, hence $F(b) \in \{a,c\}$.

**Corollary 2.** If a poset $\mathbb{P}$ of the *finite* height has an element comparable to all other elements, then $\mathbb{P}$ has a [[Fixed Point Property|fixed point property]].
$\color{red}\text{Proof}$ is a simple exercise.

**Corollary 2.1.** If poset $\mathbb{P}$ is of the *finite* height has the [[Least and Greatest Elements|least element]] or the [[Least and Greatest Elements|greatest element]], then $\mathbb{P}$ has a [[Fixed Point Property|fixed point property]].
$\color{red}\text{Proof}$ is a trivial exercise.

**Corollary 2.2.** If $\mathbb{P}$ is a *finite* [[Linear Order and Chain|linear order]], then $\mathbb{P}$ has a [[Fixed Point Property|fixed point property]].
$\color{red}\text{Proof}$ is a trivial exercise.

**Corollary 3.** If poset $\mathbb{P} = (P, \leq)$ is *finite*, then endomorphism $f: P \rightarrow P$  a [[Fixed Point and Fixed-Point-Free|fixed point]] $\iff$ $\exists p \in P$ s.t. $p \sim f(p)$.
$\blacktriangle$ Finite poset has finite height, hence the statement is applicable. $\boxtimes$

**Intuition.** This statement fails if the height is *infinite*. For example, consider $\mathbb{Z}$ with a natural ordering and $f: z \mapsto z+1$.


**Sources.** My generalization of exercise 1-17 from @schroderOrderedSetsIntroduction2016.