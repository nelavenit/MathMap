---
tags:
  - Example
  - Finite
---
**Exercise.** (Pr.1.22. from @schroderOrderedSetsIntroduction2016) Prove the following order has the [[Fixed Point Property|fixed point property]].
![[Order with FPP Example 02.png|200]]
$\blacktriangle$ Let's call the [[Partial Order|ordered set]] $\mathbb{P}$ and suppose for a contradiction that there is an [[Order-preserving map (Order Homomorphism)|order-preserving map]] $F : P \to P$ such that F has no [[Fixed Point and Fixed-Point-Free|fixed point]]. Then $F(b)$ cannot be related to $b$ by [[Finite Height FPF Endomorphism Criterion]], thus $F(b) \in \{a, c\}$. 
Define $\Phi: P \rightarrow P$ s.t. $a \leftrightarrow c$, $b \mapsto b$, $d \leftrightarrow f$, $e \mapsto e$, $g \leftrightarrow k$, $h \mapsto h$. Because $\Phi$ is an [[Order Automorphism|automorphism]], we can assume without loss of generality that $F(b) = a$. (Otherwise we would apply the whole following argument to $\Phi^{-1} \circ F \circ \Phi$, which is a fixed point free endomorphism, too.)

Because $F(b)=a$, we have $F[\mathord{\uparrow}b] = F[\{d,e,g,h,k,f\}] \subseteq \mathord{\uparrow}{a} = \{a,d,e,g,h,k\}$. So, because $F(g)$ cannot be related to $g$ (again by [[Finite Height FPF Endomorphism Criterion|this]]), we must have $F(g) \in \{h,k\}$. If $F(g)=h$, then we must have that $a=F(b) \leq F(d) \leq F(g)=h$.

$F(d) = h$ would lead to $F(h) \geq F(d) = h$ and then $F(h) = h$, which is not possible. We exclude $F(d) = a$ in similar manner. This leaves $F(d) = d$, a contradiction.

Therefore we must have $F(g) = k$, which then leads to a contradiction in similar fashion. Thus $\mathbb{P}$ has no fixed point free endomorphisms and, hence, $\mathbb{P}$ has the fixed point property. $\boxtimes$