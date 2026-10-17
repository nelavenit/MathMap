---
tags:
  - Statement
---
**Statement (Alternative definition of a Well-ordered set).** Let $\mathbb{W} = (W, \leq)$ be a [[Partial Order|poset]]. Then $\mathbb{W}$ is a [[Well-Ordered Set|woset]] iff for every $X \subseteq W$ the [[Subposet|subposet]] $\mathbb{W}|_X$ has the [[Least and Greatest Elements|least element]].
$\blacktriangle$ $(\implies)$ By [[Well-Founded Order|well-foundedness]] of $\mathbb{W}$ any $X \subseteq W$ has a [[Minimal and Maximal Elements|minimal element]], by [[Linear Order (Chain)|linearity]] of $\mathbb{W}$ this element [[Minimal and Least, Maximal and Greatest in Linear Orders|is]] also the least.
$(\impliedby)$ We need to prove that $\mathbb{W}$ is both well-founded and linear:
1. Every least element is minimal so the order is well-founded
2. Assume $\mathbb{W}$ is not linear, then there are two $\leq$-incomparable elements $w_1, w_2 \in W$. Consider $\{ w_1, w_2\}$. It's a subset of $W$, so $\mathbb{W}|_{\{ w_1, w_2\}}$ has a least element — contradicts 