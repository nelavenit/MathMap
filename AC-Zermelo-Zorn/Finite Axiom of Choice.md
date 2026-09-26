---
tags:
  - Statement
  - Set-Theory
---
**Statement (The finite version of [[Axiom of Choice|AC]]).** let $X$ be a finite set of nonempty sets (note that elements of $X$ may be infinite), then the choice function for $X$ exists, i.e. $\exists f$ s.t. $dom(f) = X$ and $\forall x \in X$ we have $f(x) \in x$.
$\color{red}\text{Proof idea}$ (in ZF) (in case of axiom limitation the only way I see not to be wrong is to code a formal proof, so I consider this an idea rather than a full proof):
Induction on the size of X: 
1. assume $|X|=n$ and we have the statement for $k<n$ 
2. $|X| = n \neq 0 \Rightarrow \exists x∈X ⇒ |X \setminus \{x\}| = n - 1 \Rightarrow \exists f$ – choice function for $X \setminus \{x\}$
3. $n≠0 ⇒ ∃y∈x ⇒ f∪\{(x,y)\}$ – choice function for $X\ \boxtimes$  

**Intuition.** It's an obvious desire to do the same using transfinite induction on an arbitrary $X$, but [[Well-Ordered Set|well-ordering]] arbitrary $X$ or even getting any well-ordered set of cardinality at least $|X|$ is exactly what requires an AC.

**Remark.** Sometimes finite Axiom of Choice is referred to as <u>Axiom of Choice for finite families</u> and is denoted as <u>AC<sub>fin</sub></u>.