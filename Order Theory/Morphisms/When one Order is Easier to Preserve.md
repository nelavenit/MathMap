---
tags:
  - Statement
---
**Statement.** Let $\mathbb{P}=(X,\leq)$ and $\mathbb{Q}=(X,\leq')$ be such [[Partial Order|orders]], that every $f:X\to X$ that [[Order Endomorphism|preserves]] $\leq$ also preserves $\leq'$ (in other words every [[Order Endomorphism|endomorphism]] of $\mathbb{P}$ is an endomorphism of $\mathbb{Q}$, i.e. $End \mathbb{P} \subseteq End \mathbb{Q}$), then there are only 3 cases: 
1. $\leq = \leq'$
2. $\leq'$ is the [[Dual Order|dual ordering]] $\leq^d$ of $\leq$
3. no two points are $\leq'$-comparable, i.e. $\mathbb{Q}$ is an [[Antichain|antichain]]
$\blacktriangle$ (Theorem 1 from @gibsonEndomorphismClassesOrdered1998) 
If $\mathbb{Q}$ is an antichain then every map $f: X → X$ is order-preserving in $\mathbb{Q}$. We will suppose that there is at least one comparability in $\mathbb{Q}$. The same way, if $\mathbb{P}$ is an antichain, then $End\mathbb{P} = X^X \Rightarrow End\mathbb{Q} = X^X \Rightarrow \mathbb{Q}$ is an antichain. So let's assume there is at least one comparability in $\mathbb{P}$.
Let $y \nleq x$, and let a < b. Then there exists a [[Generic Order Homomorphism|generic endomorphism]] $f$ of $\mathbb{P}$ such that $f(x) = a$ and $f(y) = b$. We shall write $f$ as $f[y, a, b]$ and vary the parameters (that is, we vary y, a and b) to specify other such maps. 

Let's show $\mathbb{P}$ and $\mathbb{Q}$ have the same comparabilities.
1. Let a < b. By assumption at least two elements of X are comparable in $\mathbb{Q}$, say x <' y. Either $y \not\leq x$ or $x \not\leq y$, so that either $f[y, a, b]$ or $f[x, a, b]$ is an endomorphism of $\mathbb{P}$, s.t. casts $\{x,y\}$ into $\{a,b\}$ (either $f[y,a,b](x)=a$ and $f[y,a,b](y)=b$ or $f[x,a,b](x)=b$ and $f[x,a,b](y)=a$). By assumption it is also an endomorphism of $\mathbb{Q}$. Thus {a, b} is the order preserving image of a comparable pair $\{x,y\}$ in $\mathbb{Q}$, so $a$ and $b$ are comparable in $\mathbb{Q}$. This means "$a,b$  are $\leq$-comparable" implies "$a,b$  are $\leq'$-comparable".

2. Let $x$ and $y$ be incomparable in $\mathbb{P}$, and consider $a < b$ from previous paragraph. Then both $f[y, a, b]$ and $f[x, a, b]$ are order-preserving maps of $\mathbb{P}$ and hence of $\mathbb{Q}$. Since $a$ and $b$ are comparable in $Q$, $x$ and $y$ cannot be (otherwise one of the foregoing maps would not be order-preserving). This means "$x,y$  are $\leq$-incomparable" implies "$x,y$  are $\leq'$-incomparable".

So far we have shown that $\mathbb{P}$ and $\mathbb{Q}$ have the same comparabilities. Now fix $a < b$ and let $x < y$. Suppose that $b <' a$. It follows that $y \nless' x$, because $f[y, a, b]$ is an order-preserving map of $\mathbb{P}$ (and hence of $\mathbb{Q}$), then $y <' x$ because $x$ and $y$ are comparable in $\mathbb{Q}$. Since $x$ and $y$ were an arbitrary comparable pair, this shows that $\mathbb{Q} = \mathbb{P}^d$. If, on the other hand, we suppose that $a <' b$, then it follows similarly that $\mathbb{Q} = \mathbb{P}$. $\boxtimes$
