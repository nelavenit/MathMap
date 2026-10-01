---
tags:
  - Statement
  - AC-used
---
**Intuition.** Let's try to decompose a [[Partial Order|poset]] into a number of [[Linear Order (Chain)|chains]]. We can't have less than [[Width|width]] of $\mathbb{P}$ chains because then two elements of an [[Antichain|antichain]] would lie in one chain. But can we always manage with exactly $w(\mathbb{P})$ chains?
The idea can be to remove the [[Maximal Chain|maximal chain]] to decrease the width by 1, but it works only sometimes. Consider the same poset, but with different maximal chains for removal:
![[Maximal Chains Removal Example.png|350]]

It appears that we can apply stronger restrictions to the chain, more than just being maximal, and always decrease $w(\mathbb{P})$ by 1 by removing the chosen chain. And the result would work even in the case of infinite poset. But the proof is non-constructive and requires the finite case as a subtask.

**Statement (Dilworth's chain decomposition theorem).** Let $\mathbb{P} = (P, \leq)$ be a poset of width $k$. Then $P$ is a union of $k$ chains: $\exists C_1, C_2, \ldots C_k \subseteq P$ – chains s.t. $P = \bigsqcup\limits_{i = 1}^k C_i$.
$\color{red}\text{Extra-short proof idea:}$
1. Finite case by induction on $|P|$ by dividing $P$ into $U$ an $L$ — parts upper and lower than some [[Maximal Antichain|maximal antichain]]
2. Infinite case by induction on $k$.
	1. We give a definition of "strongly $k$-dependent chain"
	2. By finite case we get there are some such chains
	3. By [[Zorn's Lemma|Zorn's lemma]] we get maximal such chain and decrease the width by removing it

$\color{red}\text{Full proof:}$ 
**Finite case:** $\boldsymbol{|P| < \infty}$**.** (Th.2.26. from @schroderOrderedSetsIntroduction2016)
Induction on $|P|$
Base: $|P|=1$ - obvious
Step: assume theorem is right or any $k$ and posets with size $< n$, consider $|P|=n$ and width$(\mathbb{P})=k.$ Let's address two cases:
1. There is an antichain $A=\{a_1, \ldots a_k\}$ where at least one element is not [[Minimal and Maximal Elements|maximal]] and at least one element is not [[Minimal and Maximal Elements|minimal]]. Then $L := \mathord{\downarrow}A = \bigcup_{i=1}^k \mathord{\downarrow} a_i$ and $U := \mathord{\uparrow}A = \bigcup_{i=1}^k \mathord{\uparrow} a_i$ both have width of $k$ (trivial exercise) and size $<n$ by the choice of $A$ (else if $L=P$, then $\nexists p > a_i \ \forall i \implies$ $a_i$ are all maximal) so induction assumption is applicable: $L=\bigsqcup_{i=1}^k L_i$ and $U=\bigsqcup_{i=1}^k U_i$ where $U_i, L_i$ are chains in $\mathbb{P}$. Then $\forall i$ $a_i$ is the [[Least and Greatest Elements|greatest element]] of some $L_{j_i}$ and is the [[Least and Greatest Elements|least element]] element of some $U_{l_i}$.
   Else $\left [ \begin{array}{l} a_i \in L_{j_i} \text{, but not minimal — contradicts } L \text{ and } A \text{ definitions} \\ a_i \notin L \text{ — contradict, the definition of } L \end{array} \right.$ 
   WLOG Let's say $a_i$ is the least of $U_i$ and the greatest of $L_i$. Then $\{L_i \cup U_i\}_{i=1}^k$ is the desired decomposition. They are trivially 1) chains 2) disjoint. Lets show they 3) cover whole $P$: assume $\exists p \in P$ s.t. $p \notin L_i \cup U_i \ \forall i \implies \forall i \ a_i \nleq p \ngeq a_i \implies \{a_i\}_{i=1}^k \cup \{p\}$ is an antichain of size $k+1$ — contradicts $w(\mathbb{P}) = k$.
2. Every antichain of size $k$ consists either of maximal elements or maximal elements, then let $C \subseteq P$ be a maximal chain in $P$. $C$ contains a maximal and a minimal element (else $C$ is not maximal), i.e. $C$ contains same $a_i \in A$ for every antichain $A$ of size $k$, because $\text{Min}(\mathbb{P})$ and $\text{Max}(\mathbb{P})$ are the only candidates for antichain with a size of $k$ $\implies$ $\text{w}(P \setminus C) = k - 1$ and also we have $|P \setminus C| < n$ $\implies$ induction assumption is applicable: $P \setminus C = \bigsqcup_{i=1}^{k-1} C_i$ $\implies$ $P = \left( \bigsqcup_{i=1}^{k-1} C_i \right) \sqcup C$. $\boxtimes$
**Infinite case.** (Original proof from @dilworthDecompositionTheoremPartially1948) 
	**Definition.** Set $C \subseteq P$ is called <u>strongly k-dependent</u> if for every finite $F \subseteq P$ there is a representation $F = K_1 \sqcup K_2 \sqcup \ldots \sqcup K_k$ as a union of exactly $k$ chains $K_i$ and $F \cap C \subseteq K_i$ for some $1 \leq i \leq k$.
	**Statement.** Strongly k-dependent set is a chain.
		$\blacktriangle$ If there are incomparable $c_1,c_2\in C$, then we can consider $F:=\{c_1,c_2\}$, $C\cap F = F$ — can't be contained in a chain because it is an antichain. $\boxtimes$
	~={lblue}Theorem proof idea: 
	1. Prove there exists a maximal strongly k-dependent chain $C_1$
	2. Prove $P \setminus C_1$ has a width $k-1$ 
	3. Induction on $k$ =~
	
   I. Induction on $k = w(\mathbb{P})$.
   Induction base: $k = 1 \implies \mathbb{P}$ is a chain, hence we have what we wanted.
   Step: assume for $w(\mathbb{P})<k$ we have a decomposition of $\mathbb{P}$ into $w(\mathbb{P})$ chains. Now consider $\mathbb{P}$ with width $k$.
   II. Let's show in $\mathbb{P}$ there exists a maximal strongly k-dependent chain $C_1$: for that we check the Zorn's lemma condition.
   Let $\mathbb{S} = (S, \subseteq)$ be a set of all str. k-dep. chains (= str. k-dep. sets) of $\mathbb{P}$ with set inclusion relation:
	   1. $S$ is non-empty: 
	      By the finite case of Dilworth's decomposition theorem every finite set $F$ can be represented as $K_1 \sqcup K_2 \sqcup \ldots \sqcup K_k$ (here some $K_i$ may be $\emptyset$, if $w_\mathbb{P}(F) < k$) $\implies$ every one-element set is strongly k-dependent, because a single-element set intersected with $F$ is at most single-element set $\implies$ lies in some single $K_i$.
	   2. Let $\{s_i\}_{i \in I}$ be a chain in $\mathbb{S}$, then $s := \bigcup_{i \in I} s_i$ is a str. k-dep. chain in $\mathbb{P}$:
	      Let $F \subseteq P$ be finite and $F = K_1 \sqcup K_2 \sqcup \ldots \sqcup K_k$, where every $K_i$ is a chain in $\mathbb{P}$.
	      We have $s \cap F$ is finite $\implies$ we can write it as $\{f_1, \dots, f_d\}$, $f_i \in s \implies \forall i \in 1..d$ $\exists j_i$ s.t. $f_i \in S_{j_i} \implies s \cap F \subseteq \bigcup_{i=1}^d S_{j_i} = S_{j_r}$ – $\subseteq$-maximal from $\{S_{j_i}\}$, $S_{j_r}$ is str. k-dep. $\implies$ $S_{j_r} \subseteq K_j \implies s \cup F \subseteq K_j \implies s \in S$ and $s$ is an [[Lower and Upper Bounds|upper bound]] of $\{S_i\}_{i \in I} \implies$ Zorn's lemma is applicable to $\mathbb{S} \implies \exists C_1$ – maximal str. k-dep. chain in $\mathbb{P}$.
   III. Prove $P \setminus C_1$ has a width of $k-1$: assume the opposite, i.e. there exists $\{a_1, \dots, a_k\}$ – antichain in $P \setminus C_1$.
	   Let $C_1$ be maximal strongly $k$-dependent set $\implies$ $\forall i \in 1 \ldots k$ $\{a_i\} \cup C_1$ — is not a str. k-dep. set $\implies$ $\forall i\ \exists F_i \subseteq P$ – finite, s.t. for every chain decomposition of $F_i$ there is no chain containing $F_i \cap (C_1 \cup \{a_i\})$.
	   Consider $F := \bigcup_{i=1}^{k} F_i$.
	   $F$ is finite $\implies$ $\exists\ K_1 \ldots K_k$ – chain decomposition of $F$ s.t. $F \cap C_1 \subseteq K_d \implies$ $\forall i\ F_i \cap C_1 \subseteq K_d$, but $\forall i\ F_i \cap (C_1 \cup \{a_{i}\}) \nsubseteq K_d$ (because $\forall i\ \{K_j \cap F_i\}_{j = 1}^{k}$ is a chain decomposition of $F_i$) $\implies \forall i \begin{cases} a_{i} \in F_i \\ a_{i} \notin K_d \end{cases}$, but every $K_j$ is a chain, so no $K_j$ can contain two elements of $\{a_i\}_{i=1}^k \implies \exists a_i \in K_d$ — contradiction $\implies$ there can't exist an antichain $\{a_i\}_{i=1}^k$ $\implies$ $w_\mathbb{P}( P \setminus C_1) < k \implies$ induction assumption is applicable $\implies P \setminus C_1 = \bigsqcup_{i=2}^k C_i \implies$ $P = \bigsqcup_{i=1}^k C_i$ is the desired chain decomposition. $\boxtimes$

**Further reading.** It's interesting to investigate into when exactly is taking any maximal chain is not enough to decrease the width of an order, and when it is enough. See [[Removal of Maximal Chain Decreases Width Criteria]].