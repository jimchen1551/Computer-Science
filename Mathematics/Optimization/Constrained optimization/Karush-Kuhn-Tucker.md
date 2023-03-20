---
Created: [[2023-03-10]]
Aliases: KKT
Types: Card
Tags: 
- 
---
# Karush-Kuhn-Tucker
$$\min_{x}f(x);\ g_i(x)\leq0,\ i\in[1, m];\ h_j(x)=0,\ j\in[1, n]$$
$$L(x, \lambda,\mu)=f(x)+\lambda^Tg(x)+\mu^Th(x)$$
taking the [[Partial derivatives]] of L, then
$$\Rightarrow\frac{\partial L}{\partial x}=\nabla_xf(x)+\lambda^T\nabla_xg_(x)+\mu^T\nabla_xh(x)=0$$
and
$$\Rightarrow g(x)\leq0$$
and
$$\Rightarrow\frac{\partial L}{\partial \mu}=h(x)=0$$
Additionally, the optimum also satisfies
$$\lambda^Tg(x)=0,\ \lambda_i\geq0$$
- first-order necessary condition
- $\lambda$ and $\mu$ are **KKT multipliers**
- the original optimum is at the **saddle point** of the [[Lagrange multiplier]] function
  (taking min with respect to $x$ and max with respect to KKT multipliers)
- For **convex problems**, it's **sufficient** and **necessary**. 