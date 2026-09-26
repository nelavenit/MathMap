---
tags:
  - Statement
  - Set-Theory
  - AC-used
---
**Statement.** If we accept [[Axiom of Choice|AC]], them a countable union of countable sets is countable.
$\blacktriangle$ What we do to show $C^k$ is countable when $C$ is countable is we do an induction on $k$ an every step we use bijections $f_{k-1}: \mathbb{N} \to C^{k-1}$ and $g: \mathbb{N} \to C$ and get $f_k: \mathbb{N} \to C^k$, but in case $\bigcup\limits_{i=1}^\infty C_i$ we have an infinite amount of bijections, and if we know only the fact they exist we have no way to address them all at once, not one by one. I.e. we want to get a sequence/set $\{g_i\}_{i=1}^\infty$, where $\forall i$ $g_i: \mathbb{N} \to C_i$ is a bijection. AC gives us this set, for example, this way: let $G_i$ be a set of all bijections between $C_i$ and $\mathbb{N}$. $G := \bigcup\limits_{i=1}^\infty \{G_i\}$ exists by the Axiom Schema of Replacement. Now we can consider a choice function for $G - f$. $C_i \xmapsto{\text{ZF}} G_i \xmapsto{f} g_i$ is a way to address any bijection we need, and most importantly $f$ is a way to address an infinite number of bijections at once to get the sought-for bijection between $\mathbb{N}$ and $C^\mathbb{N}$.

**Intuition.** This result (unlike, for example, [[Infinite Line of Wizards|this]]) seems to be intuitively right, because we can describe in natural language the exact way to enumerate all the elements: ![[Counting Countable Union of Countable Sets.png|200]]
But of course calling any property of an infinite set "intuitive" contains a certain amount of oversimplification and assumption of having some math "culture". The classical example of an idea of an infinity being counterintuitive is the [[Hilbert's Paradox of Grand Hotel]].

**Intuition.** ZF is strictly insufficient to prove this fact. For example, there is a Feferman-Levy model of ZF in which $\mathbb{R}$ is a countable union of countable sets.

**Remark.** In this case AC is actually excessive, the axiom of a countable choice would suffice.