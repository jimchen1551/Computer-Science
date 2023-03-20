---
Created: [[2023-03-15]]
Aliases: 
Types: Card
Tags: 
- 
---
# Beta distribution
$$X\sim Beta(\alpha, \beta)$$
- in [[Binomial distribution]], the [[probability]] is a parameter
- in [[Beta distribution]], the [[probability]] is a random variable

## Discrete form
[[Probability density function|PDF]]:
$$f_X(x)=\frac{1}{B(\alpha, \beta)}\ x^{\alpha-1}\ (1-x)^{\beta-1}$$
$$B(\alpha,\beta)=\int_0^1\ t^{\alpha-1}\ (1-t)^{\beta-1}$$
[[Cumulative distribution function|CDF]]:
$$F_X(x)=\frac{f_X(x)}{B(\alpha,\beta)}$$
