---
Created: [[2022-09-21]]
Aliases: 
Types: Card
Tags: 
- 
---
# Exponential distribution
$$X\sim Exponential(\lambda)$$
- $x=$ the time between events in the [[Poisson process]]
- the continuous analog of the [[Geometric distribution]]
- memoryless
## Continuous form
[[Probability density function|PDF]]: 
$$f_X(x)=
\begin{cases}
\lambda e^{-\lambda x}& \quad ,x\geq 0\\
0 & \quad ,otherwise
\end{cases}$$
[[Cumulative distribution function|CDF]]: 
$$F_X(x)=\int_{-\infty}^xf_X(u)du=\int_0^x\lambda e^{-\lambda u}du=
\begin{cases}
1-e^{-\lambda x}&\quad ,x\geq0\\
0&\quad ,x<0
\end{cases}$$
[[Conjugate prior]]: 
[[Gamma distribution]]
