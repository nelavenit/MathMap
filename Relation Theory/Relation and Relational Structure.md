---
tags:
  - Relation-Theory
  - Definition
---
**Definition.** Let $A_1,\ldots,A_n$ be sets, where $n\geq1$. A subset $R\subseteq A_1\times\cdots\times A_n$ is called an $n$-<u>ary relation</u> between_ $A_1,\ldots,A_n$. If $A_1=\cdots=A_n=A$, it is called an $n$<u>-ary relation</u> on $A$. 

**Definition.** Let $R$ be a $2$-ary relation, then it is called a <u>binary relation</u> and $(a_1, a_2) \in R$ is denoted by $a_1 \mathrel{R} a_2$. 

**Definition.** Let $R$ be a $1$-ary relation on $A$, then it is called a <u>unary relation</u>.

**Definition.** Let $R$ be an $n$-ary relation, then $n$ is called the <u>arity of </u>$R$. 

**Definition.** Let $A$ be a set and $(R_i)_{i\in I}$ be an indexed family of relations on $A$, where $R_i$ has arity $n_i$ (i.e. $R_i\subseteq A^{n_i}$). A pair $\mathbb A=\bigl(A,(R_i)_{i\in I}\bigr)$ is called a <u>relational structure</u>.
The set $A$ is called its <u>underlying set</u> or <u>domain</u>.

**Notation.** If the family consists of a single relation $R$, we write $\mathbb{A} = (A, R)$, omitting the one-element tuple notation.

**Examples.**
1. [[Preorder]] is a relational structure, with a [[Preorder|preordering]] being a binary relation
2. [[Partial Order|Poset]] is a relational structure, with an [[Partial Order|ordering]] being a binary relation
3. [[Graph]] is a relational structure, with an [[Graph|adjacency]] being a binary relation on the [[Graph|vertex set]]
4. [[Directed Graph]] is a relational structure, with a [[Directed Graph|directed adjacency]] being a binary relation
5. For any family of sets $\mathcal{A}$ the pair $(\mathcal{A}, {\subseteq}\big|_{\mathcal A\times\mathcal A})$ is a relational structure, with ${\subseteq}\big|_{\mathcal A\times\mathcal A}$ being a binary relation on $\mathcal{A}$
6. For any family of sets $\mathcal{A}$ the pair $(\mathcal{A}, {\subsetneq}\big|_{\mathcal A\times\mathcal A})$ is a relational structure, with ${\subsetneq}\big|_{\mathcal A\times\mathcal A}$ being a binary relation on $\mathcal{A}$
7. In set theory we have for any family of sets $\mathcal{A}$ the pair $(\mathcal{A}, {\in}\big|_{\mathcal A\times\mathcal A})$ being a relational structure, with ${\in}\big|_{\mathcal A\times\mathcal A}$ being a binary relation
8. Even numbers $E:=\{n \in \mathbb{Z} \text{ s.t. } 2 \mid n\}$ is a unary relation on $\mathbb{Z}$ 


Maybe TODO semantic difference from binary predicate