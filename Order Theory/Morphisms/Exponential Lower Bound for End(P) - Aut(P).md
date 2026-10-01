---
tags:
  - Statement
---
**Statement.** Let $\mathbb{C}=(C,\leq)$ be a *finite* [[Linear Order (Chain)|chain]] of the [[Chain Length|length]] $l=|C|-1>0$. Then $\mathbb{C}$ has at least $2^l = 2^{|C|-1}$ [[Order Endomorphism|endomorphisms]] that are not [[Order Automorphism|automorphisms]].
$\blacktriangle$ For each element we decide whether $\left[ \begin{array}{ll} a_i \mapsto a_{i+1} \\ a_i \mapsto a_i \end{array} \right .$ , where $a_{i+1}$ is an [[Lower and Upper Covers, Adjacence|upper cover]] of $a_i$, and $a_{|C|} \mapsto a_{|C|}$. This way we would have $2^{|C|-1}$ endomorphism, but one of them is an automorphism, so lets replace it with $f := const = a_{|C|}$.
Note: doesn't work when $|c| = 1$ because $f$ was already considered, so in case $|C| = 2$ we fix $f' := const = a_0$. $\boxtimes$

**Statement.** Let $\mathbb{P}=(P,\leq)$ be a *finite* [[Partial Order|poset]] with $|P|=n>1$ and $h(\mathbb{P})=h$. Then $\mathbb{P}$ has at least $2^{\frac{h}{h+1}n}$ endomorphisms that are not automorphisms.
$\blacktriangle$ 
1. If $\mathbb{P}$ is a chain then we have a previous statement. Let’s assume $\mathbb{P}$ is not a chain.
2. Let $c_0 \ldots c_h$ be a chain and let $r_0 \ldots r_h$ be the numbers of elements of every [[Rank|rank]]. Consider $j$ be a number of the smallest $r$, i.e. $∀i\ rⱼ ≤ rᵢ$. Let also $R_0 \ldots R_k$ be the sets of elements of every rank. Then for any $U_0 \subseteq R_0 , \ldots , U_k \subseteq R_k$ we would have an endomorphism which:
	1. For each $i < j$ it casts $U_i$ to $c_{i+1}$ and $R_i \setminus U_i$ to $c_i$
	2. For each $i >j$ it casts $u_i$ to $c_{i-1}$ and $R_i \setminus U_i$ to $c_i$
	3. casts $R_j$ to $c_j$	   
	![[Endomorphism Creation Scheme for Exponential Gap Theorem.png|250]]
	This is an endomorphism (verifying so is a simple exercise) and not an automorphism, because $\mathbb{P}$ is not a chain $\implies$ $∃rᵢ>1$ $\implies$ our morphism is not injective because there is only a single node of the every rank at maximum.	   
3. Number of such endomorphisms is $\prod_{i=0}^{j-1} 2^{r_i} \cdot \prod_{i=j+1}^{h} 2^{r_i} = 2^{n - r_j} \geqslant 2^{n - \frac{n}{h+1}} = 2^{\frac{h}{h+1}n}$. $\boxtimes$ 

**Corollary.** Let $\mathbb{P} = (P, \leq)$ be a poset, then $|End(\mathbb{P}) \setminus Aut(\mathbb{P})| \geq 2^{\frac{|P|}{2}}$.
$\blacktriangle$ If $h(\mathbb{P}) = 0$, $\mathbb{P}$ is an [[Antichain|antichain]] and every non-bijective function lies in $End(\mathbb{P}) \setminus Aut(\mathbb{P})$. Else, if $h > 0$, then $\frac{h}{h+1} > \frac{1}{2},$ hence we get the desired statement by the previous theorem. $\boxtimes$