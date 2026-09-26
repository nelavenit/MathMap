---
tags:
  - Definition
---
**Definition.** Let $\mathbb{P} = (P, ≤_P)$, $\mathbb{Q}=(Q, ≤_Q)$ be [[Partial Order|orders]], then $f: P→Q$ is called <u>order-preserving function from</u> $\mathbb{P}$ <u>to</u> $\mathbb{Q}$ iff $∀p₁,p₂∈ P$ we have $p₁≤_P p₂$ implies $f(p₁)≤_Q f(p₂)$. 
We would more often use the name <u>order homomorphism  from</u> $\mathbb{P}$ <u>to</u> $\mathbb{Q}$. 
Homomorphism is the general mathematic term for a structure-preserving function, so if multiple structure types are used in the context we can't omit "order" for brevity. We'll omit it just when the only structures in the context are orders and [[Preorder|preorders]] to avoid ambiguity.

**Notation.** When the orders between which function is order-preserving are obvious from the context we will omit the "from $\mathbb{P}$ to $\mathbb{Q}$" for brevity.

**Notation.** The set of all homomorphisms from $\mathbb{P}$ to $\mathbb{Q}$ is denoted as $Hom(\mathbb{P},\mathbb{Q})$.

**Examples.** 
1. ![[Injective Non-Surjective Order Homomorphism Example.png|300]]
2. ![[Surjective Non-Injective Order Homomorphism Example.png|300]]
3. [[Generic Order Homomorphism]]

**Statement.** Being an order homomorphism is [[Self-dual Properties|self-dual]]:
$f: P \to Q$ is order-preserving from $\mathbb{P}$ to $\mathbb{Q}$ $\Longleftrightarrow$ $f: P \to Q$ is order-preserving from $\mathbb{P}^d$ to $\mathbb{Q}^d$.
$\color{red}\text{Proof}$ is a simple exercise.

**Remark.** In some sources order-preserving function is called <u>isotone map</u> (comes as the increasing variant of <u>monotone map</u>, as opposite to the <u>antitone map</u>, which is a decreasing one).
**Remark.** Using the name "homomorphism" will be more consistent with the [[Order Isomorphism|order isomorphism]] term than the "order preserving map" is.