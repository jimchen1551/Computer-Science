---
Created: [[2023-03-10]]
Aliases: ML, MLE
Types: Card
Tags: 
- 
---
# Maximum likelihood
$$\mathbf{M}(q)=\arg\max_{l\in levels(t)}P(q[1],\dots,q[m]|t=l)$$
$$\mathbf{M}(q)=\arg\max_{\theta}P(q[1],\dots,q[m]|\theta)$$
- aka **MLE** prediction
- **Frequentist**
- Real is rational, and rational is real
- creating a **likelihood function** and make it maximized to yield the best parameter
	- the likelihood is evaluated with **data observed**
	- the parameter making the data observed have the maximal likelihood is the **best parameter** (and there exists only one best parameter)
- returning the target level with the highest conditional probability given the state of the descriptive features in the query
- equivalent to minimizing the [[Kullback-Leibler divergence|KL divergence]]

If the queries are [[Independent and identically distributed|iid]], 
$$\mathbf{M}(q)=\arg\max_{l\in levels(t)}\prod_{i=1}^mP(q[i]|t=l)$$
$$\mathbf{M}(q)=\arg\max_{\theta}\prod_{i=1}^mP(q[i]|\theta)$$
Then, 
$$\mathbf{M}(q)=\arg\max_{l\in levels(t)}\sum_{i=1}^m\ln P(q[i]|t=l)$$
$$\mathbf{M}(q)=\arg\max_{\theta}\sum_{i=1}^m\ln P(q[i]|\theta)$$
- It's an unconstrained [[optimization]] problem and can be resolved directly or by [[Gradient descent]] or [[Newton's method]]
## Bernoulli distribution as an example
$$\mathbf{M}(n, x)=\arg\max_{p}\ln(p^x(1-p)^{n-x})=\arg\max_{p}x\ln p+(n-x)\ln(1-p)$$
$$\frac{d(x\ln p+(n-x)\ln(1-p))}{dp}=\frac{x}{p}-\frac{n-x}{1-p}=0$$
$$\mathbf{M}(n, x)=\frac{x}{n}$$
## Normal distribution as an example
$$\mathbf{M}(X)=\arg\max_{\mu,\ \sigma}\prod_{i=1}^n\frac{1}{\sqrt{2\pi}\sigma}e^{-\frac{(x_i-\mu)^2}{2\sigma^2}}=\arg\max_{\mu,\ \sigma}(2\pi\sigma^2)^{-\frac{n}{2}}e^{-\frac{1}{2\sigma^2}\sum_{i=1}^n(x_i-\mu)^2}$$
$$\mathbf{M}(X)=\arg\max_{\mu,\ \sigma}-\frac{n}{2}\ln(2\pi\sigma^2)-\frac{1}{2\sigma^2}\sum_{i=1}^n(x_i-\mu)^2=\arg\max_{\mu,\ \sigma}\ln L(\mu, \sigma)$$
$$\frac{\partial \ln L(\mu, \sigma)}{\partial \mu}=\frac{1}{\sigma^2}\sum_{i=1}^n(x_i-\mu)=0$$
$$\frac{\partial \ln L(\mu, \sigma)}{\partial \sigma}=-\frac{n}{\sigma}+\frac{1}{\sigma^3}\sum_{i=1}^n(x_i-\mu)^2=0$$
$$\mu=\frac{1}{n}\sum_{i=1}^nx_i$$
$$\sigma^2=\frac{1}{n}\sum_{i=1}^n(x_i-\mu)^2$$
## Multivariate normal distribution as an example
$$\mathbf{M}(X)=\arg\max_{\mu,\ \Sigma}\prod_{i=1}^m\frac{1}{\sqrt{(2\pi)^{n}|\Sigma|}}e^{-\frac{(x_i-\mu)^T\Sigma^{-1}(x_i-\mu)}{2}}=\arg\max_{\mu,\ \Sigma}(2\pi)^{-\frac{nm}{2}}|\Sigma|^{-\frac{m}{2}}e^{-\frac{1}{2}\sum_{i=1}^m(x_i-\mu)^T\Sigma^{-1}(x_i-\mu)}$$
$$\mathbf{M}(X)=\arg\max_{\mu,\ \Sigma}-\frac{nm}{2}\ln(2\pi)-\frac{m}{2}\ln|\Sigma|-\frac{1}{2}\sum_{i=1}^m(x_i-\mu)^T\Sigma^{-1}(x_i-\mu)=\arg\max_{\mu,\ \Sigma}\ln L(\mu, \Sigma)$$
$$\nabla_{\mu}\ln L(\mu, \Sigma)=\sum_{i=1}^m\Sigma^{-1}(x_i-\mu)=0$$
$$\nabla_{\Sigma}\ln L(\mu, \Sigma)=-\frac{m}{2\Sigma}+\frac{1}{2\Sigma^2}\sum_{i=1}^m(x_i-\mu)(x_i-\mu)^T=0$$
$$\mu=\frac{1}{m}\sum_{i=1}^mx_i$$
$$\Sigma=\frac{1}{m}\sum_{i=1}^m(x_i-\mu)(x_i-\mu)^T$$
