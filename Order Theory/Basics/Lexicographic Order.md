---
tags:
  - Definition
---
**Definition.** Let $\mathbb{P} = (P, \leq_P)$ and $\mathbb{Q} = (Q, \leq_Q)$ be [[Partial Order|posets]]. Then <u>lexicographic order</u> (denoted as $\mathbb{P} \times \mathbb{Q}$) is $P \times Q$ with such $\leq$, that:
$$(p_1, q_1) \leq (p_2, q_2) \overset{\text{def}}{\Leftrightarrow} \left[ \begin{array}{ll} p_1 <_P p_2 \\ \begin{cases} p_1 = p_2 \\ q_1 \leq_Q q_2 \end{cases} \end{array} \right .$$
**Statement.** Let $\mathbb{P} = (P, \leq_P)$ and $\mathbb{Q} = (Q, \leq_Q)$ be posets, then $\mathbb{P} \times \mathbb{Q}$ is a poset.
$\color{red}\text{Proof}$ is a simple exercise.

**Definition.** Inductively we define lexicographic order for any finite number of posets:
on $\mathbb{P}_1 \times \mathbb{P}_2 \times \ldots \times \mathbb{P}_k$ =  $(\mathbb{P}_1 \times \mathbb{P}_2 \times \ldots \times \mathbb{P}_{k-1}) \times \mathbb{P}_k$.
