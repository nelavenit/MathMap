---
tags:
  - Example
---
**Definition.** Let $\mathbb{P} = (P, \leq_P)$ and $\mathbb{Q} = (Q, \leq_Q)$ be [[Partial Order|posets]], $p_0 \in P$, if there are $q_1, q_2 \in Q$ s.t. $q_1 <_Q q_2$ (i.e. $\mathbb{Q}$ is not an [[Antichain|antichain]]), then $f: P \rightarrow Q$ s.t.
$$f(p) := 
\begin{cases}
q_2, \text{ if } p \geq_P p_0 \\
q_1, \text{ else}
\end{cases}$$
is called <u>generic order homomorphism</u>. Function $f$ may be seen as a parametrized: $f[p_0, q_1, q_2](\cdot)$.

In other words $f$ is such function, that $f^{-1}(q_2) = \mathord{\uparrow}{p_0}$ and $f^{-1}(q_1) = P\ \setminus  \mathord{\uparrow}{p_0}$.

**Statement.** For any posets $\mathbb{P} = (P, \leq_p)$ and $\mathbb{Q} = (Q, \leq_q)$, $p_0 \in P$ and $q_1, q_2 \in Q$ s.t. $q_1 <_q q_2$ the function $f[p_0, q_1, q_2](\cdot)$ is a [[Order-preserving map (Order Homomorphism)]].
$\blacktriangle$ 
Fix $x,y∈P$ s.t  $x≤y$, let's consider cases:
1. $x \geq_P p_0 , y \geq_P p_0$, then $f(x) = q_2 = f(y)$
2. $x \geq_P p_0 , y \ngeq_P p_0$, impossible because $y \geq_P x$
3. $x \ngeq_0 p_0, y \geq_P p_0$, then $f(x) = q_1 <_Q q_2 = f(y)$
4. $x \ngeq_P p_0 , y \ngeq_P p_0$, then $f(x)=q_2=f(y)$ $\boxtimes$

**Statement.** If $\exists p \in P$ s.t. $p < p_0$ or $p$ and $p_0$ are $\leq_P$-incomparable, then $f[p_0, q_1, q_2]$ is non-trivial.
$\blacktriangle$ $f[p_0, q_1, q_2]$ casts $p \mapsto q_1$ and $p_0 \mapsto q_2$.  

**Intuition.** This homomorphism is called "generic" because is exists for every non-trivial orders pair, basically we made $f$ non-trivial by mapping $p,p_0$ into non-trivial pair $q_1,q_2$ and squashing other points into $q_1$ and $q_2$.
