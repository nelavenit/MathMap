---
tags:
  - Statement
---
**Statement.** Let $\mathbb{P} = (P, \leq)$ be a [[Partial Order|poset]], $F \neq \emptyset$ - [[Filter and Ideal|filter]]. If $P$ is finite, then $F$ is a [[Principal Filter and Ideal]], i.e. $F = \mathord{\uparrow}{f}$ for some $f \in F$.
$\blacktriangle$ Lets give an algorithm for finding $f$: 
1. take arbitrary $f_0 \in F$
2. if $\mathord{\uparrow} f_0 = F$ then we are done, else $\exists f_1 \in F$ s.t. $f_1 \notin \uparrow f_0$, then we take any lower bound of $\{f_1, f_0\} =: f_2,$ which is possible because $F$ is [[Upward and Downward Directed Subsets|downward directed]]. Now $\mathord{\uparrow} f_2$ contains both $\mathord{\uparrow} f_0$ and $f_1$, so we increased the size of our principal filter by at least one element.
3. Repeat the step 2. The algorithm will end because $|F|$ is finite (Note: P is not required to be finite). $\boxtimes$