---
tags:
  - Definition
---
**Definition.** A [[Poset|poset]] $\mathbb{P} = (P, ≤)$ is called a <u>linear order</u> or a <u>chain</u> if all the elements of $\mathbb{P}$ are $\leq$-comparable, i.e. $\forall p_1, p_2 \in P$ $\left[ \begin{array}{ll} \ p_1 \leq p_2 \\\ p_2 \leq p_1 \end{array} \right .$. Relation $\leq$ is called a <u>linear ordering</u>.

**Definition.** Let $\mathbb{P} = (P, \leq)$ be a poset and $C \subseteq P$. If [[Induced Subposet|induced subposet]] $\mathbb{P}|_C$ is a linear order, we call $C$ a <u>chain in </u>$\mathbb{P}$.

**Examples.** 
1. ![[Linear Order Example 01.png|250]]
2. $\mathbb{N}, \mathbb{Z}, \mathbb{Q}, \mathbb{R}$ with natural orderings
3. Let $\mathbb{L}_1, \mathbb{L}_2, \ldots, \mathbb{L}_n$ be linear orders, then [[Lexicographic Order|lexicographic order]] $\mathbb{L}_1 \times \mathbb{L}_2 \times \ldots \times \mathbb{L}_n$ is linear too.  (Intuition: alphabetic ordering on letters is linear, hence lexicographic ordering on words in the dictionary is also linear)
4. Let $\mathbb{P} = (P, \leq)$ be a poset and $f$ be an [[Order Endomorphism|endomorphism]] of $\mathbb{P}$. Then for each $p \in P$ s.t. $p \leq f(p)$ the set $\{f^n(p) \mid n \in \mathbb{N}\}$ is a chain in $\mathbb{P}$.  
   $\blacktriangle$ 
	1. By induction on $n$ show that $\forall n \in \mathbb{N}$ $p \leq f^n(p)$. Step: $p \leq f^k(p) \Rightarrow f(p) \leq f^{k+1}(p)$, but we also have $p \leq f(p) \Rightarrow p \leq f^{n+1}(p)$  
	2. Let $n, m \in \mathbb{N}$ and $n > m$, we know $p \leq f^{n-m}(p) \Rightarrow f^m(p) \leq f^m \circ f^{n-m}(p) = f^n(p)$  

**Examples.**
1. ![[Chain Example 01.png|250]]
2. Any set of natural numbers is a chain in $\mathbb{N}$
3. All the natural numbers form a chain in $\mathbb{Z}$
4. All the rational numbers form a chain in $\mathbb{R}$

**Remark.** Another commonly used names for a linear order are <u>total order</u>, <u>linearly ordered set</u> and <u>totally ordered set</u>.

**Remark.** A chain in $\mathbb{P}$ is a subset of $P$, not a subposet of $\mathbb{P}$, similarly to the "[[Complete Graph (Clique)|clique]] of $\mathbb{G}$" in [[Graph|graph]] theory.

**Statement.** Being a linear order is [[Self-dual Properties|self-dual]].
$\color{red}\text{Proof}$ is a simple exercise.

**Statement.** Subset being a chain is [[Self-dual Properties|self-dual]].
$\color{red}\text{Proof}$ is a simple exercise.
