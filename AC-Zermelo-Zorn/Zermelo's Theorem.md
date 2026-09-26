---
tags:
  - Statement
  - AC-used
---
**Statement (Zermelo's theorem, also called Well-ordering theorem).** 
Every set can be [[Well-Ordered Set|well-ordered]], i.e. $\forall X\ \exists ≤\ \subseteq{X\times X}$ s.t. $(X,≤)$ – woset.
This theorem is equivalent to the [[Axiom of Choice]].
$\blacktriangle$ (Th.24 from @vereshchaginNachalaTeoriiMnozhestv2012)
(AC $\Rightarrow$ WO) Let $X$ be a set and $f$ be a choice function from an [[Equivalent form of AC through Subset Complement|equivalent form of the AC]], i.e. $f: \mathcal{P}(X) \setminus \{X\} \to X$ s.t. $A \subsetneq X \mapsto f(A) \in X \setminus A$. 
Intuition:
	we want to do kinda a transfinite induction: $x_0 = f(\emptyset)$, $x_1 = f(\{x_0\})$, $x_2 = f(\{x_0, x_1\})$. The problem is we need to already have some well-ordered set, which is a cycle. Let's address this problem, while sticking to the idea  that $x = f([0, x))$ ($[0,x)$ is defined [[Form of Arbitrary Downset of Woset|here]]), i.e. $f$ gives us the next element.
Let $S \subseteq X$ and $(S, \leq_S)$ be a [[Partial Order|poset]]. We call it a <u>correct fragment</u> if
1. ($S$, $\le_S$) is a woset
2. $\forall s \in S$, $s = f([0,s))$
Idea:
	 (2) gives us that all correct fragments are "compatible", and as a result the union of all of them will be a poset.
	 (1) gives us that the union of all correct fragments will be well-ordered
Lemma:
	**Lemma 1.** Let $\mathbb{S} = (S, \leq_S)$, $\mathbb{T} = (T, \leq_T)$ be correct fragments of $X$. Then one of the sets [[Wosets Comparison|is]] a [[Upset and Downset|downset]] of the other, and moreover the relations are compatible, i.e. $\forall x,y \in T\cap S$ we have $x \leq_S y \iff x \leq_T y$.
	$\blacktriangle$ (of lemma 1) By [[Wosets Comparison]] either $\mathbb{S}$ is [[Order Isomorphism|isomorphic]] to a downset of $\mathbb{T}$, or vice versa. WLOG let $\mathbb{S}$ be isomorphic to a downset of $\mathbb{T}$ and $h: S \rightarrow T$ be an isomorphism. Lemma states that $h$ is an identity, i.e. $\forall x \in S\ h(x)=x$. Let's prove it by transfinite induction, now it is possible, because $\mathbb{S}$ is a woset.
	Induction step: let $\forall y \leq_S x$ $h(y)=y$. Consider downsets $[0,x)_S$ and $[0,h(x))_T$, by induction assumption they are the same sets and $\leq_T |_{[0,x)_S} = \leq_S |_{[0,x)_S}$, because they have the identity isomorphism. Then by the condition (2) for correct fragments $x=f([0,x)_S) = f( [0,h(x))_T) = h(x)$ – so an identity is an isomorphism, hence S is a downset of $\mathbb{T}$ and orders are the same. $\boxtimes$
Consider  $U = \bigcup\limits_{S \text{ – correct fragments of } X} S$. 
Let the order $\leq$ on $U$ be: $u₁, u₂ ∈ U$, by definition of $U$ this means such correct fragments $\mathbb{T} = (T, \leq_T), \mathbb{S} = (S, \leq_S)$ exist, that $u_1 ∈ T$ and $u_2 ∈ S$. Then by Lemma 1 either $T \subseteq S$ or $S ⊆ T$ $\Rightarrow$ WLOG $u_1, u_2 \in T$. Then define $u_1 \leq u_2 \overset{def.}{\iff} u_1 \leq_T u_2$.
This would be an ordering, lemma 1 provides that the relation is independent of the choice of $\mathbb{T}$. This order is linear as shown while defining.
Lemma:
	**Lemma 2.** $(U, \leq)$ is a woset. Let's show the order is well-founded. Assume the opposite, then by [[Well-Founded Order Criteria|well-foundedness criteria]] $\exists x_0 ≥ x_1 ≥ x_2 ≥ \ldots$ Assume $(T, ≤_T)$ be a correct fragment containing $x_0$ $\implies$ by *lemma 1* the set $T$ contains all $x ≤ x_0$, because if $x \leq x_0 \implies \exists (S, \leq_S)$ s.t. $x ≤_S x_0$, hence, by *lemma 1*, either 1) $S$ is a downset of $(T, ≤_T)$ – then $x ∈ T$ or 2) $T$ is a downset of $(S,\leq_S)$ – then again $x ∈ T \implies x_1, x_2, ... ∈ T$ – contradiction with well-foundedness of $(T, ≤_T)$. $\boxtimes$
Another point of view is "there exists a greatest (not even just maximal) correct fragment $U$".
Now we finish the proof: we have $(U,\leq)$-woset, $U \subseteq X$. Let's show $U=X$, assume the opposite: $U \neq X$, $x:=f(U)$ and consider new poset $(U,\leq)+\{x\}$ (definition of $+$ is [[Orders Sum|here]]), it's a correct fragment (it's a woset as a sum of wosets, it's correct by the choice of $x$, because $[0,x)=U$) — contradicts the construction of $U$.

(WO $\Rightarrow$ AC) We will use the usual form of AC: $\forall X$ s.t. $\emptyset \notin X \rightarrow ∃f : \forall A \in X$ we have $f(A) \in A$. Let $U := \bigcup X$, consider $(U, ≤)$ – well-ordering of $U$, now define $f$ as $f(A) := min(A)$ – well-defined because $A ⊆ U$. $\boxtimes$

**Intuition.** As Zermelo's theorem is equivalent to the AC, it also can be used to produce a number of unintuitive/unconstructible results.
**Example.** As an evident result of well-ordering theorem is the ability to well-order a real line $\mathbb{R}$. The problem is we can't present this very ordering, just prove it exists, and still there are. In fact, it is impossible within ZF. For example, we have a Solovay’s model, in which every set of reals is Lebesgue measurable — which implies there is no well-ordering of $\mathbb{R}$ (construction similar to [[Unmeasurable Set on Circle]] and Vitali set, just by using $min$ as a choice function).