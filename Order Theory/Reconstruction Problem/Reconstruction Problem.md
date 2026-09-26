---
tags:
  - Open-Problem
---
**Intuition.** Can we always unambiguously deconstruct the [[Partial Order|order]], knowing the [[Deck|deck]], i.e. do non-[[Order Isomorphism|isomorphic]] orders always have different decks?
There are two non-isomorphic orders with the same decks:

| ![[Reconstruction Problem 2-Element Counterexample.png]] | ![[Reconstruction Problem 3-Element Counterexample.png\|700]] |
| -------------------------------------------------------- | ------------------------------------------------------------- |
These are the **only** examples known so far.

**Open problem (Reconstruction problem (finite case)).** Is it true that for any $\mathbb{P}, \mathbb{Q}$ – *finite* orders with at least four elements $D_\mathbb{P} = D_\mathbb{Q}$ implies $\mathbb{P}$ and $\mathbb{Q}$ are isomorphic?

**Approach to the problem 1.** We could try to prove [[Reconstructibility|reconstructibility]] for more and more special classes of orders until every poset must belong to at least one of such class.
For example now we know:
1. [[Poset with Least or Greatest Element is Reconstructible]]
2. [[Poset with Isolated Point is Reconstructible]]
3. [[Fence is Reconstructible]]
	1. [[N-Order is reconstructible]], which is the corollary, but instead is proved by a brute force
4. [[Crown is Reconstructible]]

**Approach to the problem 2.** We could reconstruct more and more parameters of an order until every poset is uniquely determined just by knowing a set of reconstructible parameters.
For example now we know:
1. [[Width is Reconstructible]]
2. [[Height is Reconstructible]]
3. [[Number of Comparabilities and Degree of Missing Element are Reconstructible]]
4. [[Kelly Lemma]]: number of subsets of any type is reconstructible 