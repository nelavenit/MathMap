---
tags:
  - Definition
  - Order-Theory
---
**Definition.** Let $\mathbb{P} = (P, \leq)$ be a poset and $Q \subseteq P$, then $(Q, \leq|_{Q \times Q}) := (Q, \leq \cap\ Q \times Q)$ is called a <u>subposet of </u>$\mathbb{P}$<u> induced by </u>$Q$ and is denoted by $\mathbb{P}|_{Q}$. Any induced subposet is also called simply <u>subposet of </u>$\mathbb{P}$. 

**Examples.** 
![[Subposet Example.png|400]]


**Notation.** When the corresponding relation is obvious from the context we may call the $Q$ itself the subposet.

**Remark.** In some sources $\mathbb{P}|_Q$ is denoted by $\mathbb{P}[Q]$.

**Remark.** In some sources subposet is called an <u>ordered subset</u> or a <u>suborder</u>.

**Remark.** This differs from the definition of the [[Subgraph|subgraph]] for the [[Graph|graph]] binary relation and is a direct analog of the [[Induced Subgraph|induced subgraph]]. This is because, if we allow for the removal of arbitrary [[Lower and Upper Covers, Adjacence|covers]] (i.e. edges in the [[Hasse Diagram|Hasse diagram]]), we may get a relation that is not a poset because of the [[Transitivity|transitivity]] violation. Unlike in the graph case, where there is no transitivity.