---
Created: [[2022-09-21]]
Aliases: Gaussian distribution
Types: Card
Tags: 
- 
---
# Normal distribution
$$X\sim \mathcal{N} (\mu, \sigma^2)$$
$$X\sim Gaussian (\mu, \sigma)$$

## Continuous form
[[Probability density function|PDF]]:
$$f_X(x)=\frac{1}{\sqrt{2\pi}\sigma}e^{-\frac{(x-\mu)^2}{2\sigma^2}}$$
[[Conjugate prior]]: 
[[Normal distribution]], [[Gamma distribution]]
## Derivation
1. [[Gaussian integral]]
2. [[Central limit theorem]]
   ![[Screenshot 2023-04-11 at 23.38.18.png]]
3. [[Euler-Lagrange equation]]
   To maximize [[Shannon's entropy]] of $f$ 
   $$\begin{cases}
   \int_{-\infty}^{+\infty}p(x) dx\\
   \int_{-\infty}^{+\infty}p(x)\cdot x dx=\mu\\
   \int_{-\infty}^{+\infty}p(x)\cdot(x-\mu)^2 dx=\sigma^2\\
   \end{cases}$$
   $$H[p]=-\int_{-\infty}^{+\infty}p(x)\cdot\ln p(x)dx$$
   Considering the [[Lagrange multiplier]], 
   $$F[p,\alpha,\beta,\gamma]=-\int_{-\infty}^{+\infty}p(x)\ln p(x)dx+\alpha(\int_{-\infty}^{+\infty}p(x)dx-1)+\beta(\int_{\infty}^{+\infty}p(x) xdx-\mu)+\gamma(\int_{-\infty}^{+\infty}p(x)(x-\mu)^2dx-\sigma^2)$$
   The kernel of this [[Functional]] is 
   $$L(x,p(x),p'(x))=-p(x)\ln p(x)+\alpha p(x)+\beta xp(x)+\gamma(x-\mu)^2p(x)$$
   $$\frac{\partial L}{\partial p}-\frac{d}{dx}(\frac{\partial L}{\partial p'})=-(1+\ln p(x))+\alpha+\beta x+\gamma(x-\mu)^2=0$$
   $$p(x)=\exp(\gamma(x-\mu)^2+\beta x+\alpha-1)$$
   $$\begin{cases}
   \alpha=1-\ln(\sqrt{2\pi}\sigma)\\
   \beta=0\\
   \gamma=-\frac{1}{2\sigma^2}
   \end{cases}$$
   $$\Rightarrow p(x)=\frac{1}{\sqrt{2\sigma^2}}\exp(-\frac{(x-\mu)^2}{2\sigma^2})$$

## Standard normal distribution
$$Z\sim N(0, 1)$$
$$\frac{X-\mu}{\sigma}\sim N(0, 1), \forall X\sim N(\mu, \sigma^2)$$
[[Probability density function|PDF]]: 
$$f_Z(z)=\frac{1}{\sqrt{2\pi}}e^{-\frac{z^2}{2}}$$
[[Cumulative distribution function|CDF]]:
$$\Phi(z)=\int_{-\infty}^z\frac{1}{\sqrt{2\pi}}e^{-\frac{u^2}{2}}du$$
$$\Phi(-z)=1-\Phi(z)$$

## Multivariate normal distribution
![[Screenshot 2023-04-12 at 00.04.24.png]]
$$X\sim\mathcal{N}_k(\mu, \Sigma)$$
- replace the random variables of the [[normal distribution]] with random vectors
- $(x-\mu)^T\Sigma^{-1}(x-\mu)$ is the square of [[Distance matric#Mahalanobis distance]]
- $x,\ \mu\in \mathbb{R}^k,\ \Sigma$ is the [[covariance]] matrix of $x$
[[Probability density function|PDF]]:
$$f_X(x)=\frac{1}{\sqrt{(2\pi)^{n}|\Sigma|}}e^{-\frac{(x-\mu)^T\Sigma^{-1}(x-\mu)}{2}}$$
[[Conjugate prior]]: 
[[Normal distribution#Multivariate normal distribution]]

## Conditional Gaussian distribution
![[Screenshot 2023-04-12 at 00.24.09.png]]

## Marginal Gaussian distribution

## 
