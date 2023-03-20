---
Created: [[2023-03-13]]
Aliases: GMM
Types: Card
Tags: 
- 
---
# Gaussian mixture model
$$X\sim GMM(w, \mathcal{N})$$
$$\|w\|_1=1$$
## Continuous form
[[Probability density function|PDF]]/[[Marginal probability density function|MPDF]]:
$$f_X(x)=w^T\mathcal{N}=\sum_{i=1}^nw_i\mathcal{N}(x;\mu_i,\Sigma_i)$$
$$f_X(x|z=i)=\mathcal{N}(x; \mu_i,\Sigma_i)$$
$$f_X(z=i)=w_i$$
$$f_X(x, z=i)=f_X(x|z=i)f_X(z=i)=w_i\mathcal{N}(x;\mu_i,\Sigma_i)$$
