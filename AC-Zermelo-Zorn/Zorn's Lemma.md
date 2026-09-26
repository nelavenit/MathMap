---
tags:
  - Statement
  - AC-used
---
**Intuition.** Another way to see [[Axiom of Choice|AC]] is an order-theoretic statement called Zorn's lemma. On one hand, it is used in different branches of math just as a reformulation of AC to make some proves shorter and easier, than while using [[Zermelo's Theorem|Zermelo's theorem]] and transfinite induction directly. On the other hand, in order theory it's a stand-alone theorem (when assuming AC of course).

**Statement (Zorn's lemma).** Let $\mathbb{P} = (P, \leq)$ be a non-empty [[Partial Order|poset]] in which every [[Linear Order and Chain|chain]] has an [[Lower and Upper Bounds|upper bound]], then there is a [[Minimal and Maximal Elements|maximal element]] in $\mathbb{P}$. And even more: $\forall p \in P\ \exists m \in Max(\mathbb{P})$ s.t. $m \geq p$.
This statement is equivalent to AC and Zermelo's theorem.
$\blacktriangle$ (Th.30 from @vereshchaginNachalaTeoriiMnozhestv2012)
**(WO $\boldsymbol{\Rightarrow}$ Zorn)** Let $\mathbb{P} = (P, ≤)$ be a poset in which every chain has an upper bound. We want to prove that for every $p ∈ P\  ∃ m ∈ Max(\mathbb{P})$ s.t. $m ≥ p$.
Consider $\mathbb{I} = (I, \leq_I)$  – [[Well-Ordered Set|woset]] with cardinality strictly greater than the one of P. For example we may take power set of P which has a strictly greater cardinality and well-order it by Zermelo's theorem.
Intuition:
	$\mathbb{I}$ stands for index, because we will use it as a way to index elements of P to perform a transfinite induction/recursion.
	Note that having a well-ordered set of a greater cardinality for any set P requires Zermelo's theorem, it's impossible in ZF.
Let's define recursively a [[Strict Order Homomorphism|strict homomorphism]] $f: I → P$
1. $f(Min(\mathbb{I})) = p$
2. Assume $f$ is defined for all $j ≤_I i$ and is a strict homomorphism (i.e. $a <_I b$ implies $f(a) < f(b)$. $[0, i)$ is a chain in $\mathbb{I} \implies f([0, i))$ is a chain in $\mathbb{P}$ $\implies$ by lemma assumption $∃$ upper bound $g$ of $f([0, i))$, and among other $g ≥ p$. If $g$ is a maximal element then we are done, else $\exists g' \in P \ \text{s.t.} \ g' > g$, let  $f(i) := g'$. Function $f$ still would be a strict homomorphism.
3. This way by a [[Transfinite Recursion Theorem]] we would define $f$ on the whole $I$. And $f$ would be injective because it's a strict homomorphism — contradicts the fact the cardinality of $I$ is strictly greater than of $P$ — this means at some point $\not\exists g'$ — exactly what we needed.
In this argument, strictly speaking, there is a gap: we simultaneously define a function by transfinite recursion and prove its monotonicity by means of transfinite induction. Our recursive definition makes sense only if the already constructed part of the function is monotone. Formally speaking, one should use [[Transfinite Recursion Theorem|transfinite recursion for a partially defined function]], stipulating that the next value is undefined if the already constructed segment is not monotone, and thus obtain a function defined either on all of $I$ or on an [[Form of Arbitrary Downset of Woset|initial segment]] of $I$. If it is defined on some initial segment, then it is monotone on that segment by construction, and therefore the next value is also defined — a contradiction.

**(Zorn $\boldsymbol{\Rightarrow}$ AC)** Let $X$ be a set we want to get the choice function $f: X \to \bigcup\limits_{x \in X} x$ for. Consider the set $F$ of all the function $f: D \to \bigcup\limits_{x \in X} x$ s.t. $D \subseteq X$ and for all $n \in D$ $f(n) \in n$. This set is not empty because for any finite $D \subseteq X$ such function exists by [[Finite Axiom of Choice]]. (This is the key idea)
Now consider poset $\mathbb{F} = (F, \leq) := (F, \subseteq)$, i.e. $f \leq g \overset{def.}{\iff} f = g|_{\text{dom}(f)}$. Now show that every chain in $\mathbb{F}$ has an upper bound: let $C \subseteq F$ be a chain, then $f := \bigcup\limits_{g \in C} g$ is an element of $F$ an is $\geq$ then every element of $C$:
1. $f$ is well-defined on every $x \in \bigcup\limits_{g\in C} dom(g)$ because C is a chain
2. f is a choice function: $\forall x \in \bigcup\limits_{g\in C} dom(g)$ we have $f(x) =$ \[for some $g \in C$\] $= g(x) \in x$
3. $\bigcup\limits_{g\in C} dom(g) \subseteq X$
4. $f$ is an upper bound: $∀g ∈ C\ g \subseteq f$ by definition of $f$ $\implies g ≤ f$
Then $\mathbb{F}$ satisfies the Zorn's lemma condition $\implies$ $\exists m \in Max(\mathbb{F})$.
Assume $m$ is not defined on some $x \in X$, then $x \neq \emptyset \implies$ $\exists y \in x \implies$ $m \cup \{(x,y)\}$ is an element of $F$ that is strictly greater then $m$ — contradicts the choice of $m$ $\implies$ $m$ is the desired choice function. $\boxtimes$

**Alternative proof of (WO $\boldsymbol{\Rightarrow}$ Zorn).** (Comment after Th.30 from @vereshchaginNachalaTeoriiMnozhestv2012)
Let $\mathbb{P} = (P, ≤)$ be a poset in which every chain has an upper bound. We want to prove that for every $p ∈ P\ ∃ m ∈ Max(\mathbb{P})$ s.t. $m ≥ p$.
1. Let's well-order $P$, this would be an order having no relation to $≤$, we'll denote it $\preccurlyeq$  
2. Using transfinite recursion we want to build a function $f$ with the following properties:  
	2.0. $f : P \rightarrow P$
	2.1. $\forall q \in P\ f(q) \geq p$
	2.2. $f$ is monotonous but in unusual way: $x \preccurlyeq y$ implies $f(x) \leq f(y)$, in other words $f$ is a [[Order-preserving map (Order Homomorphism)|homomorphism]] from $(P, \preccurlyeq)$ to $(P, \leq)$
	2.3. $\forall q \in P \ f(q) \nless q$
3. If we have such $f$ then:
	$Im_f(P)$ is a $\leq$-chain due to (2.2) property $\implies$ by lemma assumption it has an upper bound $\beta$, which is $\geq p$ (by 2.1). If $\beta$ is $<$ than some $m \in P$ then $f(m) \leq \beta < m$ — contradicts (2.3)$\implies$$\beta$ is a maximal element.
4. The only thing left is to build f:
	4.1. If $p_0$ is a [[Least and Greatest Elements|least element]] of $(P, \preccurlyeq)$, then $f(p_0) := \max_{\leq}(p_0, p)$, a.k.a. keep (2.1) and (2.3)
	4.2. If $f$ is defined for all $q' \prec q$, then $f(q) := \max_{\leq}(\text{upper bound}_{\leq}(\text{Im}_f([0, q))), q)$
	4.3. Check the properties
		2.0. Obvious  
		2.1. If $\exists q$ $f(q)<p$, then $\max_\leq (\text{upper bound}_\leq(\text{Im}_f([0,q))),q)<p$ — contradicts $p \leq f(p_0)$, because $f(p_0) \in Im_f([0,q))$  
		2.2. If $x\preccurlyeq y$ then $f(y)\geq \text{upper bound}_\leq(\text{Im}_f([0,y))) \geq f(x)$, because $f(x) \in Im_f([0,y))$
		2.3. Obvious $\boxtimes$
**Intuition.** This is actually somewhat similar to the first proof, in the both approaches we build a monotonous function from a well-ordered set to the our $\mathbb{P}$. But there's a difference:

| First proof                                                                      | Alternative proof                                                                        |
| -------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------- |
| Needs a set of a greater cardinality, which may be harder to comprehend for some | Working with two order relations on the some set simultaniously is a harder thing for me |
| We need to assume $\neg$Zorn's on every step of recursive $f$ building           | Assuming $\neg$Zorn's is used only once                                                  |
