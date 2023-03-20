---
Created: [[2023-03-18]]
Aliases: 
Types: Card
Tags: 
- 
---
# Conditional entropy
$$H(Y|X)=-\sum_x\sum_yp(x, y)\ln\frac{p(x, y)}{p(x)})$$
$$H(Y|X)=-\int_{-\infty}^{+\infty}\int_{-\infty}^{+\infty} p(x, y)\ln\frac{p(x, y)}{p(x)}dxdy$$
$$H(Y|X)=H(X, Y)-H(X)=H(X)-I(X, Y)$$
## Properties
1. $$H(Y|X)\geq0$$
2. $$H(X)\geq H(X|Y)$$
3. $$\text{if fully dependence, }H(Y|X)=0$$
4. $$\text{if independence, }H(Y|X)=H(Y)$$
