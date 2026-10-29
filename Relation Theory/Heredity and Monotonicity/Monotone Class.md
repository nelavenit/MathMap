---
tags:
  - Relation-Theory
  - Definition
---
**Definition.** Let $\mathcal{C}$ be a class of [[Relation and Relational Structure|relational structures]] of the fixed [[Relation and Relational Structure|signature]], it's called <u>monotone</u> if every [[Substructure|substructure]] of any member of $\mathcal{C}$ belongs to $\mathcal{C}$.

**Definition.** Let $\mathcal{A}$ be some class of relational structures of the fixed signature, called it an <u>ambient class</u>. Then a class of relational structures $\mathcal{C} \subseteq \mathcal{A}$ is called <u>monotone relative to </u>$\mathcal{A}$ if every substructure of any member of $\mathcal{C}$ belongs to $\mathcal{C}$ if it belongs to $\mathcal{A}$.

**Remark.** A <u>class of relational structures</u> is a set-theoretic class whose members are relational structures. So it can be a set and can be a proper class, hence we should be cautious not to do something impossible in ZFC, like, for example, take set of all relations (unless we restrict the [[Relation and Relational Structure|domain]]).

**Examples.** 
1. A class of all relational structures with binary [[Symmetry|symmetric]] relation is not monotone. For example consider $\neq$ on the two-element set $\{a, b\}$, it's symmetric. But $(\{a,b\}, (a,b))$ is its substructure, but not symmetric. Compare to this class being [[Hereditary Class|hereditary]]
2. A class of all relational structures with binary [[Antisymmetry|antisymmetric]] relation is monotone
3. A class of all relational structures with binary [[Reflexivity|reflexive]] relation is not monotone: we may remove any pair $(a,a)$
4. A class of all relational structures with binary [[Irreflexivity|irreflexive]] relation is monotone
5. A class of all relational structures with binary [[Transitivity|transitive]] relation is monotone
6. A class of all [[Graph|graphs]] is not monotone: we may break symmetry
7. A class of all [[Poset|partial orders]] is not monotone: we may break both reflexivity and transitivity
8. A class of all [[poset|strict orders]] is not monotone: we may break transitivity
9. A class of all [[Preorder|preorders]] is not monotone, we may break transitivity
10. A class of all [[Directed Graph|digraphs]] is monotone
11. A class of all connected graphs is not monotone: the substructure may be disconnected. It's not monotone even relative to the class of all graphs
12. A class of all forests is monotone relative to the class of all graphs (but not monotone in general)
13. A class of all trees is monotone relative to the class of all connected graphs (but not monotone even relative to the class of all graphs)
14. A class of all orders of the finite [[Height|height]] is monotone relative to the class of all orders
15. A class of all [[Linear Order (Chain)|linear orders]] is not monotone: we can make it into an [[Antichain|antichain]]

**Statement.** If class $\mathcal{A}$ is monotone, then for any class $\mathcal{C}$ we have: $\mathcal{C}$ is monotone $\iff$ $C$ is monotone relative to $\mathcal{A}$.
$\color{red}\text{Proof}$ is a simple exercise.
**Corollary.** It's sensible only to choose non-monotone as an ambient class.


TODO Reference "graph connectivity"
TODO Reference "forest"
TODO Reference "tree"
TODO Intuition?