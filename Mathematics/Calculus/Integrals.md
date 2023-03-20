---
Created: [[2023-01-27]]
Aliases: integral
Types: Card
Tags: 
- 
---
# Integrals
## Definition
### Summation of changes
$$\Delta x=\sum_{i=1}^n\Delta x_i$$
$$\Delta f(x)=\sum_{i=1}^n\Delta f(x_i)$$
### Integration of differential changes
- summing up the product of the [[Derivatives]] and differential change in variables with $n$ times, where we take the [[Limits|limit]] of $n$ to $\infty$
$$\Delta x=\lim_{n\rightarrow\infty}\sum_{i=1}^ndx=\int dx$$
$$\Delta f(x)=\lim_{n\rightarrow\infty}\sum_{i=1}^ndf(x_i)=\int df(x)=\int f'(x)dx$$
## Properties
1. $$\int_a^bc\cdot dx=c(b-a)$$
2. $$\int c\cdot f(x)dx=c\cdot\int f(x)dx$$
3. $$\int[f(x)\pm g(x)]dx=\int f(x)dx\pm\int g(x)dx$$
4. $$\int_a^af(x)dx=0$$
5. $$\int_a^b f(x)dx=-\int_b^a f(x)dx$$
6. $$\int_a^bf(x)dx=\int_a^cf(x)dx+\int_c^bf(x)dx$$
## Techniques
- [[Integration by substitution]]
- [[Integration by parts]]
- [[Integration by partial fractions]]
- [[Gaussian integral]]
## Rules and theorems
- [[Fundamental theorem of calculus]]
