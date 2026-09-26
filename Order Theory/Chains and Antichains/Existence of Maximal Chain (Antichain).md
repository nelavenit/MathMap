---
tags:
  - Statement
  - AC-used
---
**Statement.** Let $\mathbb{P}=(P,\leq)$ be a [[Partial Order|poset]], $C\subseteq P$ – [[Linear Order and Chain|chain]] ([[Antichain|antichain]]), then there exists $M\subseteq P$ s.t. $C\subseteq M$ and $M$ is a [[Maximal Chain|maximal chain]] ([[Maximal Antichain|maximal antichain]]).
$\blacktriangle$ Very similar to the proof of (Zorn's $\Rightarrow$ AC) (see [[Zorn's Lemma|here]]).
We'll prove for a chain, antichain case is exactly the same.
Let $Q$ be the set of all chains in $\mathbb{P}$ containing $C$. Consider $\mathbb{Q}:=(Q,\subseteq)$, let's show it satisfies the [[Zorn's Lemma|Zorn's lemma]] condition: if $\{q_i\}_{i \in I}$ is a chain in $\mathbb{Q}$ then $q:=\bigcup_{i \in I} q_i$ is 1) a chain in $\mathbb P$ and 2) contains $C$ $\implies q \in Q$ and $q$ is an [[Lower and Upper Bounds|upper bound]] for $\{q_i\}_{i \in I}$. Then, by applying Zorn's lemma to $\mathbb{Q}$, we get a [[Minimal and Maximal Elements|maximal element]] of $\mathbb{Q}$ – desired maximal chain. $\boxtimes$
