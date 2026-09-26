---
tags:
  - Statement
---
**Statement.** Let $\mathbb{P} = (P, \leq_P)$, $\mathbb{Q} = (Q, \leq_Q)$ be [[Partial Order|posets]], $D_P \subseteq P$ – [[Upset and Downset|downset]] of $\mathbb{P}$, $f: P \rightarrow Q$ – [[Order Isomorphism|isomorphism]] between $\mathbb{P}$ and $\mathbb{Q}$. Then $f(D_P)$ is a downset of $\mathbb{Q}$.
$\blacktriangle$ Let $u \in f(D_P)$, and $d \in Q$ s.t. $d < u$. Consider $f^{-1}(u)$ and $f^{-1}(d)$, $f$ is an [[Order-preserving map (Order Homomorphism)|order homomorphism]], so $f^{-1}(d) \leq f^{-1}(u)$. Also $u \in f(D_P)$, hence $f^{-1}(u) \in D_P$, $D_P$ is a downset so $f^{-1}(d)$ is also in $D_P$, consequently $d = f(f^{-1}(d)) \in f(D_P)$. This proves $f(D_P)$ is a downset, because $d$ was an arbitrary element. $\boxtimes$
