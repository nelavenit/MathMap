---
tags:
  - Graph-Theory
  - Definition
---
**Definition.** Let $\mathbb{G} = (G, E)$ be a [[Graph|graph]], $R \subseteq G$. Then $R$ is called <u>irredundant</u> if a removal of any vertex from $R$ strictly reduces the neighborhood of $R$. In other words if $$\forall r \in R\quad N[r] \setminus N[R\setminus\{r\}] \neq \emptyset.$$