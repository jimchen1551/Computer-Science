---
Created: [[2023-04-11]]
Aliases: 
Types: Card
Tags: 
- 
---
# Dirichlet distribution
![[Screenshot 2023-04-11 at 23.21.32.png]]
![[Screenshot 2023-04-11 at 23.22.17.png]]
$$X\sim Dir(\alpha)$$
- in [[Multinomial distribution]], the [[probability]] is a parameter
- in [[Dirichlet distribution]], the [[probability]] is a random variable

## Discrete form
[[Probability density function|PDF]]:
$$f_X(x)=\frac{\Gamma(\alpha_0)}{\Gamma(\alpha_1)\cdots\Gamma(\alpha_k)}\prod_{i=1}^k\mu_i^{\alpha_i-1}$$
$$\Gamma(x)=\int_0^\infty\ u^{x-1}\ e^{-u}du$$
[[Conjugate prior]]: 
[[Multinomial distribution]]
