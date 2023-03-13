---
Created: [[2022-09-21]]
Aliases: 
Types: Card
Tags: 
- 
---
# Geometric distribution
$$X\sim Geometric (p)$$
- conducting ([[Independent and identically distributed|iid]]) Bernoulli trials until one success and $x=$ the number of trials conducted
## Discrete form
[[Probability mass function|PMF]]: 
$$p_X(x)=
\begin{cases}
(1-p)^{x-1}\cdot p & \quad ,x\in N^+\\
0 & \quad ,otherwise
\end{cases}$$
[[Cumulative distribution function|CDF]]: 
$$F_X(x)=
\begin{cases}
1-(1-p)^{\lfloor x\rfloor} & \quad ,x\geq1\\
0 & \quad ,otherwise
\end{cases}$$
