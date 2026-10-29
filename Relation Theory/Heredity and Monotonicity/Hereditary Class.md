---
tags:
  - Definition
  - Relation-Theory
---
**Definition.** Let $\mathcal{C}$ be a class of [[Relation and Relational Structure|relational structures]] of the fixed [[Relation and Relational Structure|signature]], it's called <u>hereditary</u> if every [[Induced Substructure|induced substructure]] of any member of $\mathcal{C}$ belongs to $\mathcal{C}$.

**Definition.** Let $\mathcal{A}$ be some class of relational structures of the fixed signature, called it an <u>ambient class</u>. Then a class of relational structures $\mathcal{C} \subseteq \mathcal{A}$ is called <u>hereditary relative to </u>$\mathcal{A}$ if every induced substructure of any member of $\mathcal{C}$ belongs to $\mathcal{C}$ if it belongs to $\mathcal{A}$.

**Remark.** A <u>class of relational structures</u> is a set-theoretic class whose members are relational structures. So it can be a set and can be a proper class, hence we should be cautious not to do something impossible in ZFC, like, for example, take set of all relations (unless we restrict the [[Relation and Relational Structure|domain]]).

**Examples.** 
1. A class of all relational structures with binary [[Symmetry|symmetric]] relation is hereditary
2. A class of all relational structures with binary [[Antisymmetry|antisymmetric]] relation is hereditary
3. A class of all relational structures with binary [[Reflexivity|reflexive]] relation is hereditary
4. A class of all relational structures with binary [[Irreflexivity|irreflexive]] relation is hereditary
5. A class of all relational structures with binary [[Transitivity|transitive]] relation is hereditary
6. A class of all [[Graph|graphs]] is hereditary
7. A class of all [[Poset|partial orders]] is hereditary
8. A class of all [[Poset|strict partial orders]] is not monotone: we may break transitivity
9. A class of all [[Preorder|preorders]] is hereditary
10. A class of all [[Directed Graph|digraphs]] is hereditary
11. A class of all connected graphs is not hereditary: the substructure may be disconnected. It's not hereditary even relative to the class of all graphs
12. A class of all forests is hereditary
13. A class of all trees is hereditary relative to the class of all connected graphs (but not hereditary in general)
14. Every [[Monotone Class|monotone]] class is hereditary, the converse may not be true, for example consider (1)
15. Every class [[Monotone Class|monotone relative to ]]$\mathcal{A}$ is hereditary relative to $\mathcal{A}$
16. A class of all [[Complete Graph (Clique)|complete graphs]] is hereditary relative to the class of all graphs
17. A class of all [[Linear Order (Chain)|linear orders]] is hereditary
18. A class of all orders with the [[Least and Greatest Elements|greatest element]] is not hereditary: we may remove the greatest element

**Statement.** If class $\mathcal{A}$ is hereditary, then for any class $\mathcal{C}$ we have: $\mathcal{C}$ is hereditary $\iff$ $C$ is hereditary relative to $\mathcal{A}$.
$\color{red}\text{Proof}$ is a simple exercise.
**Corollary.** It's sensible only to choose non-hereditary as an ambient class.


TODO Reference "graph connectivity"
TODO Reference "forest"
TODO Reference "tree"
TODO Intuition?