---
Created: [[2023-03-10]]
Aliases: 
Types: Card
Tags: 
- 
---
# Variance
$$\mathbf{var}(X)=\mathbb{E}[(X-\mathbb{E}[X])^2]=\mathbb{E}[X^2]-\mathbb{E}[X]^2$$
## for discrete random variables
$$\mathbf{var}(X)=\sum_i(x_i-\mathbb{E}[X])^2\cdot p(x_i)$$
## for continuous random variables
$$\mathbf{var}(X)=\int_{-\infty}^{\infty}(x-\mathbb{E}[X])^2\cdot p(x)dx$$
## Properties
$$\mathbf{var}(X+c)=\mathbf{var}[X]$$
$$\mathbf{var}(kX)=k^2\cdot\mathbf{var}[X]$$
$$\mathbf{var}(X+Y)=\mathbf{var}(X)+\mathbf{var}(Y)+2\mathbf{cov}(X, Y)$$
