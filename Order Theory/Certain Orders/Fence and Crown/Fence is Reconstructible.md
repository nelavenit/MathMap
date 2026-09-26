---
tags:
  - Statement
  - Finite
---
**Statement.** [[Fence|Fences]] of at least 4 elements are [[Reconstructibility|reconstructible]].
$\blacktriangle$ Let's show that: $\mathbb{P}$ is a fence of at least 4 elements $\iff$ two [[Card|cards]] of $\mathbb{P}$
are fences and all the rest of cards are the union of two fences.
$\boldsymbol{(\Longrightarrow)}$ Obvious
$\boldsymbol{(\Longleftarrow)}$
1. If two cards are fences, i.e. connected, we know the whole $\mathbb{P}$ is connected
2. If another card in a union of two fences, say $F_1$ and $F_2$, this means the removed vertex $r$ made the order connected, so $\exists f_1 \in F_1, f_2 \in F_2$ s.t. $r \sim f_1$ and $r \sim f_2$.
   The picture is:![[Fence is Reconstructible Proof Illustration 01.png]]
   Let's call the [[Fence|endpoints]] of $F_1$ – $f_{end_0}$ and $f_{end_1}$, the endpoints of $F_2$ – $f_{end_2}$ and $f_{end_3}$.
   $r$ can't be connected to any other element of $F_1$ other than $f_1$ because else the card with $f_{end_3}$ removed wouldn't be a fence or two fences. In the following picture this means that blue edges are impossible: ![[Fence is Reconstructible Proof Illustration 02.png]]
   Then the card with $f_1$ removed would be a union of three fences (which contradicts the antecedent, unless $f_1$ is an endpoint of $F_1$. Same way we get $f_2$ be an endpoint of $F_2$. So, WLOG, $f_1 = f_{end_1}$ and $f_2 = f_{end_2}$. Now the picture is:![[Fence is Reconstructible Proof Illustration 03.png]]
3. Now there are 4 cases of how $f_1$ and $f_2$ are either at the top or at the bottom of the fence. And for each case there are 4 cases of how $r$ is related to $f_1$ and $f_2$:
	1. $g < f_1 \land d > f_2$
		1. $r > f_1 \land r > f_2$ — card with $f_{end_0}$ (or with $f_{end_3}$ if F_1 is of 1 or 2 elements only) removed is not a fence of two fences, so this case is impossible
		2. $r > f_1 \land r < f_2$ — same as 3.1.1.
		3. $r < f_1 \land r < f_2$ — same as 3.1.1.
		4. $r < f_1 \land r > f_2$ — same as 3.1.1.
	2. $g< f_1 \land d < f_2$
		1.  $r > f_1 \land r > f_2$ — same as 3.1.1.
		2. $r > f_1 \land r < f_2$ — same as 3.1.1.
		3. $r < f_1 \land r < f_2$ — $\mathbb{P}$ is a fence
		4. $r < f_1 \land r > f_2$ — same as 3.1.1.
	3. $g > f_1 \land d > f_2$ — same as 3.2.
	4. $g > f_1 \land d < f_2$ — same as 3.1. $\boxtimes$



TODO reference to connectivity of an order