---
tags:
  - Order-Theory
  - Statement
---
**Statement.** Let $\mathbb{W} = (W, \leq)$ be a [[Well-Ordered Set|woset]]. Then $\mathbb{W}$ has a [[Fixed Point Property|fixed point property]] $\iff$ it has a [[Least and Greatest Elements|greatest element]].
$\blacktriangle (\implies)$ Assume it doesn't have a greatest element. Then $w \mapsto w + 1$ is an [[Fixed Point and Fixed-Point-Free|FPF]] [[Order Endomorphism|endomorphism]] of $\mathbb{W}$ — contradicts FPP.
$(\impliedby)$ Assume there exists f – an FPF endomorphism of $\mathbb{W}$. By transfinite induction prove $\forall w \in W$ we have $f(w) > w$.
Base: 0 – [[Least and Greatest Elements|least element]] of $\mathbb{W}$:
	1. we can't have $f(0) < 0$, because $0$ is the least element;
	2. we can't have $f(0) = 0$, because $f$ is FPF,
	3. hence $f(0) > 0$, because $\mathbb{W}$ is [[Linear Order (Chain)|linear]].
Step: assume for all $w' < w$ we have $f(w') > (w)$. Then $f(w) \geq w$ by $f$ being an endomorphism, and $f(w) \neq w$ by $f$ being FPF, so $f(w) > w$ — exactly what we wanted.
Now we have $\forall w \in W \quad f(w) > w$. Apply to the greatest element of $\mathbb{W}$ to get a contradiction to its greatness. $\boxtimes$