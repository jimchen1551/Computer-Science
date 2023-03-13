---
Created: [[2023-02-22]]
Aliases: Adam
Types: Card
Tags: 
- 
---
# Adaptive moment
$$(m_k)_i=\beta_1(m_{k-1})_i+(1-\beta_1)(\nabla f(x_k))_i$$
$$(\nu_k)_i=\beta_2(\nu_{k-1})_i+(1-\beta_2)(\nabla f(x_k))^2_i$$
, where $0<\beta_1, \beta_2<1$
$$(x_{k+1})_i=(x_k)_i-\alpha\frac{\sqrt{1-\beta_2^k}}{1-\beta_1^k}\frac{(m_k)_i}{\sqrt{(\nu_k)_i}+\epsilon}$$
- automatically setting and updating the learning rate and momentum
