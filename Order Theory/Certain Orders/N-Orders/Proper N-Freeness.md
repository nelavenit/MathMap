---
tags:
  - Definition
---
**Definition.** Let $\mathbb{P} = (P, \leq)$ be a [[Partial Order|poset]]. [[Subposet]] of four elements $a,b,c,d \in P$  is called a <u>proper N-suborder</u> if 
$$\begin{cases}
a < b > c < d \\
a \nsim c \\
b \nsim d \\
\nexists x \in P \text{ s.t. } b > x > c \land x\nsim a \land x\nsim d 
\end{cases}$$

**Examples.** 
1. ![[Proper N-Order Example 01.png|150]] – proper N-order
2. ![[Non Proper N-Order Example 01.png|150]] – [[N-Order|N-order]], but not a proper N-order

**Definition.** A poset $\mathbb{P} = (P, \leq)$ is called <u>proper N-free</u> if it contains no proper N-suborder. 

**Examples.** 
1. ![[Proper N-Free Order Example 01.png|150]] – proper N-free, but not [[N-Freeness|N-free]]
2. ![[Not Proper N-Free Order Example 01.png|150]] – not proper N-free

**Statement.** A proper N-suborder is an N-order, hence N-freeness implies proper N-freeness.
$\color{red}\text{Proof}$ is a trivial exercise.
