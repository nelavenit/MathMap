---
tags:
  - Definition
---
**Definition.** Let $\mathbb{P} = (P, \leq)$ be a [[Partial Order|poset]]. An [[Antichain|antichain]] $A \subseteq P$ is called a <u>maximal antichain</u> if it can't be extended to a larger antichain, i.e. it is [[Minimal and Maximal Elements|maximal]] in the set of all antichains of $\mathbb{P}$ with respect to set inclusion, in other words, there is no $a \in P\setminus A$ s.t. $A \cup \{a\}$ is an antichain.

**Statement.** Let $\mathbb{P} = (P, \leq)$ be a poset and $A$ be an antichain in $\mathbb{P}$. Then $A$ is a maximal antichain iff every element of $P$ is comparable to some element of $A$.
$\color{red}\text{Proof}$ is a trivial exercise.
**Corollary.** Let $\mathbb{P} = (P, \leq)$ be a poset and $A$ be a maximal antichain. Then $P = \mathord{\uparrow}{A}\ \cup \mathord{\downarrow}{A}$.
$\color{red}\text{Proof}$ is a trivial exercise.

TODO Examples