---
tags:
  - Statement
  - Set-Theory
  - AC-used
---
**Statement.** Consider a circle and let there be a sigma-additive measure μ on a circle s.t.:
1) $\mu \not\equiv 0$
2) for any $X \in dom(μ)$ we have $μ$ – invariant under the rotation of the $X$ (which is exactly what we want from a sensible measure)
Then, if we accept [[Axiom of Choice|AC]], $\mu$ can't be defined on every circle subset.
$\blacktriangle$ Let's say two points on a circle are $\sim$ iff the angle of an arc between them is rational. This is an equivalence relation, so we can consider a quotient set, let's choose a single representative of an each equivalence class. Let $M$ be a set of all representatives (here is when we use AC). If we rotate $M$ by any rational angle $α,$ s.t. $0 < α < 2π$, we will get a set with no intersection with $M$ (by a definition of $\sim$, else we get different classes representatives differ by a rational angle). Let's call rotated set $M_\alpha$. Every point has a representative of its class, so $\bigcup_{\alpha \in \mathbb{Q}} M_\alpha$ covers the whole circle. So we partitioned a circle into a countable number of sets that differ only by rotation. 
Assume there is a $\mu$ satisfying the conditions (1) and (2) and it is defined on every subset of a circle. Then either $\mu(M)=0 \Rightarrow \mu(circle)=\mu(\bigcup_{\alpha \in \mathbb{Q}} M_{\alpha})=\sum_{\alpha \in \mathbb{Q}} \mu(M_{\alpha})=\\ \sum_{\alpha \in \mathbb{Q}} 0 = 0$ or $\mu(M) \neq 0 \Rightarrow \sum_{\alpha \in \mathbb{Q}} \mu(M_{\alpha})=\sum_{\alpha \in \mathbb{Q}} \mu(M) = \infty$. So $\mu$ can't be defined on $M$, i.e. $M$ is an unmeasurable set.

**Intuition.** In fact building an unmeasurable set requires some way to get "indescribable" sets (for example an AC), in ZF it's impossible to build one. The proof is a Solovay model of ZF in which all subsets of $\mathbb{R}$ are Lebesgue measurable.

**Remark.** The same idea is used to build an unmeasurable set on a real line $\mathbb{R}$ (see Vitali set), but for a bit shorter proof we would consider a measure on a circle.