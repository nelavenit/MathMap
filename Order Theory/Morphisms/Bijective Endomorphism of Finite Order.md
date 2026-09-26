---
tags:
  - Statement
---
**Statement.** Let $\mathbb{P} = (P, \leq)$ be *finite* [[Partial Order|order]], then any bijective [[Order Endomorphism|endomorphism]] of $\mathbb{P}$, call it $f$, is an [[Order Automorphism|automorphism]].
$\blacktriangle$ By assumption $f$ is a permutation of $P$ so $(f(\cdot),f(\cdot))$ is a permutation of $P \times P$. The fact $f$ is an endomorphism is exactly:
$$(f(\cdot),f(\cdot))[\leq]\ \ \subseteq\ \ \leq$$
For $f$ to be an automorphism we lack only $f^{-1}$ to be an endomorphism, i.e. to:
$$(f^{-1}(\cdot),f^{-1}(\cdot))[\leq]\ \ \subseteq\ \ \leq$$
The $(f,f)$ is a bijection and every element of $\leq$ is mapped into $\leq$, so, because $P$ is finite, $(f^{-1},f^{-1})$ maps the whole $\leq$ into $\leq$ too as a one-to-one correspondence of the finite sets. $\boxtimes$
 
**Intuition.** We can paraphrase the statement as "every non-automorphic endomorphism on a finite set is both non-injective and non-surjective", because for a finite order both injective endomorphism and surjective endomorphism are bijective.

**Statement.** It wouldn't work in the infinite case.
$\blacktriangle$ Consider $\mathbb{N}$ with a natural ordering, and let's add a countable "pool" of incomparable elements $\mathbb{N}'$. Define: $$f(n)=
\begin{cases}
n+1, n \in \mathbb{N} \\
 1 , n = 1' \in \mathbb{N}' \\
n-1, n \in \mathbb{N}'
\end{cases}$$
![[Bijective Non-automorphic Endomorphism.png|300]]
Proof that $f$ is a bijective endomorphism is a trivial exercise.
But $f^{-1}$ is not an endomorphism because $1≤2$ , but $f^{-1}(1)=1' \nleq 1 = f^{-1}(2)$.
In the terms of the proof we have $(2,1) \in \leq$ but $(f^{-1}(2),f^{-1}(1)) = (1,1') \not \in \leq$, because an injectivity doesn't cause bijectivity for the infinite sets.


**Sources.** My solution to Exercise 1-22 from @schroderOrderedSetsIntroduction2016.