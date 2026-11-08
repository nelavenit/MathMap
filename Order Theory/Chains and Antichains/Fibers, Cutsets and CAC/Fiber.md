---
tags:
  - Definition
  - Order-Theory
---
**Definition.** Let $\mathbb{P} = (P, \leq)$ be a [[Poset|poset]]. A set $F \subseteq P$ is called a <u>fiber of </u>$\mathbb{P}$ if it intersects every [[Antichain|maximal antichain of ]]$\mathbb{P}$.

**Definition.** Let $\mathbb{P} = (P, \leq)$ be a [[Poset|poset]]. A set $F \subseteq P$ is called a <u>weak fiber of </u>$\mathbb{P}$ if it intersects every [[Antichain|maximal antichain of ]]$\mathbb{P}$ of the size at least $2$.

**Intuition.** Fibers and weak fibers differ only in how they treat [[Splitting Element|splitting elements]]. They are similar object, just one or the other may be convenient in different context. For example fibers are more convenient when considering CAC orders and N-freeness, while weak fiber is more convenient while talking about  min fiber size. This difference is seen in the following statement.

**Statement.** Let $\mathbb{P} = (P, \leq)$ be a poset and $F \subseteq P$. Then $F$ is a fiber in $\mathbb{P}$ $\iff$ $F$ is a weak fiber in $\mathbb{P}$ and it contains all the splitting elements of $P$.
$\color{red}\text{Proof}$ is a simple exercise, knowing splitting element singleton is the only possible antichain of the size $1$.

**Remark.** In some sources "weak fiber" is called a nontrivial fiber. (here is reference to Duffus)
**Remark.** Words "fiber" and "fibre" are interchangable and are simply British and American versions of the same word.

TODO Verify Maximal antichain is in antichain note
TODO reference to the paper with "nontrivial fiber"
TODO reference to both CAC/N-freeness and min fiber size investigation