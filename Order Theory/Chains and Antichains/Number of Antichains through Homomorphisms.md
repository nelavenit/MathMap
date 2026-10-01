---
tags:
  - Statement
  - Finite
---
**Intuition.** Let $\mathbb{P} = (P, \leq)$ be a *finite* [[Partial Order|order]] and $\mathbb{C}_2 = (\{0,1\},\{(0,0),(0,1),(1,1)\}$ be a two-element [[Linear Order (Chain)|linear order]]. What is $\operatorname{Hom}(\mathbb{P}, \mathbb{C}_2)$? 
We decide which elements to cast into $1$ and which into $0$. If we cast $X$ into $0$, then the whole $\mathord{\downarrow} X$ needs to be cast into $0$ for the map to be [[Order-preserving map (Order Homomorphism)|order-preserving]]. So it's enough to describe all the [[Upset and Downset|downsets]] $D$ of $\mathbb{P}$, and for each we would have a homomorphism:
$$f_D(p) = 
\begin{cases}
1,\text{if } p \notin D \\
0,\text{if } p \in D \\
\end{cases}$$
And, in the same time, $\mathbb{P}$ is finite, so we [[Number of Antichains through Downsets|have a bijection]] between [[Antichain|antichains]] of $\mathbb{P}$ and downsets of $\mathbb{P}.$ 

**Statement.** Let $\mathbb{P} = (P, \leq)$ be a *finite* order. Then the number of [[Antichain|antichains]] in $\mathbb{P}$ is equal to the number of homomorphisms from $\mathbb{P}$ to the two-element linear order $\mathbb{C}_2$.
$\blacktriangle$ (strongly reworked version of Pr.2.36. from @schroderOrderedSetsIntroduction2016) 
By [[Number of Antichains through Downsets]] statement we have to just find a bijections between the set of all downsets of $\mathbb{P}$ and $\operatorname{Hom}(\mathbb{P},\mathbb{C}_2)$. Let $\mathcal{D}(\mathbb{P})$ be a set of all downsets of $\mathbb{P}$, define $F: \mathcal{D}(\mathbb{P}) \rightarrow \operatorname{Hom}(\mathbb{P},\mathbb{C}_2)$ such, that $F(D) :=  f_D$ as discussed in the intuition part:
1. Correctness: the only way for $f_D$ not to be a homomorphism is a pair $p,q \in P$ s.t. p < q, but $f_D(p) = 1 > 0 = f_D(q)$, which is impossible because $f_D(q) = 0$ implies $q \in D$, which implies $p \in D$ by $D$ being a downset, which, in turn, implies $f_D(p) = 0$ — contradiction.
2. Injectivity proof is a trivial exercise
3. Surjectivity: assume $f \in \operatorname{Hom}(\mathbb{P},\mathbb{C}_2)$, then $f^{-1}[0]$ is a downset by order-preserveness of $f$ because $0$ is the [[Least and Greatest Elements|least element]] of $\mathbb{C}_2$. And, because the range has only two elements, $f^{-1}[0]$ uniquely defines the $f$ on other elements and we get $f = f_{f^{-1}[0]}$, so $f^{-1}[0] = F^{-1}(f)$. $\boxtimes$

**Example.** 
Here what we do is $A \mapsto f_{\mathord{\downarrow}A}$
![[Number of Antichains through Homomorphisms Example.jpg|450]]
