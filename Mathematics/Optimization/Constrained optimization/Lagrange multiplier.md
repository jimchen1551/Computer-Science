---
Created: [[2023-01-29]]
Aliases: 
Types: Card
Tags: 
- 
---
# Lagrange multiplier
$$\min_{x}f(x);\ g_i(x)=0,\ i\in[1, n]$$
$$L(x, \lambda)=f(x)+\lambda^Tg(x)$$
taking the [[partial derivatives]] of L, then
$$\Rightarrow\frac{\partial L}{\partial x}=\nabla_xf(x)+\lambda^T\nabla_xg_(x)=0$$
$$\Rightarrow\nabla_xf(x)=-\lambda^T\nabla_xg_(x)$$
and
$$\Rightarrow\frac{\partial L}{\partial \lambda}=g(x)=0$$
- first-order necessary condition
- $\lambda$ is **Lagrange multiplier**
- used to find the extrema of a function with constrained equations
- If the [[Hessian matrix]] is positive definite, the point must be the global minimum
  , and vice versa. 

