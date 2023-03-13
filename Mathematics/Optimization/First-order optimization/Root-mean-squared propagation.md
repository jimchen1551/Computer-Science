---
Created: [[2023-02-22]]
Aliases: RMSProp
Types: Card
Tags: 
- 
---
# Root-mean-squared propagation
$$E[(\nabla f(x))^2]_k=\delta E[(\nabla f(x))^2]_{k-1}+(1-\delta)(\nabla f(x_k))^2\text{, where }0<\delta<1$$
$$RMS((x_k)_i)=\delta RMS((x_{k-1})_i)+(1-\delta)(\nabla f(x_k))^2\text{, where }0<\delta<1$$
$$(x_{k+1})_i=(x_k)_i-\alpha\frac{(\nabla f(x_k))_i}{\sqrt{(E[(\nabla f(x))^2]_k)_i+\epsilon}}$$
- solving the cumulating denominator problem in [[Adaptive gradient|AdaGrad]] 
- manually setting $\delta$ (coefficient of decay) and $\alpha$
