---
Created: [[2023-03-10]]
Aliases: LD
Types: Card
Tags: 
- 
---
# Lagrange duality
$$\min_{x}f(x);\ g_i(x)\leq0,\ i\in[1, m];\ h_j(x)=0,\ j\in[1,n]$$
$$L(x, \lambda,\mu)=f(x)+\lambda^Tg(x)+\mu^Th(x)$$
$$p^*=\min_x\max_{\mu, \lambda\geq0}L(x, \lambda, \mu)=\min_x\theta_P(x)$$
$$d^*=\max_{\mu, \lambda\geq0}\min_xL(x, \lambda, \mu)=\max_{\mu, \lambda\geq0}\theta_D(\lambda, \mu)$$
## Duality gap
$$p^*-d^*$$
## Weak duality
$$d^*\leq p^*$$
## Strong duality
$$p^*=d^*=L(x^*, \lambda^*, \mu^*)$$
- **Slater condition**
	- If an $x$ **strictly** satisfies all constrained inequality ($g(x^*)<0$), there exists $(x^*, \lambda^*, \mu^*)$ to be the optimum of the **original** problem and the **dual** problem
	- the **sufficient** but **not necessary** condition for strong duality