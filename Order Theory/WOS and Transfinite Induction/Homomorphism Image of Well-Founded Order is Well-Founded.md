---
tags:
  - Statement
---
**Statement.** Let $\mathbb{P} = (P, \leq_P), \mathbb{Q} = (Q, \leq_Q)$ be [[Partial Order|posets]] and $\mathbb{P}$ is [[Well-Founded Order|well-founded]], $f: P \to Q$ is an [[Order-preserving map (Order Homomorphism)|order homomorphism]]. Then $(f(P), \leq_{f(P) \times f(P)})$ is well-founded.
$\blacktriangle$ Let $Y \subseteq Q$, consider $f^{-1}(Y) \subseteq P$. If $f^{-1}(Y) \neq \emptyset$, then 
$\exists m \in \text{Min}(f^{-1}(Y))$ by well-foundedness of $\mathbb{P}$, then $f(m)$ is [[Minimal and Maximal Elements|minimal]] in $A$: $\forall y \in Y \ \exists x \in f^{-1}(Y) \text{ s.t. } y = f(x)$, by the choice of $m$ we have $m \leq x \Rightarrow$ $f(m) \leq f(x) = y$ because $f$ is order-preserving $\Rightarrow f(m)$ is minimal in $Y$. $\boxtimes$ 