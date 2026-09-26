---
tags:
  - Finite
  - Statement
---
**Statement.** Let $\mathbb{C_n} = (C_n, \leq)$ be a $n$-[[Crown|crown]] and $f$ be a [[Fixed Point and Fixed-Point-Free|fixed-point-free]] [[Order Endomorphism|endomorphism]] of $\mathbb{C}_n$. Then $f$ is an [[Order Automorphism|automorphism]].
$\blacktriangle$ Assume toward contradiction $f$ is non-automorphic fixed-point-free endomorphism. Crown is a finite order so by [[Bijective Endomorphism of Finite Order]] we know $f$ is automorphism $\iff$ $f$ is a bijective endomorphism, so $f$ must be non-bijective, hence $f[C_n]\subsetneq C_n$. At the same time, $\mathbb{C}_n$ is connected, hence $f[C_n]$ is connected too. So the [[Subposet|subposet]] corresponding to $f[C_n]$ is a connected subposet of a crown, which is not a full crown $\implies$ $f[C_n]$ is a [[Fence|fence]].
Now let's work just as in the proof of [[Fence has FPP]]. Let's name elements of $C_n$ with $c_1, \ldots, c_n$ in a way that $c_n \not \in f[C_n]$. Now consider a function $g:\overline{1,\ldots,n} \rightarrow \overline{1,\ldots,n}$ such, that $$g(k_1) = k_2 \overset{\ \text{ def.}}{\iff} f(c_{k_1}) = c_{k_2}$$
By $f$ being an endomorphism and $f[C_n]$ being a fence, not having $c_n$ as an element, we have $|k_1 - k_2| \leq 1$ implies $|g(k_1) - g(k_2)| \leq 1$. On the other hand, by $f$ being FPF, we have $|k - g(k)| \geq 1$, which, by [[Finite Height FPF Endomorphism Criterion]], implies $|k - g(k)| \geq 2$ (note: the criterion is applicable because [[Height|height]] of the crown is 2 — finite).
Now consider the smallest natural $m$ s.t. $g(m) \leq m$. It will exist at least because $f(c_n) \neq c_n$. As $m$ is the smallest such, we have $g(m - 1) \geq m$. Hence $g(m-1) \geq m+1$ or else, again by [[Finite Height FPF Endomorphism Criterion]], $f$ is not FPF. On the other hand $|(m-1) - m| = 1$, hence, as shown before, $|g(m-1) - g(m)| \leq 1$ — contradiction. $\boxtimes$


**Statement.** Same would be wrong for the [[Crown Tower|crown towers]], see exercise 2 [[_Exercises/Crowns and Fences/Crown Tower Exercises|here]].







TODO Reference to Connected