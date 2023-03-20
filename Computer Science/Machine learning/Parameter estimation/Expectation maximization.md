---
Created: [[2023-03-17]]
Aliases: EM
Types: Card
Tags: 
- 
---
# Expectation maximization
![[Pasted image 20230319194335.png]]
- the most classic way to tackle latent variables 
- constructing the lower bound function (easier for [[optimization]]) for [[Maximum likelihood|MLE]]
1. Considering the [[Maximum likelihood|MLE]], $$L(\theta)=\sum_{i=1}^n\ln p(x_i; \theta)=\sum_{i=1}^n\ln\sum_{z}p(x_i, z; \theta)$$, where $L$ is the likelihood function to be maximized and $z$ is the latent variable.
2. Construct the lower bound function with the [[probability]] distribution of the latent variable $z$ and consider [[Jensen's inequality]] and $\ln$ is a concave function, $$\sum_{i=1}^n\ln p(x_i; \theta)=\sum_{i=1}^n\ln\sum_{z}Q(z)\frac{p(x_i, z; \theta)}{Q(z)}\geq\sum_{i=1}^n\sum_zQ(z)\ln\frac{p(x_i, z; \theta)}{Q(z)}$$, where $Q(z)$ is the [[Probability mass function|PMF]] of the random variable $z$. 
3. Initialize $\theta$ and iterate. 
4. E: $$Q_t(z)=p(z|x; \theta_t)$$
5. M: $$\theta_{t+1}=\arg\max_\theta\sum_{i=1}^n\sum_zQ_t(z)\ln\frac{p(x_i, z;\theta)}{Q_t(z)}$$
## [[Gaussian mixture model|GMM]] as an example
