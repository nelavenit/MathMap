---
tags:
  - Statement
  - Finite
---
**Statement.** [[Crown|Crowns]] are [[Reconstructibility|reconstructible]].
$\blacktriangle$ It suffices to prove:
$\mathbb{P}$ is a crown $\iff$ every [[Card]] of $\mathbb{P}$ is a [[Fence|fence]] with both [[Fence|endpoints]] being either the top ones or the bottom ones
$\boldsymbol{(\Longrightarrow)}$ A simple exercise
$\boldsymbol{(\Longleftarrow)}$ Assume the opposite: there is a card of $\mathbb{P}$ s.t. it is a fence with both endpoint being the bottom ones (WLOG, cause the case of the top ones is done the same way), but the $\mathbb{P}$ is not a crown. The removed vertex is $r$:
![[Crown is Reconstructible Proof Illustration 01.png|250]]
There are two cases why $\mathbb{P}$ is not a crown:
1. $r \not > f_0$ or $r \not > f_{n-2}$
   WLOG consider case $r \not > f{n-2}$
	1. If $r \nless f_{n-2}$, then card with $f_{n-3}$ removed is not a fence, because it's not connected — $f_{n-2}$ is an [[Isolated Point|isolated point]]
	2. If $r < f_{n-2}$, then card with $f_0$ removed is not a fence, because there is a 3-element [[Linear Order and Chain|chain]] $f_{n-3} > f_{n-2} > r$
2. $r \sim f_k$ with $k \neq n-2$ and $k \neq 0$ — then the picture is:
   ![[Crown is Reconstructible Proof Illustration 02.png|200]] or  ![[Crown is Reconstructible Proof Illustration 03.png|200]]
   Then the card with $f_0$ removed is not a fence, because there is a 3-element chain $r > f_k > f_{k+1}$ or $r < f_k < f_{k+1}$ $\boxtimes$

