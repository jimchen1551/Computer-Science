---
Created: [[2023-01-30]]
Aliases: 
Types: Note
Tags: 
- 
---
# Optimization
$$\lim_{k\rightarrow+\infty}\nabla f(x_k)=0$$
- [[Fermat's theorem (stationary point)]]
- to find out the optimum of transcendental functions, it's more practical by numerical optimization with **iteration** compared to taking $\nabla f(x)=0$ directly

| First-order optimization           | abbrev   |
| ---------------------------------- | -------- |
| [[Gradient descent]]               | GD       |
| [[Steepest descent]]               | SD       |
| [[Stochastic gradient descent]]    | SGD      |
| [[Gradient descent with momentum]] | GDM      |
| [[Adaptive gradient]]              | AdaGrad  |
| [[Adaptive delta]]                 | AdaDelta |
| [[Root-mean-squared propagation]]  | RMSProp  |
| [[Adaptive moment]]                | Adam     |

| Second-order optimization            | abbrev |
| ------------------------------------ | ------ |
| [[Newton method]]                    | NM     |
| [[Quasi-Newton method]]              | QNM    |
| [[Davidon-Fletcher-Powell]]          | DFP    |
| [[Broyden-Fletcher-Goldfarb-Shanno]] | BFGS   |

| [[Divide and conquer]]              | abbrev   |
| ----------------------------------- | -------- |
| [[Coordinate descent]]              | CD       |
| [[Sequential minimal optimization]] | SMO      |
| [[Adaptive boosting]]               | AdaBoost |

| Constrained optimization | abbrev |
| ------------------------ | ------ |
| [[Lagrange multiplier]]  | LM     |
| [[Lagrange duality]]     | LD     |
| [[Karush-Kuhn-Tucker]]   | KKT    |

## Convex optimization
### Convex set
$$\theta x+(1-\theta)y\in C,\ 0\leq\theta\leq1$$
$$\text{if }Ax=b\text{ and }Ay=b$$
$$\text{then }A(\theta x+(1-\theta)y)=\theta Ax+(1-\theta)Ay=b$$
### n Sub-level set
$$\{f(x)\leq n, x\in D(f)\}$$
$$\text{if }f(x)\leq n\text{ and }f(y)\leq n$$
$$\text{then }f(\theta x+(1-\theta)y)\leq n$$
### Convex problem
$$\min_{x}f(x), x\in C$$
- the feasibility domain is a convex set
- the target function is a convex function
- (D, F) = (feasibility domain, target function)
  - if (convex, non-convex), there exist multiple local minima
  - if (non-convex, convex), local minima locate at the edge of the domain
- the [[Hessian matrix]] of a convex function is positive and semi-definite, so there's **no saddle point**

$$\min_{x}f(x);\ g_i(x)\leq0,\ i\in[1, m];\ h_j(x)=0,\ j\in[1, n]$$
- $g$ is the inequality of constraint function and must be **convex**
- $h$ is the equation of constraint function and must be **linear**
- because the **0 sub-level set** of a convex function is a convex set, it must be $\leq0$

## Pareto optimality
- for multi-objective optimization, we take Pareto improvements for several iterations to reach Pareto optimality
- Pareto improvement: at least one target function gets improved and the others remain
- Pareto optimality: no more Pareto improvement we can take
