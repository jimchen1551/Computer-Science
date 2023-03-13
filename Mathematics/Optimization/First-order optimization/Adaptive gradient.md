---
Created: [[2023-02-22]]
Aliases: AdaGrad
Types: Card
Tags: 
- 
---
# Adaptive gradient
$$(x_{k+1})_i=(x_k)_i-\alpha\frac{\nabla f(x_k)_i}{\sqrt{\sum_{j=1}^k(\nabla f(x_j)_i)^2+\epsilon}}$$
- taking the history of the gradient for iterations to calculate the update dynamically
- manually setting $\alpha$
- with $k$ going bigger, the denominator get larger and larger so that the update would approximate to 0
