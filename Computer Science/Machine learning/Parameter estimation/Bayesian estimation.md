---
Created: [[2023-03-17]]
Aliases: BE
Types: Card
Tags: 
- 
---
# Bayesian estimation
$$P(\theta|x)=\frac{P(x|\theta)P(\theta)}{\int_\theta P(x|\theta)p(\theta)d\theta}$$
- similar to [[Maximum a posteriori|MAP]]
- doesn't resolve the value of $\theta$ but take the distribution of $\theta$
- take $\mathbb{E}[P(\theta|x)]$ as the parameter estimation
## Variational inference
$$p(z|x)\approx q(z)$$
$$\min_q D_{KL}(q(z)\|p(z|x))=\min_q\sum_xq(z)\ln\frac{q(z)}{p(z,x)/p(x)}$$
- to approximate $\int_\theta P(x|\theta)p(\theta)d\theta$ we need [[Kullback-Leibler divergence|KL divergence]] to evaluate the result

