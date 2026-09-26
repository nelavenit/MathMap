---
tags:
  - Statement
---
**Statement.** Any set of [[Well-Ordered Set|wosets]] $\mathcal{W}$ has the [[Least and Greatest Elements|least element]] with relation "is [[Order Isomorphism|isomorphic]] to a [[Upset and Downset|downset]]".
$\blacktriangle$ Consider arbitrary $\mathbb{W} \in \mathcal{W}$, if its the least, then we are done, else $\exists \mathbb{V} \in \mathcal{W}$ s.t. $\exists D$ – downset of $\mathbb{W}$ s.t. $\mathbb{V} \cong D$. Also we know a [[Form of Arbitrary Downset of Woset]].
So consider $X = \{ w \in \mathbb{W} \mid \exists \mathbb{V} \in \mathcal{W} \text{ s.t. } \mathbb{V} \simeq [0, w) \}$, $X \subseteq W$ $\Rightarrow X$ has a least element $x$, then the least element of $\mathcal{W}$ is a woset corresponding to $x$, i.e. isomorphic to $[0,x)$.

**Intuition.** This property differs from being a [[Well-Founded Order|well-founded]] poset because class of WOSs is proper and this is a statement about arbitrary subset $\mathcal{W}$, not a subclass, which is a strictly weaker statement.