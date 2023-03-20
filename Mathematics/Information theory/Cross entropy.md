---
Created: [[2023-03-17]]
Aliases: 
Types: Card
Tags: 
- 
---
# Cross entropy
$$H_q(p)=\mathbb{E}_p[-\ln q]=-\sum_xp(x)\ln q(x)=-\int_{-\infty}^{+\infty}p(x)\ln q(x)dx$$
## Properties
1. $$\text{if }p(x)=q(x),\ H_q(p)=H(p)=H(q)$$
2. $$H_q(p)\neq H_p(q)$$
3. $$\text{If }p=q\text{, then }H_q(p)\text{ has the minimum.}$$
$$H_a(x)=-\sum_{i=1}^na_i\ln x_i;\ \sum_{i=1}^nx_i=1$$
Considering the [[Lagrange multiplier]], 
$$L(x, \lambda)=-\sum_{i=1}^na_i\ln x_i+\lambda(\sum_{i=1}^nx_i-1)$$
$$\begin{cases}
\frac{\partial L}{\partial x_i}=-\frac{a_i}{x_i}+\lambda=0\\
\sum_{i=1}^nx_i=1\\
\sum_{i=1}^na_i=1
\end{cases}$$
$$\Rightarrow \lambda=1;\ x_i=a_i$$
Considering the second [[Derivatives|derivative]], 
$$\frac{\partial^2H}{\partial x_i^2}=\frac{a_i}{x_i^2};\ \frac{\partial^2H}{\partial x_i\partial x_j}=0,\ i\neq j$$
$$\nabla^2H=\begin{bmatrix}
\frac{a_1}{x_1^2}&0&\cdots&0\\
0&\frac{a_2}{x_2^2}&\cdots&0\\
\vdots&\vdots&\ddots&\vdots\\
0&0&\cdots&\frac{a_n}{x_n^2}
\end{bmatrix}$$
Because the [[Hessian matrix]] is positive definite, [[Cross entropy]] is a convex function and has the minimum if $a_i=x_i$. 