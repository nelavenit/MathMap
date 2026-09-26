---
tags:
  - Statement
  - AC-used
---
**Statement.** Let $(P, ≤)$ be a [[Partial Order|poset]], then $\leq$ can be extended to be a [[Linear Order and Chain|linear ordering]], i.e. $∃ ≤_L s.t. ≤ ⊆ ≤_L$ and $(P, ≤_L)$ is a linear order.
$\blacktriangle$
1. Consider $Q ⊆ powerset(P×P)$ – a set of all orderings of $P$ that contain $≤$. Consider $\mathbb{Q} = (Q, \subseteq),$ let's show this poset satisfies the [[Zorn's Lemma|Zorn's lemma]] condition. Let C ⊆ Q be a chain in $\mathbb{Q}$, then $\preccurlyeq := \bigcup_{≤' ∈ C} ≤'$ is an ordering and an [[Lower and Upper Bounds|upper bound]] of C:
	1. Transitivity of $\preccurlyeq$: $p_1 \preccurlyeq p_2$ and $p_2 \preccurlyeq p_3$ $\iff$ $\exists \leq_1 \in C$ s.t. $p_1 \leq_1 p_2$ and $\exists \leq_2 \in C$ s.t. $p_2 \leq_2 p_3$.
	  $C$ is a chain $\implies$ either $\leq_1 \subseteq \leq_2$ or $\leq_2 \subseteq \leq_1$ $\implies$ Either $p_1 \leq_2 p_2$  and  $p_2 \leq_2 p_3$ or  $p_1 \leq_1 p_2$ and $p_2 \leq_1 p_3$ $\implies$ either way $p_1 \preccurlyeq p_3$ by the transitivity of $\leq_1$ and $\leq_2$
	2. Reflexivity: trivial
	3. Antisymmetry: same way as with transitivity we would have $p_1 \preccurlyeq p_2 \wedge p_2 \preccurlyeq p_1 \Rightarrow \exists \leq_1 \in C$ s.t. $p_1 \leq_1 p_2 \wedge p_2 \leq_1 p_1 \Rightarrow p_1=p_2$ by antisymmetry of $\leq_1$
	4. Being an upper bound is trivial
2. Then by applying Zorn's lemma to $\mathbb{Q}$ we get $\leq_L \in Max(\mathbb{Q})$. Let's show $\leq_L$ is a linear ordering: assume the opposite - let $p_1, p_2 \in P$ be $\leq_L$-incomparable.
   Define $\leq'$:
	$$a \leq' b \overset{def.}{\iff} \left\{ \begin{array}{l} a \leq_L b \\ a \leq_L p_1 \text{ and } p_2 \leq_L b \end{array} \right.$$
	i.e. add $(p_1, p_2)$ and do a transitive closure. Let's prove $\leq'$ is an ordering:
	1. Reflexivity: $\forall p \in P$ $p \leq_L p \Rightarrow p \leq' p$
	2. Transitivity: $q_1, q_2, q_3 \in P$, $q_1 \leq' q_2$ and $q_2 \leq' q_3$. There are 4 cases of how this two relations were derived from $\leq_L$:
		1. $q_1 \leq_L q_2$, $q_2 \leq_L q_3$ — then $q_1 \leq_L q_3$ $\implies$ $q_1 \leq' q_3$
		2. $q_1 \leq_L q_2$, $q_2 \leq_L p_1$, $p_2 \leq_L q_3$ $\implies$ $q_1 \leq_L q_3$ $\implies$ $q_1 \leq' q_3$ by $\leq'$ definition
		3. $q_1 \leq_L p_1$, $p_2 \leq_L q_2$, $q_2 \leq_L q_3$ — analogously to (2)
		4. $q_1 \leq_L p_1$, $p_2 \leq_L q_2$, $q_2 \leq_L p_1$, $p_2 \leq_L q_3$ $\implies$ $p_2 \leq_L p_1$ — contradicts $p_1$ and $p_2$ being $\leq_L$-incomparable
	Then $\leq'$ is an ordering of $P$, containing $\leq$, and $\leq_L \subsetneq \leq'$ — contradicts the [[Minimal and Maximal Elements|maximality]] of $\leq_L$. $\boxtimes$

**Statement.** Not every partial ordering can be extended to be a [[Well-Ordered Set|well-ordering]].
$\blacktriangle$ For example assume any linear ordering, which is not [[Well-Founded Order|well-founded]], e.g. ($\mathbb{Z}$, $\leq$).