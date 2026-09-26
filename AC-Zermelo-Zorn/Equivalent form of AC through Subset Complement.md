---
tags:
  - Statement
  - Set-Theory
---
**Intuition.** For some proofs it would be convenient to use an equivalent form of the [[Axiom of Choice|Axiom of Choice]].

**Definition (Equivalent form of Axiom of Choice).** Let $X$ be a set, then there is a function $f$ s.t. it maps each subset $A \subset X$, except $X$ itself to an element from $X\setminus A$:
$$\forall X\ (\exists f\ (\forall A \subset X\ (f(A) \in X \setminus A)))$$

**Statement.** This form is equivalent to the Axiom of Choice.
$\blacktriangle$ (AC $\Rightarrow$) Consider $X' = \text{powerset}(X) \setminus \{\emptyset, X\}$, let $f$ be a choice function for $X'$. Then $\overline{f} : \overline{f}(B) = f(X \setminus B)$ exists by Axiom Schema of Replacement and satisfies the equivalent condition.
(AC $\Leftarrow$) Consider $f$ be a choice function by the equivalent definition for the set $X$. 
1. Then let's consider $\overline{f}$: $\overline{f}(A) = f(X \setminus A)$, it exists by Axiom Schema of Replacement. 
2. Now let's restrict it to single-element subsets of $X$: $A \in \text{dom}(f') \Leftrightarrow \exists x \in X \text{ s.t. } A = \{x\}$ – $f'$ maps $\{A\}$ to an element of $A$ 
3. Lets make $f''$ by replacing every $\{A\}$ in $\text{dom}(f')$ with $A$, it exists by the Axiom Schema of Replacement, $f''$ is exactly the sought-for choice function. $\boxtimes$