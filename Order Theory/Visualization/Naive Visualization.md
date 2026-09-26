---
tags:
  - Intuition
---
Any finite [[Partial Order|poset]] $\mathbb{P} = (P, \leq)$ can be visualized as a directed graph: $V := P,\ E\ := \leq$.

But the picture will be overloaded will edges, the way to avoid it is not to add transitive edges: draw ![[Small Directed Graph without Transitive Edge.png|200]]instead of ![[Small Directed Graph with Transitive Edge.png|170]].
Formally our diagram is a directed graph of [[Lower and Upper Covers, Adjacence|cover]] relation.

These are 3 diagrams showing the same order:
![[Naive Visualization Example 1.png|200]] ![[Naive Visualization Example 2.png|220]] ![[Naive Visualization Example 3.png|230]]
This example shows that by using arbitrary directed graph visualization it is both:
1. Hard to analyze the order: 3 quite differently looking diagrams for the same order
2. Quite difficult to be sure [[Symmetry and Antisymmetry|antisymmetry]] is not broken by some cycle