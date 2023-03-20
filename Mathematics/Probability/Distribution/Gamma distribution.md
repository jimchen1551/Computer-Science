---
Created: [[2022-09-21]]
Aliases: Erlang distribution
Types: Card
Tags: 
- 
---
# Gamma distribution
$$X\sim Erlang (n,\lambda)$$
- similar to [[Exponential distribution]] but $x=$ the time between $k$ events in the [[Poisson process]]
## Continuous form
[[Probability density function|PDF]]: 
$$f_X(x)=
\begin{cases}
\frac{1}{(n-1)!}\lambda^nx^{n-1}e^{-\lambda x}&\quad, x\geq0\\
0 &\quad ,otherwise
\end{cases}$$
[[Cumulative distribution function|CDF]]: 
$$F_X(x)=
\begin{cases}
1-\Sigma_{k=0}^{n-1}\frac{(\lambda x)^k}{k!}e^{-\lambda x}&\quad, x\geq0\\
0 &\quad ,otherwise
\end{cases}$$
[[Conjugate prior]]: [[Gamma distribution]]
