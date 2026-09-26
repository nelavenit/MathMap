---
tags:
  - Definition
---
**Intuition.** To address this problems of [[Naive Visualization|naive order visualization]] let's use the fact an [[Partial Order|order]] gives us a hierarchy of elements.

**Definition.** The <u>Hasse diagram</u> of a finite ordered set $(P, ≤)$ is the diagram of $(P, \prec)$ with all the edges going "down":
1. ($\mathbb{R}^2$ case) If $p < q$ then object representing $q$ is having a larger y-coordinate then the one representing $p$
2. (IR³ case) If $p < q$ then object representing $q$ is having a larger z-coordinate then the one representing $p$
3. Now height is an indicator of edge direction, so we can draw undirected edges
The Hasse diagram for the order from [[Naive Visualization|naive visualization]] is, for example, this
![[Hasse Diagram Example.png|200]]
Furthermore while presenting an order by giving its Hasse Diagram we guarantee the relation is indeed [[Symmetry and Antisymmetry|antisymmetric]].