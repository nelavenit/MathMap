---
tags:
  - Statement
---
**Statement.** Let $\mathbb{P} = (P, \leq_P)$ and $\mathbb{Q} = (Q, \leq_Q)$ be [[Partial Order|posets]], $\mathbb{P}$ be [[Connectivity|connected]] and $f: P \to Q$ be an [[Order-preserving map (Order Homomorphism)|order homomorphism]]. Then $f[P]$ is connected too.
$\blacktriangle$ Consider any $q_1, q_2 \in f[P]$. They are images of some $p_1, p_2 \in P$. $\mathbb{P}$ is connected, so there is a [[Fence|fence]] $(F, \leq_P|_{F\times F})$ with $p_1$ and $p_2$ as [[Fence|endpoints]]. Then, by $f$ being order-preserving, $f[F]$ is a fence in $\mathbb{Q}$ with $f(p_1) = q_1$ and $f(p_2) = q_2$ as endpoints. Hence $f[P]$ is connected. $\boxtimes$
(here proving $f[F]$ is a fence is omitted as a simple exercise) 