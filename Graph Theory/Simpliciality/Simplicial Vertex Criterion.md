---
tags:
  - Statement
  - Graph-Theory
---
**Statement (Finite case).** Let $\mathbb{G} = (G, E)$ be a finite [[Graph|graph]], $v \in G$, then the following are equivalent:
1. $v$ is a [[Simplicial Vertices and Cliques|simplicial vertex]], i.e. $N[v]$ is a [[Complete Graph (Clique)|clique]]
2. $N[v]$ is a maximal clique of $\mathbb{G}$
3. The [[Neighborhood of Vertex|open neighborhood]] $N(v)$ is a clique of $\mathbb{G}$
4. $v$ is not the middle vertex of any three-vertex [[Path and Induced Path|induced path]] of $\mathbb{G}$. 
5. $v$ belongs to exactly one maximal clique of $\mathbb{G}$
$\blacktriangle$ **(1 $\boldsymbol{\Rightarrow}$ 2)** Assume the opposite: there is a clique $C$ of $\mathbb{G}$ s.t. $N[v] \subsetneq C$, which includes $v \in C$. Then there is a vertex $u \in C \setminus N[v]$. By definition of a neighborhood, we have $(u,v) \not\in E$ – contradicts $C$ being a clique of $\mathbb{G}$.
**(2 $\boldsymbol{\Rightarrow}$ 1)** Obvious.
**(1 $\boldsymbol{\Leftrightarrow}$ 3)** Trivial.
**(3 $\boldsymbol{\Leftrightarrow}$ 4)** A vertex $v$ is the middle vertex of a three-vertex induced path precisely when there exist distinct $x,y \in N(v)$ s.t. $(x,y) \not\in E$. Hence, no such path exists exactly when $N(v)$ is a clique.  
**(2 $\boldsymbol{\Rightarrow}$ 5)** Assume there is another $C \subseteq G$ – maximal clique of $\mathbb{G}$ with $v \in C$. Then $C \subseteq N[v]$, else it's not a clique, because $v$ wouldn't be adjacent to some vertex of $C$, then either $C = N[v]$ or $C$ is not maximal.
**(5 $\boldsymbol{\Rightarrow}$ 1)** Assume the opposite, i.e. $N[v]$ is not a clique. This means there are two distinct $x,y \in N[v]$ s.t. $(x,y) \not\in E$. Then consider any maximal clique of $\mathbb{G}$ containing $\{x, v\}$ and any maximal clique of $\mathbb{G}$ containing $\{ v, y \}$. They would exist due to finiteness of $\mathbb{G}$ and they can't be equal due to $(x,y) \not\in E$ – contradicts $v$ belonging to exactly one maximal clique of $\mathbb{G}$. $\boxtimes$

**Remark.** Existence of maximal cliques in **(5 $\boldsymbol{\Rightarrow}$ 1)** is the only step of the proof not justified in ZF for arbitrary infinite graphs.

**Statement (General case in ZF).** Let $\mathbb{G} = (G, E)$ be a [[Graph|graph]], $v \in G$, then the following are equivalent:
1. $v$ is a [[Simplicial Vertices and Cliques|simplicial vertex]], i.e. $N[v]$ is a [[Complete Graph (Clique)|clique]]
2. $N[v]$ is a maximal clique of $\mathbb{G}$
3. The [[Neighborhood of Vertex|open neighborhood]] $N(v)$ is a clique of $\mathbb{G}$
4. $v$ is not the middle vertex of any three-vertex [[Path and Induced Path|induced path]] of $\mathbb{G}$. 
$\color{red}\text{Proof}$ is exactly the same as in finite case, just the **(2 $\boldsymbol{\Rightarrow}$ 5)** and **(5 $\boldsymbol{\Rightarrow}$ 1)** removed.

**Statement (General case in ZFC).** Let $\mathbb{G} = (G, E)$ be a [[Graph|graph]], $v \in G$, then the following are equivalent:
1. $v$ is a [[Simplicial Vertices and Cliques|simplicial vertex]], i.e. $N[v]$ is a [[Complete Graph (Clique)|clique]]
2. $N[v]$ is a maximal clique of $\mathbb{G}$
3. The [[Neighborhood of Vertex|open neighborhood]] $N(v)$ is a clique of $\mathbb{G}$
4. $v$ is not the middle vertex of any three-vertex [[Path and Induced Path|induced path]] of $\mathbb{G}$. 
5. $v$ belongs to exactly one maximal clique of $\mathbb{G}$
$\color{red}\text{Proof}$ is the same as in finite case, just in the **(5 $\boldsymbol{\Rightarrow}$ 1)** the maximal cliques exist by the [[Maximal Clique Existance|principle]] that every clique is contained in a maximal clique, which is equivalent to AC over ZF.

Note: **(1 $\boldsymbol{\Rightarrow}$ 5)** works for an arbitrary graph $\mathbb{G}$ in ZF.
**Statement.** Let $\mathbb{G} = (G, E)$ be a graph. Then every simplicial vertex of $\mathbb{G}$ belongs to exactly one maximal clique.
$\blacktriangle$ The implications **(1 $\boldsymbol{\Rightarrow}$ 2)** and **(2 $\boldsymbol{\Rightarrow}$ 5)** from the finite-case proof apply without any finiteness assumption. $\boxtimes$