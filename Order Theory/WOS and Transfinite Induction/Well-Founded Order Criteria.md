---
tags:
  - Statement
---
**Statement.** (Theorem 15 from @vereshchaginNachalaTeoriiMnozhestv2012) Let $\mathbb{P} = (P, \leq)$ be a [[Partial Order|poset]]. Then the following properties are equivalent:
1. $\mathbb{P}$ is [[Well-Founded Order|well-founded]], i.e. any non-empty [[Subposet|subposet]] of $\mathbb{P}$ has a [[Minimal and Maximal Elements|minimal element]]

2. There is no infinite strictly decreasing sequence $p_0 > p_1 > p_2 > \ldots$ of elements of $\mathbb{P}$

3. For $\mathbb{P}$ induction principle is true in the following form: if for all $x \in P$ we have $A(x)$ true under assumption $A(y)$ is true for all $y < x$, then $A(x)$ is true for all $x \in P$ (i.e. $\forall n \, (\forall y \, ((y < x) \rightarrow A(y)) \rightarrow A(n)) \rightarrow \forall n \, A(n)$).
$\blacktriangle$ 
**(1) $\boldsymbol{\Rightarrow}$ (2)** Assume the opposite, i.e. $\exists p_0 > p_1 > \ldots$ then $\bigcup_{i=1}^∞ n_i \subseteq P$ and has no minimal element - contradiction
**(2) $\boldsymbol{\Rightarrow}$ (1)** Let $X \subseteq P$. Assume $X$ has no minimal element, then let's fix arbitrarily $x_0 \in X$. $x_0$ is not a minimal element in $X$ by assumption $\Rightarrow$ $\exists x_1 \in X$ s.t. $x_1 < x_0$, and so on we get an infinite strictly decreasing sequence $x_0 > x_1 > x_2 > \ldots$ - contradicts (2)
**(1) $\boldsymbol{\Rightarrow}$ (3)** Assume the opposite: $\exists A(\cdot)$ s.t. $\forall x (\forall y ((y<x)\to A(y))\to A(x))$ but $\not\forall x\ A(x)$.
Consider $F := \{ x\in X \mid A(x) \text{ is false} \}$. $F\subseteq X$ and $F \neq \emptyset \Rightarrow \exists m \in \text{Min}(F)$.
$m$ is minimal in $F$ $\Rightarrow \forall x < m\ A(x) \Rightarrow$ by assumption $A(m)$ is also true – contradicts $m\in F$.
(The main idea here is that we can consider $F$ and it has a minimal element)
**(3) $\boldsymbol{\Rightarrow}$ (1)** Assume the opposite: Let $X \subseteq P$ be a non-empty set with no minimal element. Let’s prove that $X = \emptyset$. Consider $A(x) := x \notin X$. Let’s prove $A$ satisfies the antecedent: if $\forall y < x\ A(y),$ then if $A(x)$ is false this means $x \in X \Rightarrow$ then $x \in \text{Min}_{\mathbb{P}}(X)$ – contradicts the choice of $X \Rightarrow A(n)$ is true $\Rightarrow$ by (3) we have $\forall x\ A(x) \Rightarrow X = \emptyset$ – contradicts the choice of $X$.
(The main trick here is that "not being an element of a certain set with no minimal elements" is a property of elements). $\boxtimes$