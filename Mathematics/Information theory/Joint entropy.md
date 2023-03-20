---
Created: [[2023-03-17]]
Aliases: 
Types: Card
Tags: 
- 
---
# Joint entropy
$$H(X, Y)=-\sum_x\sum_yp(x, y)\ln p(x,y)$$
$$H(X, Y)=-\int_{-\infty}^{+\infty}\int_{-\infty}^{+\infty}p(x, y)\ln p(x,y)dxdy$$
## Properties
1. $$H(X_1, \cdots, X_n)\geq0$$
2. $$H(X, Y)=H(X)+H(Y)\text{, if independence}$$
3. $$\text{for multivariate normal distribution, }H(x)=\frac{n}{2}\ln2+\frac{1}{2}\ln|\Sigma|+\frac{n}{2}$$
