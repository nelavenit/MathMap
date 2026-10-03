---
tags:
  - Definition
---
**Definition.** [[Partial Order|Poset]] $(Q, \leq')$ is called an <u>subposet</u>, <u>ordered subset</u> or <u>suborder</u> of an order $(P, \leq)$ if $Q \subseteq P$ and $\leq' = \leq|_{Q \times Q}.$

**Examples.** 
![[Subposet Example.png|400]]

**Notation.** When the corresponding relation is obvious from the context we may call the $Q$ itself the subposet.

**Remark.** This differs from the definition of the [[Subgraph|subgraph]] for the [[Graph|graph]] binary relation and is a direct analog of the [[Induced Subgraph|induced subgraph]]. This is because, if we allow for the removal of arbitrary [[Lower and Upper Covers, Adjacence|covers]] (i.e. edges in the [[Hasse Diagram|Hasse diagram]]), we may get a relation that is not a poset because of the [[Transitivity|transitivity]] violation. Unlike in the graph case, where there is no transitivity.