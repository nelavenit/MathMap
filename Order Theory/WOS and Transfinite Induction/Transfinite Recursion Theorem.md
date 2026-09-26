---
tags:
  - Statement
---
**Intuition.** Our goal is to learn to give recursive function definitions not only on natural numbers, but on an arbitrary [[Well-Ordered Set|well-ordered set]]. I.e. $f(w)$ is defined using values of $f(\cdot)$ on $[0,w)$.

**Statement.** Let $\mathbb{W} = (W, \leq)$ be a [[Well-Ordered Set|woset]]. A – arbitrary set. Let there be a recursive rule, that is a function $F$ that maps an element $w \in W$ and a function $g: [0, w) \rightarrow A$ into an element of $A$. Then exists and is unique a function $f: W \rightarrow A$ s.t. $\forall w \in W\  f(w) = F(w, f|_{[0, w)})$.
$\color{red}\text{Proof idea:}$ 
1.   Transfinite induction on "a": we want $\forall w \in [0,a] \, f(w)=F(w,f\vert_{[0,w)})$.
	Assume for each $c < a$ We have $\exists f_c$ s.t. $\forall w \in [0,c] \, f_c(w)=F(w,f_c\vert_{[0,w)})$.
	Consider $c_1 < c_2$, show $f_{c_1}\vert_{[0,\min(c_1,c_2)]}=f_{c_2}\vert_{[0,\min(c_1,c_2)]}$
2.   This means $h:=\bigcup_{c<\alpha}f_c$ is a correct function $h: [0,a) \rightarrow B$.
	We add $(a,F(a,h))$ to the $h$ and get the desired $f_a$
3.   Same way we get $f=\bigcup_{a\in W}f_a$

**Intuition.** In practice we often need to get $f$ when F is partially defined (i.e. for some $w∈W$ and $g : [0,w) → A$ it is not defined). Let's address such case.

**Statement.** Let $\mathbb{W} = (W, \leq)$ be a woset, $A$ – arbitrary set. Let there be a recursive rule, that is a partially defined $F$ that maps an element $w \in W$ and a function $g: [0, w) \to A$ into an element of $A.$ Then exists such $f$, that:  
1. either is defined on $W$ and is consistent with the recursive definition  
2. or is defined on some [[Upset and Downset|downset]] $[0, w_0)$ and on it is consistent with the recursive definition, moreover $F(w_0, f)$ is undefined

$\color{red}\text{Proof idea:}$
Let's add "$\perp$" – the "undefined" sign to $A: A' := A \cup \{\perp\}$.
Let $F'$ be $F$ with the value "$\perp$" in every case $F$ was not defined.
Now $A'$ and $F'$ satisfy the previous theorem assumption $\Rightarrow$ $∃f' : W → A'$
1. If $\perp ∉ Im(f')$, then we have the first case and $f := f'$
2. Else let $w$ be least element of $\{ w ∈ W | f'(w) = \perp \}$, then $f := f'|_{[0,w)}$ satisfies the second case
