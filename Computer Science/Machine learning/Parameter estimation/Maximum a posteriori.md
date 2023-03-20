---
Created: [[2023-03-10]]
Aliases: MAP, MAPE
Types: Card
Tags: 
- 
---
# Maximum a posteriori
$$\mathbf{M}(q)=\arg\max_{l\in levels(t)}P(t=l|q[1],\dots,q[m])$$
$$\mathbf{M}(q)=\arg\max_{\theta}P(\theta|q)=\arg\max_{\theta}\frac{P(q|\theta)P(\theta)}{\int_\theta P(q|\theta)P(\theta)d\theta}=\arg\max_{\theta}P(q|\theta)P(\theta)$$
- aka **MAP** prediction
- **Bayesian**
- different from [[Maximum likelihood|MLE]], it takes parameters as a **random variable**
- the parameter must follow the **prior** distribution
- taking the maximum of the **posterior** probability
- returning the target level with the highest posterior probability given the state of the descriptive features in the query
- more accurate if the prior probability is known
$$P(t=l|q[1],\dots,q[m])=\eta\cdot P(q[1],\dots,q[m]|t=l)P(t=l)$$
## Bernoulli distribution as an example
$$X\sim B(n, p)$$
$$P\sim\mathcal{N}(\mu, \sigma^2)$$
- the random variable $X$ follows [[Bernoulli distribution]]
- the parameter $p$ is the random variable that follows the [[Normal distribution]]
$$\mathbf{M}(x)=\arg\max_{p}P(x|p)P(p)=\arg\max_{p}p^x(1-p)^{n-x}\frac{1}{\sqrt{2\pi}\sigma}e^{-\frac{(p-\mu)^2}{2\sigma^2}}=\arg\max_{p}L(p)$$
$$\mathbf{M}(x)=\arg\max_{p}\ln L(p)=\arg\max_{p}x\ln p+(n-x)\ln(1-p)+\ln\frac{1}{\sqrt{2\pi}\sigma}-\frac{(p-\mu)^2}{2\sigma^2}$$
$$\frac{d\ln L(p)}{dp}=\frac{x}{p}-\frac{n-x}{1-p}-\frac{p-\mu}{\sigma^2}=0$$
$$p(1-p)(p-\mu)=\sigma^2(x-np)$$
$$p^3-(\mu+1)p^2+(\mu-\sigma^2n)p+\sigma^2x=0$$
## Normal distribution as an example
$$X\sim\mathcal{N}(\mu_x, \sigma_x^2)$$
$$\mu_x\sim\mathcal{N}(\mu, \sigma^2)$$
- the random variable $X$ follows [[Normal distribution]]
- the parameter $\mu_x$ is the random variable that follows the [[Normal distribution]]
$$\mathbf{M}(x)=\arg\max_{\mu_x}P(x|\mu_x)P(\mu_x)=\arg\max_{\mu_x}\prod_{i=1}^n(\frac{1}{\sqrt{2\pi}\sigma_x}e^{-\frac{(x_i-\mu_x)^2}{2\sigma_x^2}})\frac{1}{\sqrt{2\pi}\sigma}e^{-\frac{(\mu_x-\mu)^2}{2\sigma^2}}$$
$$\mathbf{M}(x)=\arg\max_{\mu_x}\sum_{i=1}^n(\ln(\frac{1}{\sqrt{2\pi}\sigma_x})-\frac{(x_i-\mu_x)^2}{2\sigma_x^2})+\ln(\frac{1}{\sqrt{2\pi}\sigma})-\frac{(\mu_x-\mu)^2}{2\sigma^2}$$
$$\mathbf{M}(x)=\arg\min_{\mu_x}\sum_{i=1}^n(\frac{(x_i-\mu_x)^2}{2\sigma_x^2})+\frac{(\mu_x-\mu)^2}{2\sigma^2}=\arg\min_{\mu_x}\ln L(\mu_x)$$
$$\frac{d\ln L(\mu_x)}{d\mu_x}=-\sum_{i=1}^n(\frac{x_i-\mu_x}{\sigma_x^2})+\frac{\mu_x-\mu}{\sigma^2}=0$$
$$\mu_x=\frac{\sigma^2\sum_{i=1}^n(x_i)+\sigma_x^2\mu}{\sigma^2n+\sigma_x^2}$$
