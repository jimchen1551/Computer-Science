---
Created: [[2023-03-15]]
Aliases: 
Types: Card
Tags: 
- 
---
# Beta distribution
![[Screenshot 2023-04-11 at 23.11.33.png]]
$$X\sim Beta(\alpha, \beta)$$
- in [[Binomial distribution]], the [[probability]] is a parameter
- in [[Beta distribution]], the [[probability]] is a random variable

## Discrete form
[[Probability density function|PDF]]:
$$f_X(x)=\frac{1}{B(\alpha, \beta)}\ x^{\alpha-1}\ (1-x)^{\beta-1}$$
$$B(\alpha,\beta)=\int_0^1\ t^{\alpha-1}\ (1-t)^{\beta-1}$$
[[Cumulative distribution function|CDF]]:
$$F_X(x)=\frac{f_X(x)}{B(\alpha,\beta)}$$
[[Expectation]]: 
$$\mathbb{E}[x]=\frac{\alpha}{\alpha+\beta}$$
[[Variance]]: 
$$\mathbf{var}[x]=\frac{\alpha\beta}{(\alpha+\beta)^2(\alpha+\beta+1)}$$
[[Conjugate prior]]: 
[[Binomial distribution]]
![[Screenshot 2023-04-11 at 23.17.40.png]]
