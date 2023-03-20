---
Created: [[2023-03-18]]
Aliases: JS divergence
Types: Card
Tags: 
- 
---
# Jensen-Shannon divergence
$$D_{JS}(p\|q)=\frac{D_{KL}(p\|q)+D_{KL}(q\|p)}{2}$$
## Properties
1. $$D_{JS}(p\|q)\geq0$$
2. $$D_{JS}(p\|q)= D_{JS}(q\|p)$$
3. $$\text{if }p(x)=q(x)\text{, }D_{JS}(p\|q)=0$$
