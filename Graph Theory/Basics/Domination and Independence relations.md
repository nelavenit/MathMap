---
tags:
  - Graph-Theory
  - Statement
---
**Statement 1.** Let $\mathbb{G} = (G, E)$ be a [[Graph|graph]], $I \subseteq G$. Then $I$ is [[Independent Set|maximal independent set]] of $\mathbb{G} \iff I$ is an independent [[Dominating Set|dominating]] set of $\mathbb{G}$.
$\color{red}\text{Proof}$ is a simple exercise.

**Statement 2.** Let $\mathbb{G} = (G, E)$ be a graph, $I \subseteq G$. Then $I$ is a maximal independent set of $\mathbb{G} \implies I$ is a minimal dominating set of $\mathbb{G}$.
$\color{red}\text{Proof}$ is a simple exercise.

**Statement 3.** The converse of St.2 need not hold. A minimal dominating set may be dependent. For example consider: ![[Pasted image 20261013110802.png|329]]
Here $\{2, 3\}$ is a minimal dominating set, but it's not independent.

**Corollary 4.** Let $\mathbb{G} = (G, E)$ be a [[Graph|graph]], $I \subseteq G$. Then $I$ is a [[Independent Set|maximal independent set]] of $\mathbb{G} \iff I$ is a minimal independent [[Dominating Set|dominating]] set of $\mathbb{G}$.
$\color{red}\text{Proof}$ is to combine St.1 with St.2.