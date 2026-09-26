---
tags:
  - Statement
---
**Statement.** Let $\mathbb{W}=(W,\leq_W)$, $\mathbb{V}=(V,\leq_V)$ be [[Well-Ordered Set|wosets]]. Then either $\mathbb{W}$ is [[Order Isomorphism|isomorphic]] to some [[Upset and Downset|downset]] of $\mathbb{V}$, or $\mathbb{V}$ is isomorphic to some downset of $\mathbb{W}$ (this includes $\mathbb{W} \simeq \mathbb{V}$, because $V$ is a downset of $\mathbb{V}$).
$\color{red}\text{Proof idea: }$
1. Let's define $f: W → V$ recursively for $w \in W$.
   Assign f(w) to be is the [[Least and Greatest Elements|least element]] of $\mathbb{V}$ that isn't present in $\{f(w') | w' < w\}$.
   This definition is not sensible only in the case $\{f(w') | w' < w \} = V$.
   We get f from this recursive rule by [[Transfinite Recursion Theorem]].
2. $f$ is a desired isomorphism:
	1. if $f$ is defined everywhere then $\mathbb{W} \simeq \mathbb{D}$, where $\mathbb{D}$ is a downset of $\mathbb{V}$,
	2. else $f$ is defined on  $\mathbb{D}$ – downset of $\mathbb{W}$ and $\mathbb{V} \simeq \mathbb{D}$.
