---
tags:
  - Statement
  - Finite
---
**Intuition.** In *finite* [[Partial Order|orders]] every [[Upset and Downset|downset]] in uniquely defined by the set of its [[Minimal and Maximal Elements|maximal elements]]. At the same time, for any [[Subposet|subposet]] the set of maximal elements is an [[Antichain|antichain]]. So comes the following relation between antichains and downsets.

**Statement.** Let $\mathbb{P} = (P, \leq)$ be a *finite* order. Then the number of antichains in $\mathbb{P}$ is equal to the number of downsets in $\mathbb{P}$.
$\blacktriangle$ Define $\mathcal{D}(\mathbb{P})$ be a set of all the downsets of $\mathbb{P}$ and $\mathcal{A}(\mathbb{P})$ be a set of all antichains in $\mathbb{P}$. Let's show, that $F: \mathcal{A}(\mathbb{P}) \rightarrow \mathcal{D}(\mathbb{P})$ s.t. $F: A \mapsto \mathord{\downarrow}A$ is a bijection with $F^{-1}(D) \equiv \max(D)$:
1. Correctness: assume $A \subseteq P$ is an antichain, then $\mathord{\downarrow} A$ [[Upset and Downset|is]] a downset
2. Injectivity: assume $A_1, A_2 \in \mathcal{A}(\mathbb{P})$ and $A_1 \neq A_2$. If $A_1 \subseteq \mathord{\downarrow} A_2$, then $A_2 \setminus A_1 \subseteq F(A_2)$ and $A_2 \setminus A_1 \not\subseteq F(A_1)$. Else consider $a \in A_1 \setminus \mathord{\downarrow}A_2$. We would have both $a \in F(A_1)$ and $a \not\in F(A_2)$ 
3. Surjectivity: consider arbitrary $D \in \mathcal{D}(\mathbb{P})$, $\max(D)$ is an antichain, else at least one of the elements wouldn't be maximal (note: there is also the case of $D = \emptyset$, in which $\max(D) = \emptyset$ is an antichain as desired). And $D = \mathord{\downarrow}\max(D)$ by the $D$ being a downset.

**Intuition.** The same $F$ may not be bijective in the case of an infinite order. For instance, consider $\mathbb{N}$ with the natural ordering.