---
tags:
  - Definition
---
**Definition.** A [[Partial Order|poset]] $\mathbb{P} = (P, ≤)$ is called a <u>linear order</u> or a <u>chain</u> if all the elements of $\mathbb{P}$ are $\leq$-comparable, i.e. $\forall p_1, p_2 \in P$ $\left[ \begin{array}{ll} \ p_1 \leq p_2 \\\ p_2 \leq p_1 \end{array} \right .$. Relation $\leq$ is called a <u>linear ordering</u>.

**Examples.** 
1. ![[Linear Order Example 01.png|250]]
2. $\mathbb{N}, \mathbb{Z}, \mathbb{Q}, \mathbb{R}$ with natural orderings
3. Let $\mathbb{L}_1, \mathbb{L}_2, \ldots, \mathbb{L}_n$ be linear orders, then [[Lexicographic Order|lexicographic order]] $\mathbb{L}_1 \times \mathbb{L}_2 \times \ldots \times \mathbb{L}_n$ is linear too.  (Intuition: alphabetic ordering on letters is linear, hence lexicographic ordering on words in the dictionary is also linear)
4. Let $\mathbb{P} = (P, \leq)$ be a poset and $f$ be an [[Order Endomorphism|endomorphism]] of $\mathbb{P}$. Then for each $p \in P$ s.t. $p \leq f(p)$ the set $\{f^n(p) \mid n \in \mathbb{N}\}$ is a chain in $\mathbb{P}$.  
   $\blacktriangle$ 
	1. By induction on $n$ show that $\forall n \in \mathbb{N}$ $p \leq f^n(p)$. Step: $p \leq f^k(p) \Rightarrow f(p) \leq f^{k+1}(p)$, but we also have $p \leq f(p) \Rightarrow p \leq f^{n+1}(p)$  
	2. Let $n, m \in \mathbb{N}$ and $n > m$, we know $p \leq f^{n-m}(p) \Rightarrow f^m(p) \leq f^m \circ f^{n-m}(p) = f^n(p)$  

**Notation.** If we consider a linearly ordered [[Subposet|subposet]] $(C, \leq|_{C\times C})$ of poset $\mathbb{P}$, we would also call the set $C$ a <u>chain</u>. So both "$C$ is a chain in $\mathbb{P}$" and "$(C, \leq|_{C\times C})$ is a chain in $\mathbb{P}$" would be correct things to say.

**Examples.**
1. ![[Chain Example 01.png|250]]
2. Any subset of $\mathbb{N}$ with a natural ordering is a chain

**Remark.** Another commonly used names for a linear order are <u>total order</u>, <u>linearly ordered set</u> and <u>totally ordered set</u>.

**Statement.** Being a linear order is [[Self-dual Properties|self-dual]].
$\color{red}\text{Proof}$ is a simple exercise.

**Statement.** Subset being a chain is [[Self-dual Properties|self-dual]].
$\color{red}\text{Proof}$ is a simple exercise.
