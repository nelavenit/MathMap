---
tags:
  - Statement
---
**Intuition.** In [[Dilworth's Chain Decomposition Theorem]] we were searching for a decomposition of a [[Partial Order|poset]] of the [[Width|width]] $k$ into $k$ [[Linear Order and Chain|chains]]. The naive idea of taking arbitrary [[Maximal Chain|maximal chain]] to decrease the width didn't work, so we used a maximal strong k-dependent chain instead. But it's interesting to investigate when exactly just taking the maximal chain is enough.

**Statement.** Let $\mathbb{P} = (P, \leq)$ be a poset of the finite width. Then removal of any maximal chain strictly decreases the width of $\mathbb{P}$ iff $\mathbb{P}$ is [[CAC]]. (Note: this is a CAC order criteria only in the case of a finite width)
$\blacktriangle$ $\boldsymbol{(\Longleftarrow)}$ trivial
$\boldsymbol{(\Longrightarrow)}$ Assume there is a chain $C \subseteq P$ s.t. $w(P\setminus C) = w(P) := w$, then there is an antichain $A:= \{a_i\}_{i = 1}^w$ in $P\setminus C$. Let's show $A$ is also an antichain in $P$: assume the opposite, i.e. some elements of $A$ were comparable in $P$, which can't be changed by removing $C$ — contradiction, so $A$ is an antichain in $P$, it's a [[Maximal Antichain|maximal antichain]], because else $w(P)$ would be more than $w$, hence, by CAC of $\mathbb{P}$ we have $A \cap C \neq \emptyset$ — contradicts $A \subseteq P \setminus C$. $\boxtimes$ 

**Intuition.** In @grilletMaximalChainsAntichains1969 author uses the term **regular order**, he gives the motivation for considering this specific class, but this motivation seems wrong (his definition has very little in common with this motivation, and the direct equivalence is wrong). And actual definition of a regular order seems just as an auxiliary "such order that this very proof would work". The theorem is interesting, because regular orders include, as minimum, all the finite orders. But neither the intuition behind this class not it's size is obvious and it wasn't studied outside this article as far as I know. So I'll give the definition here and some examples at the end of the note.

**Definition.** Let $\mathbb{P} = (P, \leq)$ be a poset. It's called <u>sup-regular</u> if every chain $C$ in $\mathbb{P}$ has the [[Greatest Lower Bound and Least Upper Bound|least upper bound]] $\sup(C)$ and for any $p \in P$ we have $p < \sup(C)$ implies $\exists c \in C$ s.t. $c > p$

**Intuition.** The order doesn't "branch" down from such potential LUBs, that are not present in the chains for which they are the LUBs.

**Definition.** Let $\mathbb{P} = (P, \leq)$ be a poset. Similarly, it's called <u>inf-regular</u> if every chain $C$ in $\mathbb{P}$ has the [[Greatest Lower Bound and Least Upper Bound|greatest lower bound]] $\inf(C)$ and for any $p \in P$ we have $p > \inf(C)$ implies $\exists c \in C$ s.t. $c < p$.

**Definition.** [[Partial Order|Poset]] $\mathbb{P} = (P, \leq)$ is called <u>regular</u>, if it's both sup- and inf-regular.

**Statement.** Let $\mathbb{P} = (P, \leq)$ be a regular order (note: this includes all the finite orders). Than the following conditions are equivalent:
1. $\mathbb{P}$ is CAC
2. $\mathbb{P}$ is [[Proper N-Freeness|proper N-free]]
3. $\mathbb{P}$ is [[N'-Freeness|N'-free]]
$\blacktriangle$ (Th.5. from @grilletMaximalChainsAntichains1969)
$\boldsymbol{(1 \Longrightarrow 2)}$ (Note: this implication works in the case of an arbitrary poset, not just the regular one) Let $\{a,b,c,d\}$ be an [[N-Order|N-suborder]] in $\mathbb{P}$ with $a < b > c < d$. 
Consider some maximal antichain $A$ containing $\{a,d\}$ and some maximal chain $C$ containing $\{b, c\}.$By CAC $A \cap C = \{p\}$ for some $p \in P.$
Since $a \nsim c$ and $p$ lies in a chain, $p \neq a$; similarly $p \neq d$. Therefore $p \nsim a$ and $p \nsim d$, because $p$ lies in $A$ with $a$ and $d$. It follows by [[Transitivity|transitivity]] that both $p \leq c$ and $p \geq b$ are impossible, whence $c < p < n,$ which exactly means that $\{a,b,c,d\}$ is not a [[Proper N-Freeness|proper N-suborder]]. So there are no proper N-suborders because the N-suborder was arbitrary and every proper N-suborder is an N-suborder.
$\boldsymbol{(2 \Longrightarrow 3)}$ Follows from the fact every [[N'-Freeness|N'-suborder]] is a proper N-suborder.
$\boldsymbol{(3 \Longrightarrow 1)}$ Pretty much the same as my solution to the [[Removal of Maximal Chain in N-Free Poset Decreases Width]], just we use the regularity to find the exact moment the edges from $C$ to $A$ stop going up and start going down in the case of infinite order (while I just used the structure of a finite order), let's paraphrase it a bit differently here.
	**Notation.** Let $A^-$ be $\mathord{\downarrow} A \setminus A$, and $A^+$ be $\mathord{\uparrow} A \setminus A$.
	**Lemma 1.** Let $A$ be a maximal antichain in a poset $\mathbb{P} = (P, \leq)$, then $P = A^- \sqcup A \sqcup A^+$.
		$\color{red}\text{Proof}$ is a trivial exercise.
	**Lemma 2.** Let $\mathbb{P} = (P, \leq)$ be a regular poset, $C$ be a maximal chain in $\mathbb{P}$ and $A$ be a maximal antichain in $\mathbb{P}$ s.t. $A \cap C = \emptyset$. Then $C \cap A^-$ has a [[Minimal and Maximal Elements|maximal element]] $c$, $C \cap A^+$ has a [[Minimal and Maximal Elements|minimal element]] $b$ and $b$ [[Lower and Upper Covers, Adjacence|covers]] $c$, i.e. $b \succ c$.
		$\blacktriangle$ By lemma 1 and assumption we have $C \cap A^-$ and $C \cap A^+$ are disjoint and cover $C$.
		First $\inf C \in C$ and $\inf C$ is a minimal element of $\mathbb{P}$, since $C$ is maximal. Therefore $\inf C \notin A^+$ and, hence, $\inf C \in C \cap A^-$. Dually $C \cap A^+ \neq \varnothing$.
		Let $c := \sup (C \cap A^-)$. For any $x \in C$, either $y \leqslant x$ for all $y \in C \cap A^-$ and then $c \leqslant x$; or $x < y$ for some $y \in C \cap A^-$ and then $x < c$; in either case, $x$ and $c$ are comparable. Since $C$ is maximal, $c \in C$. Also, $c \in A^+$ would imply $a < c$ for some $a \in A$ and $a < x$ for some $x \in C \cap A^-$ (by sup-regularity), which is impossible. Therefore $c \in C \cap A^-$ and $c$ is maximum element of $C \cap A^-$.
		Dually $C \cap A^+$ has a minimum element $b$. Since $b \in A^+$, $c \in A^-$, one must have $c < b$. If $b$ does not cover $c$, $C$ is not maximal. This completes the proof of the lemma.
	To complete the proof of the theorem, we find, in the situation of the lemma 2 (i.e. $\lnot$CAC), $b \in A^+$ and $c \in A^-$ such that $c \prec b = b$ covers $c$. Since $b \in A^+$, $a < b$ for some $a \in A$; similarly $c < d$ for. some $d \in A$. Then $c < a$ contradicts $c \prec b$; $a \leqslant c$ contradicts $c \in A^-$; therefore $a \nsim c$. Dually $b \nsim d.$ Finally $a \neq d$ since $c < d$, so that $a \nsim d$. Therefore $(a, b, c, d)$ is an $N'$, which completes the proof.



**ON REGULARITY**
**Examples.**
1. Every finite poset is regular: for every chain $C$ its LUB and GLB exist and lie in $C$. 
2. $\mathbb{R}$ with a natural ordering is regular
3. $\mathbb{Q}$ with a natural ordering is not regular, for example $(-\infty, \sqrt{2}) \subseteq \mathbb{Q}$ has no LUB
4. $\mathbb{N}$ with a natural ordering is not regular, but $\mathbb{N} + \infty$ is regular
5. Consider $\mathbb{N}$ with a natural ordering + $\infty$ + an element $p$ s.t. $p$ is incomparable with all the natural numbers and $p < \infty$. It's not regular because for $\mathbb{N}$ the LUB is $\infty$, but it does have a $p$ s.t. $p < \infty$ and $\nexists c \in \mathbb{N}\ p < c$.

TODO draw example 5

**Examples.**
1. $\mathbb{N}$ with a natural ordering is inf-regular, but not sup-regular
2. $\mathbb{Q}$ with a natural ordering is neither inf- nor sup-regular
3. Every [[Well-Founded Order|well-founded poset]] is inf-regular

**Statement.** Being inf-regular and being sup-regular are [[Dual Properties|dual properties]].
$\color{red}\text{Proof}$ is a trivial exercise.

**Statement.** Being regular is [[Self-dual Properties|self-dual]].
$\color{red}\text{Proof}$ is a trivial exercise.

**Remark.** Author in @grilletMaximalChainsAntichains1969 says that regularity means that the LUBs and GLBs exist and lie in the closure of a chain in interval topology, but this is in fact wrong, for example consider example 5.
TODO Interval topology