---
Created: [[2022-09-21]]
Aliases: 
Types: Card
Tags: 
- 
---
# Pascal distribution
$$X\sim Pascal(k,p)$$
- negative binomial distribution
- conducting ([[Independent and identically distributed|iid]]) Bernoulli's trials until the number of successes reached $k$ and $x=$ the number of trials
- the last time of trial must be success
## Discrete form
[[Probability mass function|PMF]]: 
$$p_X(x)=
\begin{cases}
\binom {x-1}{k-1}\cdot(1-p)^{x-k}\cdot p^k & \quad ,x=k, k+1, \dots\\
0 &\quad ,otherwise.
\end{cases}$$
[[Cumulative distribution function|CDF]]: 
$$F_X(x)=P(Y\geq k), Y\sim BIN(x, p)$$
[[Conjugate prior]]: [[Beta distribution]]
