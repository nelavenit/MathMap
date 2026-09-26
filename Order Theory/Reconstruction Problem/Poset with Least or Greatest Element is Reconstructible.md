---
tags:
  - Statement
---
**Statement.** The class of *finite* [[Partial Order|posets]] with at least 4 elements and the [[Least and Greatest Elements|least element]] ([[Least and Greatest Elements|greatest element]]) is [[Reconstructibility|reconstructible]].
$\color{red}\text{Proof idea}$ (Pr.1.37. from @schroderOrderedSetsIntroduction2016):
1. Show this class is [[Recognizability|recognizable]]
	1. If $\mathbb{P}$ has a least element, then there is at most one [[Card|card]] without one
	2. If $\mathbb{P}$ doesn't have a least element then there are at least two incomparable elements that don't have any strict [[Lower and Upper Bounds|lower bound]] $\implies$ this order has at most two cards with a least element
2. Now we have a way to check if a set has a least element and reconstruct it determining which cards have the biggest "number of times a least element can be removed before we arrive at an order without a least element"
3. $\mathbb{P}$ is any of the found cards with one least element added 
4. The very same way we show the class of orders with the greatest element is reconstructible $\boxtimes$
