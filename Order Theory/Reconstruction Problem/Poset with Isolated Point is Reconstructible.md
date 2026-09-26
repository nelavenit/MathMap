---
tags:
  - Statement
---
**Statement.** The class of finite [[Partial Order|orders]] with at least 4 elements and with an [[Isolated Point|isolated point]] is [[Reconstructibility|reconstructible]].
$\color{red}\text{Proof idea}$ (my own proof for the exercise 1-28 from @schroderOrderedSetsIntroduction2016):
1. Prove the class is [[Recognizability|recognizable]]:
	 Let $\mathbb{P} = (P, \leq_P)$ be a poset. Count $S(\mathbb{P}) = \sum_{c \text{ – cards of }\mathbb{P}} \#(\text{isolated points in }c)$. There are 4 cases:
	1. $S(\mathbb{P}) > |P| \implies \mathbb{P}$ has an isolated point}
	2. $S(\mathbb{P}) < |P| - 1 \implies \mathbb{P}$ hasn't an isolated point  
	3. $S(\mathbb{P}) = |P| \implies$ either $\mathbb{P}$ has an isolated point or $\mathbb{P}$ has a structure:
	   ![[Isolated Point Reconstructibility Proof Case 1.png|200]] (show this structure is reconstructible)  
	4. $S(\mathbb{P}) = |P| - 1 \implies$ Either $\mathbb{P}$ has an isolated point or $P$ has a structure:
	   ![[Isolated Point Reconstructibility Proof Case 2.png|250]] (show this structure is reconstructible)
2. If $\mathbb{P}$ has an isolated point, then $\mathbb{P}$ is the card with the least number of isolated points with one added isolated point