---
tags:
  - Definition
---
**Intuition.** Same as in graph theory, we consider maximal connected parts of the [[Hasse Diagram|Hasse diagram.]]

**Definition.** Let $\mathbb{P} = (P, \leq)$ be a [[Partial Order|poset]]. The [[Minimal and Maximal Elements|maximal]], with respect to inclusion, [[Connectivity|connected]] subset of $P$ is called <u>connected component</u> (sometimes simply <u>component</u>).

**Statement.** Let $\mathbb{P} = (P, \leq)$ be a poset, $S \subseteq P$ – connected in $\mathbb{P}$. Then there exists the [[Least and Greatest Elements|greatest]] (hence maximal), with respect to inclusion, set $C \subseteq P$ connected in $\mathbb{P}$, s.t. $S \subseteq C$. 
$\blacktriangle$ Let $\{ C_i \}_{i \in I}$ be a set of all subsets of $P$, that contain $S$ and are connected. Consider $C := \bigcup\limits_{i \in I} C_i$. It obviously is subset of $P$, contains $S$ and is the greatest connected, if connected. So it's only required to show, that $C$ is connected. Take $p,q \in C$, by definition of $C$ there are $C_i, C_j$ s.t. $p \in C_i, q \in C_j$. Both are connected and contain $S$ so choose any $s \in S$. There would be a [[Fence|fence]] in $C_i$ with $s$ and $p$ as [[Fence|endpoints]] and a fence in $C_j$ with $s$ and $q$ as endpoints. Thus, after possibly removing some elements (parts between elements present in both fences), the union of this two fences is a fence with $q$ and $p$ as endpoints. $\boxtimes$