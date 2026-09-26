---
tags:
  - Definition
  - Set-Theory
---
**Definition** **(Axiom of Choice).**
For any set $X$ of nonempty sets, there exist a function $f$ that is defined on $X$ and maps each set of $X$ to an element of that set (choice function):
$$\forall X \, (\emptyset \notin X \lor \exists f \, (\text{dom } f = X \land \forall A \in X \, (f(A) \in A)))$$

**Notation.** For brevity we would denote Axiom of Choice as <u>AC</u>.

**Intuition.** AC is considered a controversial axiom, it sounds "obviously" right, but creates plentiful of unintuitive results. To make things worse, [[Finite Axiom of Choice|finite version of AC]] (case when X is a finite set) is a theorem in ZF. So all the new statements AC is giving are about infinite sets, which makes difficult to decide what is intuitive and what is not, because human intuition is an evolutionary mechanism for understanding real world, which is essentially finite.
The reason for the unintuitiveness of AC consequences is that the axiom doesn't specify the form of a function $f$, unlike in ZF, where the functions in Axiom Schema of Replacement and predicate functions in Axiom Schema of Specification have a certain well-defined form "described" by a first order formula, which in case means it's constructive. In case of AC we get a function, but may have no idea how it look, we just know a one property – it is a choice function.

**Examples of unintuitive results.**
1. [[Infinite Line of Wizards]]
2. [[Unmeasurable Set on Circle]]

**Example of an intuitive result.**
[[Countable Union of Countable Sets]]

