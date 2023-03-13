---
Created: [[2023-03-10]]
Aliases: QNM, quasi-newton
Types: Card
Tags: 
- 
---
# Quasi-Newton method
$$f(x)\approx f(x_{k+1})+\nabla f(x_{k+1})^T(x-x_{k+1})$$
$$\Rightarrow\nabla f(x)\approx\nabla f(x_{k+1})+\nabla^2 f(x_{k+1})(x-x_{k+1})$$
$$\Rightarrow\nabla f(x_{k+1})-\nabla f(x_k)\approx\nabla^2f(x_{k+1})(x_{k+1}-x_k)$$
$$\Delta x_k=x_{k+1}-x_k;\ \Delta g_k=\nabla f(x_{k+1})-\nabla f(x_k)$$
$$\Rightarrow \Delta g_k\approx H_{k+1}\Delta x_k$$
**Quasi-Newton condition**:
$$\Delta x_k\approx H_{k+1}^{-1}\Delta g_k$$
- used while [[Newton method]] doesn't work
- constructing an approximate [[Hessian matrix]] and its inverse, which are **positive definite** and **symmetric**

Algorithms:
- [[Davidon-Fletcher-Powell|DFP]]: approximating $H_{k+1}^{-1}$
- [[Broyden-Fletcher-Goldfarb-Shanno|BFGS]]: approximating $H_{k+1}$
