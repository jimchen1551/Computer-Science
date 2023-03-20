---
Created: [[2023-03-18]]
Aliases: 
Types: Card
Tags: 
- 
---
# Mutual information
$$I(X, Y)=\sum_x\sum_yp(x, y)\ln\frac{p(x, y)}{p(x)p(y)}$$
$$I(X, Y)=\int_{-\infty}^{+\infty}\int_{-\infty}^{+\infty} p(x, y)\ln\frac{p(x, y)}{p(x)p(y)}dxdy$$
$$I(X, Y)=H(X)+H(Y)-H(X, Y)$$
## Properties
1. $$I(X, Y)\geq0$$$$I(X, Y)\leq H(X)$$$$I(X, Y)\leq H(Y)$$
2. $$I(X, Y)=I(Y, X)$$
3. $$\text{if independence, }I(X, Y)=0$$
