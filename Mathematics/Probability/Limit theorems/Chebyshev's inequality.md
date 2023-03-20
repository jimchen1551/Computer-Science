---
Created: [[2023-03-13]]
Aliases: 
Types: 
Tags: 
- 
---
# Chebyshev's inequality
$$P(|x-\mu|\geq\epsilon)\leq\frac{\sigma^2}{\epsilon^2}$$
## Proof
$$P(|x-\mu|\geq\epsilon)=\int_{|x-\mu|\geq\epsilon}f(x)dx$$
$$\leq\int_{|x-\mu|\geq\epsilon}\frac{|x-\mu|^2}{\epsilon^2}f(x)dx\leq\frac{1}{\epsilon^2}\int_{\mathbb{R}}|x-\mu|^2f(x)dx=\frac{\sigma^2}{\epsilon^2}$$
