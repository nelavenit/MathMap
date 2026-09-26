---
tags:
  - Definition
---
**Intuition.** Let's stack [[Crown|crowns]] of the same size on top of each other, with the bottom of the upper crown being the top of the lower crown. Let's first give example [[Hasse Diagram|Hasse diagrams]] and give a formal (rather tedious, but obvious) definition of this [[Partial Order|poset]] after. 

**Examples.**
1. 3 crowns, 4 elements each ![[Crown Tower Example 01.png|100]]
2. 3 crowns, 6 elements each ![[Crown Tower Example 02.png|200]]
3. Same as in 2, but drawn differently ![[Crown Tower Example 03.png|202]]

**Definition.** Let $n,m \in \mathbb{N}$, $n \geq 2$. For $j\in\{1,\ldots,m\}$ let $\mathbb{C}_j:=(C^j,\leq^j) = (\{b_1^j,\ldots,b^j_n, t_{1}^j, \ldots, t_n^j \},\leq^j)$ be crowns with $2n$ elements each such that, for all $i\in\{1,\ldots,n\}$ and $j\in\{2,\ldots,m\}$, we have $t_{i}^{j-1}=b_{i}^j.$ Let $\prec_j$ be the lower cover relation of $\mathbb{C}_j$. Equip $CT_{2n}^m:=\bigcup_{j=1}^m C_j$ with the order induced by the lower cover relation which is the union $\bigcup_{j=1}^m\prec_j$ of the individual lower cover relations.
The ordered set $\mathbb{CT}_{2n}^m$ thus obtained is called a <u>$2n$-crown tower with $m$ crowns</u>. 

