---
tags:
  - Example
---
**Definition.** Let $D, R$ be arbitrary sets, then the set of <u>finite partial functions</u> denoted as $Fn(D,R)$ is a set of all functions $f$ such that:
1. $\text{dom}(f)$ is a finite subset of $D$ (i.e. $\text{dom}(f) \in \text{fin}(D)$)
2. $\text{ran}(f) \subseteq R$

**Definition.** Let's define $\leq$ on $Fn(D,R)$ as $f \leq g \iff f$ is a restriction of $g$, i.e.:
1. $\text{dom}(f) \subseteq \text{dom}(g)$
2. $g|_{\text{dom}(f)} = f$

**Statement.** $(Fn(D,R), \leq)$ is a [[Partial Order|poset]]. 
▲ One could verify the conditions directly, but it is useful for us to view $\mathcal{F}n(D,R)$ in terms of sets: by the definition of functions, $\mathcal{F}n(D,R)$ is a subset of $D \times R$, and the relation $\leq$ is exactly the inclusion relation $\subseteq$ on functions regarded as sets:
1. By definition, $\text{dom}(f) = \{ x \in D \mid \exists y \text{ s.t. } (x,y) \in f \}$. Furthermore, if $f \subseteq g$, then $(x,y) \in f$ implies $(x,y) \in g$. Thus, for any $x \in \text{dom}(f)$, it holds that $x \in \text{dom}(g)$.
2. Let $x \in \text{dom}(f) \cap \text{dom}(g)$. Then, by the definitions of a function and $\text{dom}$, there exist unique $y_1$ and $y_2$ such that $(x,y_1) \in f$ and $(x,y_2) \in g$. Since $f \subseteq g$, these pairs must coincide, which means $g(x) = f(x)$. Therefore, $g|_{\text{dom}(f)} \equiv f$ due to the arbitrary choice of $x$.
Then it is a poset by [[Set with Subset Relation is Poset|set with subset relation is a poset]].