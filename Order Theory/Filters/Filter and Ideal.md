---
tags:
  - Definition
---
**Intuition.** [[Principal Filter and Ideal|Principal filters]] (ideals) are a natural and important subjects of research. Let's generalize the concept to get a wider class of [[Partial Order|order]] subsets, but that every its member will possess some essential principal filter (ideal) properties.

**Definition.** Let $(P,\leq)$ be a poset, $F\subseteq P$ is called a <u>filter</u>, if:
1) $F$ is an [[Upset and Downset|upset]]
2) $F$ is [[Upward and Downward Directed Subsets|downward directed]]

**Definition.** Analogously $I\subseteq P$ is called an <u>ideal</u>, if
1) $I$ is a [[Upset and Downset|downset]]
2) $I$ is [[Upward and Downward Directed Subsets|upward directed]]

**Example.** ![[Filter and Ideal Example 1.png|300]]
**Example.** ![[Filter and Ideal Example 2.png|300]]
**Example.** Consider [[Finite Partial Functions|finite partial function]] poset ($Fn(\mathbb{N},\{0,1\}),\subseteq$). Then set $\{\emptyset,\{(0,1)\},\{(1,1)\},\{(0,1),(1,1)\}\}$ is an ideal.

**Statement.** Being a filter and being an ideal are [[Dual Properties|dual properties]].
$\color{red}\text{Proof}$ is a trivial exercise.

**Remark.** Depending on the topic where filters are used different object names are most common:
1. An ideal may be called a filter (e.g. by some authors in forcing theory @halbeisenCombinatorialSetTheory2017), this isn't a radical thing since these are the [[Dual Properties|dual]] objects
2) Principal filters (ideals) may be called <u>principal upsets</u> (<u>principal downsets</u>) @daveyIntroductionLatticesOrder2002
