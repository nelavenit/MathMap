---
tags:
  - Exercise
---
The following is simpler version of [[Removal of Maximal Chain Decreases Width Criteria]], [[N-Freeness|N-free]] instead of proper N-free, hence one-way implication instead of a criteria, and finite order instead of a regular one (which along with simplification does the opposite by also not giving a hint on how to approach the problem).

**Exercise.** (2-17a from @schroderOrderedSetsIntroduction2016) Proof that if the finite [[Partial Order|order]] is N-free, then removal of any [[Maximal Chain|maximal chain]] will decrease the [[Width|width]]. (Solved it myself)
**Statement.** Let $\mathbb{P} = (P, \leq)$ be finite N-free poset, then removal of any maximal chain strictly decreases the width of $\mathbb{P}$.
$\blacktriangle$ (my own proof) Show by contraposition.
Assume $C$ is a maximal chain in $\mathbb{P} = (P, \leq)$, P is finite and $w(P) = w(P \setminus C) := w$. We want to find [[N-Order|N-order]] in $\mathbb{P}$.
Let $A$ be an [[Antichain|antichain]] in $(P \setminus C, \leq|_{P\setminus C \times P\setminus C})$ of the size $w$, $w(P) = w$ $\implies$ $\forall c \in C$ $\exists a \in A$ s.t. $a \sim c$.
1. If $|C| = 1$ then $C$ is an isolated point $\implies$ removal decreases the width
2. $|C| > 1 \implies \exists \max(C) \neq \min (C)$, then $\exists a_1 \in A$ s.t. $a \sim \max(C)$. $a_1 \ngeq \max(C)$ because else $C \cup \lbrace a_1 \rbrace$ is a chain — contradicts maximality of $C$ $\implies$ $a_1 < max(C)$
3. Same way we get $a_2 > min(C)$
4. ![[N-Free Poset Maximal Chain Removal 01.png|300]]
   We can't have ![[N-Free Poset Maximal Chain Removal 02.png|150]] for any $a', a \in A$, because then $a' \sim a$
5. Now combine 2,3 and 4: for some $j \in \overline{0 \ldots k-1}$  $\begin{cases} c_j < a \text{ for some } a \in A. \\ c_{j+1} > a' \text{for some} a' \in A \\ c_j \prec c_{j+1} \end{cases}$
   The picture is ![[N-Free Poset Maximal Chain Removal 03.png|150]], i.e. $(c_j, c_{j+1})$ is the moment edges going from $C$ to $A$ stop going up and start going down. $\{a', a, c_{j+1}, c_j\}$ is the sought-for N-order, unless
	1. $a' = a$ — contradicts maximality of $C$, because then $C \cup \{a\}$ would be a chain
	2. $a \sim c_{j+1}$ : 
		1. If $c_{j+1} > a$, then contradicts chain maximality
		2. If $c_{j+1} < \alpha$, then $a > a'$ — contradicts choice of $A$
	3. $a' \sim c_{j}$ 
		1. $a' > c_{j}$ — contradicts maximality of $C$
		2. $a' < c_{j}$, then $a > a'$ — contradiction $\boxtimes$


**Exercise.** (2-17b from @schroderOrderedSetsIntroduction2016) Prove the inverse is wrong. (Solved it myself)
**Statement.** The inverse is wrong: there exists a finite poset for which removal of any maximal chain decreases the width, but a poset has an N-order [[Subposet|subposet]].
$\blacktriangle$ ![[Chain Removal Decreases Width Reverse Counterexample.png|200]]
Drawn poset in not N-free, $w(P) = 4$, but for any maximal chain $C$, $w(p \setminus C) = 3$. 