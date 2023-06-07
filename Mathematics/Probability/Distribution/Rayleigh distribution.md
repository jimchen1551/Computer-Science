---
Created: [[2023-03-13]]
Aliases: 
Types: Card
Tags: 
- 
---
# Rayleigh distribution
$$X\sim Rayleigh(\Sigma)$$
Derivation from [[Universality of the Uniform]]
Given a random vector $(x, y)$ which follows [[Normal distribution#Multivariate normal distribution]] $\mathcal{N}_2(0, \mathbf{I}_{2\times2})$, we transform the Cartesian coordinates to polar coordinates. 
$$r=\sqrt{x^2+y^2},\ \theta=\arctan(\frac{y}{x})$$
$$f_{XY}(x, y)=\frac{1}{2\pi}e^{-\frac{x^2+y^2}{2}}$$
$$f_{R\Theta}(r, \theta)=\frac{1}{2\pi}e^{-\frac{r^2}{2}}\cdot|\det(\frac{\partial (x, y)}{\partial (r, \theta)})|=\frac{1}{2\pi}e^{-\frac{r^2}{2}}\cdot r$$
## Continuous form
[[Probability density function|PDF]]:
$$f_X(x)=\frac{x}{|\Sigma|}e^{-\frac{x^2}{2|\Sigma|}}$$
[[Cumulative distribution function|CDF]]:
$$F_X(x)=1-e^{-\frac{x^2}{2|\Sigma|}}$$
