---
tags:
  - Statement
---
**Notation.** When considering [[Well-Ordered Set|wosets]] we will call an [[Lower and Upper Covers, Adjacence|upper cover]] of an element a <u>successor</u>. Let $\mathbb{W} = (W, \leq)$be a woset, $w\in W$. We will denote an upper cover of $w$ as $w + 1$, an upper cover of $w + 1$ as $w + 2$ and so on.

**Statement.** Let $\mathbb{W} = (W,\leq)$ be a well-ordered set, then every element $w\in W$, except for the [[Least and Greatest Elements|greatest element]] (if such element exists), has an upper cover.
$\blacktriangle$ Consider $W \setminus \mathord{\downarrow}{w}$, it [[Every Woset Subposet has Least Element|has]] a [[Least and Greatest Elements|least element]], this would be our $w+1$:
1. $w+1$ is greater than $w$ because $w+1 \notin\ \mathord{\downarrow}{w}$ and the order is [[Linear Order (Chain)|linear]] 
2. $\nexists p \in W$ s.t. $w<p<w+1$, because $p$ would be in $W\setminus\mathord{\downarrow} w$ – contradicts $w+1$ being the least element $\boxtimes$

**Notation.** In the similar manner sometimes a [[Lower and Upper Covers, Adjacence|lower cover]] in a woset is called a <u>predecessor</u>,

**Remark.** In some sources the successor element of $w$ is denoted as $S(w)$, and then $w + 3$ is $S(S(S(w))) = S^3(w)$.