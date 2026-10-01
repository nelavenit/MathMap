---
tags:
  - Statement
---
**Statement 1.** Let $A$ be a set with $|A| = n$, then there are exactly $2^n$ binary relations on $A$ that are both [[Symmetry|symmetric]] and [[Antisymmetry|antisymmetric]].
$\blacktriangle$ Let $a_1, a_2 \in A$ and $\circ$ be a symmetric antisymmetric binary relation on $A$. If $a_1 \neq a_2$, then:
1. If $a_1 \circ a_2$ and $a_2 \circ a_1$, then $\circ$ is not antisymmetric
2. Else if $a_1 \circ a_2$ and $a_2 \centernot\circ a_1$, then $\circ$ is not symmetric
Hence, only for $a_1 = a_2$ may we have $a_1 \circ a_2$. Hence number of such relations is $\leq 2^n$ (all the ways to choose the subset of $A$).
Now consider any subset $S \subseteq A$ and define $\circ$ as $a \circ a \iff a \in S$. It is both symmetric and antisymmetric, hence we got $2^n$ different such relations. $\boxtimes$

**Statement 2.** Exactly one of this relations is [[Reflexivity|reflexive]], it is $=$. Exactly one of this relation is [[Irreflexivity|irreflexive]] and it is $\emptyset$.
$\color{red}\text{Proof}$ is a simple exercise.