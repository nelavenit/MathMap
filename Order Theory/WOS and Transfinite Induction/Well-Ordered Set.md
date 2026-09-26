---
tags:
  - Definition
---
**Intuition.** One of the natural questions that arises when investigating into [[Well-Founded Order|well-founded]] [[Partial Order|orders]] is what if they would work more like natural numbers, natural ordering on $\mathbb{N}$ is [[Linear Order and Chain|linear]]. 
It appeared that being being both well-founded and linearly ordered is an extremely strong restriction, so strong that all such sets can be ordered into a hierarchy, and their certain quotient class can even be ordered into a linear hierarchy, which would allow us to use their equivalence classes by isomorphism with the $\in$ relation to perform a transfinite induction on arbitrary sets.

**Definition.** Poset $\mathbb{W} = (W, \leq)$ is called <u>well-ordered</u> if it is  
1. Well-founded order 
2. Linear order
We will call a well-ordered poset a <u>woset</u> or a <u>WOS</u>, rarer a <u>well-ordered set</u>.

**Examples.**
1. $\mathbb{N}$ with a natural ordering is well-ordered
2. $(\mathbb{N},|)$, where $|$ means divides is well-founded, but not well-ordered
3. Any finite linear order is well-ordered
4. The [[Orders Sum|sum]] $\mathbb{N} + \infty$ is well-ordered ($\infty$ means a single-element poset $(\{\infty\},=)$)
5. Let $\mathbb{W}$ and $\mathbb{V}$ be well-ordered, then $\mathbb{W} + \mathbb{V}$ is well-ordered too

**Intuition.** Sough-for hierarchy will be represented by a theorem "for every well-ordered sets $\mathbb{W}$,$\mathbb{V}$ either $\mathbb{W}$ is isomorphic to some [[Upset and Downset|downset]] of $\mathbb{V}$, or vice versa", but to prove this we need to get some results on infinite induction and infinite recursion and some insight into woset's structure 
([[Form of Arbitrary Element of Woset]], [[Form of Arbitrary Downset of Woset]], [[Woset is Isomorphic to own Downsets Order]]).

TODO link to infinite induction and recursion