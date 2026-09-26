---
tags:
  - Statement
---
**Intuition.** Both [[Width|width]] and [[Order Diameter|diameter]] of the [[Partial Order|poset]] in a way describe how wide the [[Hasse diagram]] may be, how "far" the vertices may be from one another. This are related one way, and not related the other.

**Statement 1.** Let $\mathbb{P} = (P, \leq)$ be a poset, then $\left\lceil \frac{\operatorname{diam}(\mathbb{P}) + 1}{2}\right\rceil \leq w(\mathbb{P})$ and this inequality can't be improved. 
$\blacktriangle$ A [[Fence|fence]] of the [[Fence|length]] $n$ has an [[Antichain|antichain]] of the size $\left\lceil \frac{n + 1}{2} \right\rceil$: it's either all the [[Minimal and Maximal Elements|maximal]] elements or all [[Minimal and Maximal Elements|minimal]] elements. By definition of the diameter, we have a fence of the size $\operatorname{diam}(\mathbb{P})$, hence the statement. 
This inequality cannot be improved: consider $2k$-fence. It has diameter $2k-1$ and width $k$. $\boxtimes$

**Statement 2.** The inverse, i.e. upper-bounding width with a diameter is impossible.
$\blacktriangle$ Consider the following order:
![[Pasted image 20260926131425.png|246]]
It has width $|A|$ for any set $A$ (including the infinite one) and diameter is $2$. $\boxtimes$

TODO Examples