---
tags:
  - Statement
---
**Statement.** Let $\mathbb{W} = (W, \leq)$ be a [[Well-Ordered Set|woset]], then any $w \in W$ has a form: $z + n$, where $z$ is a [[Limit Element|limit element]] and $n$ is a natural number ($z + n$ is defined in [[Every Woset Element has Successor|here]]).
$\blacktriangle$ If $w$ is not a limit element, then let's take its predecessor: $v_1 \in W$ s.t. $w = v_1 + 1$ and repeat this process with v<sub>1</sub> and on until we get a limit element: v<sub>k</sub> s.t. w = v<sub>k</sub> + k, this will happen because else we found a descending sequence $w > v_1 > v_2 > \ldots,$ which contradicts [[Well-Founded Order|well-foundedness]] of $\mathbb{W}$.
The proof that this representation is unique is a simple exercise.

**Intuition.** The existence of such representation will work even in the case of just a well-founded order, but the uniqueness may not stand, as, for example, happens in this order:
![[Well-Founded Order with Non-unique Element Representation.png|600]]