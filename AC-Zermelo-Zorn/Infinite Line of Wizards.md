---
tags:
  - Statement
  - Intuition
  - Set-Theory
  - AC-used
---
**Statement (Infinite case of [[Finite Line of Wizards|line of wizards]]).** Consider a countable line of players $x_1, x_2, x_3, \ldots$ and 
1. Every player has a hat of a color: either blue or red
2. Every player sees all the players with a number higher than his and only them
3. Every player knows his number in line 
There are no conditions on hat color assignment.
Then, if we accept [[Axiom of Choice|AC]], there is a way for players to act so all but a finite number of them guess the color of their hat no matter the coloring. 
$\blacktriangle$ Let's call the sequence $\{c_i\}_{i=1}^\infty$ with $c_i \in \{0,1\}$ a <u>coloring</u>. 
Assume the relation $\sim$ on a set of all colorings: $C_1 \sim C_2$  $\overset{def.}{\iff} C_1$ and $C_2$ differ only on finite number of positions. Proving $∼$ is an equivalence relation is a simple exercise. 
Let's consider the quotient set of all colorings by $∼$. The algorithm of players would be: before the color assignment they choose a canonical representative of each equivalence class, this is possible, because by AC there exists a choice function for the quotient set. Now the player $k$ sees $c_{k+1}, c_{k+2}, \ldots$ With this knowledge he unambiguously determines the equivalence class of the whole coloring because a $c_1,\ldots, c_k, c_{k+1}, c_{k+2}$ is equivalent to the true coloring.
Then he makes a guess that his color is a $k^{\text{th}}$ color of a canonical coloring of this class. By the definition of $∼$ the guesses of players can differ from the right answer only in a finite number of positions. $\boxtimes$

**Intuition.** So having no data about his own hat color doesn't stop a player to guess "almost always". To many it seems unintuitive, but the thing is it is a fact about something impossible in real life: an infinite line of people; so the human intuition isn't "designed" to evaluate such cases.
Moreover, the AC doesn't guarantee the choice function f can be described in any nice way (even worse: the whole power of AC is that it often gives a function indescribable in ZF, i.e. unconstructible). So we assume players can share an object indescribable in any known language, which is also impossible in real life, so intuition doesn't consider it.

**Intuition.** One way to look at this statement is "having an infinite amount of data is huge, in order to brake the way players behave it's insufficient to change the finite amount of colors and changing an infinite amount of colors always gives the players enough info to change a decision.

**Statement (Wizard line with even fewer info).** We can get the same result even in the case the players don't know their numbers in line, but the proof is longer.
$\color{red}\text{Proof idea:}$
1. Consider ∼ relation : $\{a_i\}_{i=1}^\infty ∼ \{b_i\}_{i=1}^\infty \overset{def.}{\iff}  ∃ n,m \in \mathbb{N}$ s.t. $\forall i\ a_{n+i} = b_{m+i}$, i.e. the colorings have the same tail
2. While determining in which equivalence class our coloring lies we will have to address two cases:
	1. Visible colors sequence is periodic
	2. Visible colors sequence is non-periodic
   because we don't know our offset from the start of the line.