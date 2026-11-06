---
tags:
  - Graph-Theory
  - Definition
---
**Definition.** Let $\mathbb{C} = (C, E)$ be a [[Graph|graph]] with $k \geq 3$ being a size of $C$. Then $\mathbb{C}$ is called a <u>cycle of the length </u>$k$, or a $k$<u>-cycle</u>, if the vertices can be enumerated as $v_0, v_1, \ldots, v_{k-1}$ s.t. $E = \{(v_i, v_j)\ |\ |i - j| \in \{1, k-1\} \}$. A $k$-cycle on any vertex set is denoted $\mathbb{C}_k$.
**Definition.** Let $\mathbb{G} = (G, \leq)$ be a graph, a [[Subgraph|subgraph]] $\mathbb{C}$ of $\mathbb{G}$ is called a $k$<u>-cycle in </u>$\mathbb{G}$ if it is isomorphic to $\mathbb{C}_k$.

**Definition.** Let $\mathbb{C} = (C, E_C)$ be a cycle in $\mathbb{G}$, an edge $e \in E$ is called a <u>chord</u> of $\mathbb{C}$ if it connects elements of $C$ while not lying in $E_C$. I.e. it is an additional edge between vertices of a cycle.

**Definition.** The cycle in $\mathbb{G}$ is called <u>induced</u> if it is an [[Induced Subgraph|induced subgraph of ]]$\mathbb{G}$, equivalently there are no chords of $\mathbb{C}$ in $\mathbb{G}$.

**Definition.** A 3-cycle is called a <u>triangle</u>.
**Statement.** Every triangle of a graph is an induced one.

**Examples.** 
1. ![[3-Cycle Example.png|130]] – 3-cycle
2. ![[5-Cycle Example.png|153]] – 5-cycle
3. ![[Cycle and Chord Example.png|186]] – In orange is a cycle, which is not an induced cycle, because there is a chord (marked green)
4. ![[Induced Cycle Example 01.png|188]] – in red is an induced 4-cycle
5. ![[Induced Cycle Example 02.png|192]] – in red is an induced 3-cycle -- a triangle
