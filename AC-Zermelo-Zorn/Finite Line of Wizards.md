---
tags:
  - Statement
  - Intuition
  - Set-Theory
---
**Statement.** Consider a line of players $x_1, \ldots x_n$ with two properties:
1. Each player has a hat of a color: either blue or red
2. Player $x_k$ sees hat colors of players $x_{k+1}, x_{k+2} \ldots x_n$ and only them
There are no conditions on hat color assignment.
The goal of players is for each to determine the color of his hat. They can’t exchange data after hat colors are assigned, but before that they can cooperate in any way.
In this case there is no algorithm for players to win.
$\blacktriangle$ Decision of $x_n$ is based on no data about a hat whatsoever, so it's predetermined, so let's give him a hat of an inverse color. Choice of player $x_{n-1}$ is solely determined by a color assignment of $x_n$, so we may know it beforehand and give him the opposite color. This way we would get the coloring on which every player fails. This is intuitive: no info means no way to find out.

**Intuition.** But everything changes when we consider an [[Infinite Line of Wizards|infinite line of players]] and [[Axiom of Choice|AC]].

