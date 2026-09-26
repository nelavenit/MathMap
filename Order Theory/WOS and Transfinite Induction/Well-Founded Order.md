---
tags:
  - Definition
---
**Intuition.** Induction principle on natural numbers sounds like: 
Let $A(n)$ be a property of a natural number $n$ and let $A(n)$ be proven to be true under the assumption that $A(m)$ is true for all $m$ less than $n$. Then the property $A(n)$ is true for all natural $n$.
Formally $\forall n\ ( \forall m\ (m < n) \to A(m)) \to A(n)) \to \forall n\ A(n)$. This is one of the axioms of natural numbers if we consider Peano arithmetic, but it's just a statement about an order if we are working in $ZFC$.
A natural question is: for which orders analogous principle would work?

By the [[Well-Founded Order Criteria|criteria]] we get that well-founded posets are exactly the ones induction principle applies to.

**Definition.** [[Partial Order|Poset]] $\mathbb{P} = (P, \leq)$ is called <u>well-founded</u> if every non-empty [[Subposet|subposet]] of $\mathbb{P}$ has a [[Minimal and Maximal Elements|minimal element]].

**Examples.**
1. $\mathbb{N}$ with a natural ordering is well-founded
2. $\mathbb{Z},\mathbb{Q},\mathbb{R}, \mathbb{Q}_{[0,1]}, \mathbb{R}_{[0,1]}$ with natural orderings are not well-founded
3. Let $\mathbb{P}$ and $\mathbb{Q}$ be well-founded posets, then the [[Orders Sum|sum]] $\mathbb{P} + \mathbb{Q}$ is well-founded
4. Let $\mathbb{P}_1, \mathbb{P}_2, \ldots, \mathbb{P}_n$ be well-founded, then [[Lexicographic Order|lexicographic order]] $\mathbb{P}_1 \times \mathbb{P}_2 \times \ldots \times \mathbb{P}_n$ is well-founded
5. Every finite poset is well-founded
6. $(\mathbb{N}, |)$, where $|$ means "divides", is well-founded with $Min_{(\mathbb{N},|)}(A)$ = $\gcd(A)$
