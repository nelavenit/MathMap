---
tags:
  - Definition
  - Order-Theory
---
**Intuition 1.** We want to combine all the [[Card|cards]] of a [[Poset|poset]] but with unlabeled vertices (i.e. to have no way of determining which element of $P \setminus \{p\}$ corresponds to which element of $P$). We would realize it by taking an [[Isomorphism Class|isomorphism classes]] of the cards.
**Intuition 2.** To avoid isomorphism classes being proper classes, we restrict ourselves to the subsets of natural numbers.

**Definition.** Let $\mathcal{C}$ be the set of all isomorphism classes of orders with an underlying set contained in $\mathbb{N}$. The <u>deck</u> of a poset $\mathbb{P}$ is the function $D_\mathbb{P} : \mathcal{C} \to \mathbb{N}$ s.t. for each $[C] \in \mathcal{C}$ we have that $D_\mathbb{P}([C])$ is the number of cards of $\mathbb{P}$ that are [[Order Isomorphism|isomorphic]] to the $C$.

**Examples.** 
1. ![[Cards Example 01.png|300]] ![[Deck Example 01.png|300]]
2. ![[Reconstruction Problem 3-Element Counterexample.png|450]]
3. ![[Reconstruction Problem 2-Element Counterexample.png|450]]
