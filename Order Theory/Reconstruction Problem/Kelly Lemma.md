---
tags:
  - Statement
---
**Statement (The Kelly Lemma).** Let $\mathbb{P} = (P, \leq_P)$ be a finite [[Partial Order|poset]] of at least 4 elements and let $\mathbb{Q} = (Q, \leq_Q)$ be a poset with $|Q| < |P|$. Then the number s($\mathbb{Q}$, $\mathbb{P}$) of [[Subposet|subposets]] of $\mathbb{P}$ that are [[Order Isomorphism|isomorphic]] to $\mathbb{Q}$ is [[Reconstructibility|reconstructible]].
$\blacktriangle$ Let $d_\mathbb{Q} := \sum\limits_C |\{\mathbb{S}\text{ – subposet of } C \mid \mathbb{S} \text{ is isomorphic to } \mathbb{Q}\}|$ where the sum runs over all [[Card|cards]] $C$ of $\mathbb{P}$, with multiplicity. A certain subset $S$ of $P$ is not present in a card iff one of its point is removed, which happens exactly $|S| = |Q|$ times $\implies$ $S$ is contained in exactly $|P| - |Q|$ cards $\implies$ $d_\mathbb{Q} = s(\mathbb{Q},\mathbb{P}) (|P| - |Q|)$ $\implies s(\mathbb{Q},\mathbb{P}) = \dfrac{d_\mathbb{Q}}{|P| - |Q|}$. $\boxtimes$
