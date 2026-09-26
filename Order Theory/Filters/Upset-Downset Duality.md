---
tags:
  - Statement
---
Let ($P,\leq$) be an [[Partial Order|order]], then $D \subseteq P$ is a [[Upset and Downset|downset]] $\iff P \setminus D$ is an [[Upset and Downset|upset]].
▲
$(\Rightarrow)$ assume the opposite, i.e. that $\exists d \in P \setminus D$ and $u \in P$ s.t. $u \notin P \setminus D$ and $u \geq d$. But $u \notin P \setminus D \Rightarrow u \in D \Rightarrow$ contradiction $\begin{cases} d \notin D \\ d \leq u \\ u \in D \\ D - downset \end{cases}$
$(\Leftarrow)$ Same way