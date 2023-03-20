---
Created: [[2023-03-13]]
Aliases: 
Types: Card
Tags: 
- 
---
# Multivariate normal distribution
$$X\sim\mathcal{N}_k(\mu, \Sigma)$$
- replace the random variables of [[normal distribution]] with random vectors
- $x,\ \mu\in \mathbb{R}^k,\ \Sigma$ is the [[covariance]] matrix of $x$
## Continuous form
[[Probability density function|PDF]]:
$$f_X(x)=\frac{1}{\sqrt{(2\pi)^{n}|\Sigma|}}e^{-\frac{(x-\mu)^T\Sigma^{-1}(x-\mu)}{2}}$$
[[Conjugate prior]]: [[Multivariate normal distribution]]
