---
tags:
  - Definition
  - Order-Theory
---
**Definitions.** Let $\mathbb{P} = (P, \leq)$ be a [[Poset|poset]]. An element $p \in P$ is called a <u>splitting element of </u>$\mathbb{P}$ if it is comparable to every other element. I.e. for any $q \in  P$ we have either $p \leq q$ or $p \geq q$. 

**Examples.** All the splitting elements in the following [[Hasse Diagram|Hasse diagrams]] are colored orange
1. ![[Pasted image 20261106205932.png|28]] – every element of a [[Linear Order (Chain)|linear order]] is splitting
2. ![[Pasted image 20261106210048.png|137]]
3. ![[Pasted image 20261106210117.png|139]]
4. Every [[Least and Greatest Elements|least and greatest]] element is splitting

**Statement.** Let $\mathbb{P} = (P, \leq)$ be a poset. Then $p \in P$ is splitting in $\mathbb{P}$ $\iff$ $\{p\}$ is a cutset of $\mathbb{P}$.
$\color{red}\text{Proof}$ is a simple exercise. Hint: every maximal chain contains every splitting element.

TODO reference to cutset