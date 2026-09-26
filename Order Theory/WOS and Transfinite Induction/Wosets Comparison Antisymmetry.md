---
tags:
  - Statement
---
**Intuition.** Is it possible that the relation "[[Order Isomorphism|isomorphic]] to a [[Upset and Downset|downset]] of" on [[Well-Ordered Set|wosets]] is not antisymmetric for in the sense $\mathbb{W}$ is isomorphic to a downset of $\mathbb{V}$ and vice versa, but $\mathbb{V}$ and $\mathbb{W}$ are not isomorphic? The answer is "no"; next theorem and corollary proves it. Note: this is not a relation on a certain set, because all the wosets form a proper class, so we are asking about the formula representing this relation, not about a set.

**Theorem.** Let $\mathbb{W}=(W,\leq)$ be a woset, then a downset $D \subseteq W$ is isomorphic to $W$ (both sets are considered with $\leq$ relation) only if $D=W$.
$\blacktriangle$ Assume the opposite, i.e. $\exists f: W \rightarrow D$ – isomorphism. By [[Form of Arbitrary Downset of Woset]] $D=[0,d)$ for some $d \in W$. The $f$ is a [[Strict Order Homomorphism|strict endomorphism]], because it's an order isomorphism between a [[Partial Order|poset]] and its [[Subposet|subposet]], so by [[Woset Strict Endomorphism Lemma]] $\forall w \in W\ f(w) \geq w$, in particular $f(d) \geq d$ – contradiction to $d \notin Im_f(W)$.

**Corollary.** Let $\mathbb{W}=(W, ≤_w)$, $\mathbb{V} = (V, \leq_V)$ be well-ordered sets. If $\mathbb{W}$ is isomorphic to a downset of $\mathbb{V}$ and $\mathbb{V}$ is isomorphic to a downset of $\mathbb{W}$, then $\mathbb{V} \cong \mathbb{W}$ and the downsets are exactly W and V.
$\blacktriangle$ Let $f: W → D_\mathbb{V}$ and $g: V → D_\mathbb{W}$ be isomorphisms, where $D_\mathbb{V} ⊆ V$ and $D_\mathbb{W} ⊆ W$ are downsets.
Then $f\circ g$ would be an isomorphism between $V$ and some $D'_\mathbb{V} = Im_f(D_\mathbb{W})$, and $D'_\mathbb{V}$ is a downset of $\mathbb{V}$ [[Isomorphic Image of Downset is Downset|as an isomorphic image of a downset]] – contradicts the previous theorem unless $D'_\mathbb{V} = V ⇒ D_\mathbb{V} = V$ because $D_\mathbb{V} \subseteq D'_\mathbb{V}$.
Same way we get $D_\mathbb{W}=W$ by considering $g \circ f$.