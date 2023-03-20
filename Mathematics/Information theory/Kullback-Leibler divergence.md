---
Created: [[2023-03-18]]
Aliases: KL divergence
Types: Card
Tags: 
- 
---
# Kullback-Leibler divergence
$$D_{KL}(p\|q)=\sum_xp(x)\ln\frac{p(x)}{q(x)}$$
$$D_{KL}(p\|q)=\int_{-\infty}^{+\infty}p(x)\ln\frac{p(x)}{q(x)}dx$$
$$D_{KL}(p\|q)=H_q(p)-H_p(p)$$
- KL divergence is the difference b/w [[Cross entropy]] and [[Shannon's entropy]]
- not a measurement of distance
- the degree of **dissimilarity**
## Properties
1. $$D_{KL}(p\|q)\geq0$$$$H_q(p)\geq H_p(p)$$
2. $$D_{KL}(p\|q)\neq D_{KL}(q\|p)$$
3. $$\text{if }p(x)=q(x)\text{, }D_{KL}(p\|q)=0$$
