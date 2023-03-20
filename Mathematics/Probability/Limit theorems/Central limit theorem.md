---
Created: [[2023-03-13]]
Aliases: CLT
Types: Card
Tags: 
- 
---
# Central limit theorem
## De Moivre-Laplace theorem
[[Binomial distribution]] → [[Normal distribution]]
$$X\sim BIN(n, p)$$
Normalize the $X$, 
$$\frac{X-np}{\sqrt{npq}}$$
And we have
$$\lim_{n\rightarrow+\infty}P(a\leq\frac{X-np}{\sqrt{npq}}\leq b)=\Phi(b)-\Phi(a)$$
, where $\Phi(x)$ is the [[Standard normal distribution]]

## Lindeberg-Levy theorem
[[Independent and identically distributed|iid]] and finite-[[variance]] random variable sequence → [[Standard normal distribution]]
$$\mathbb{E}[\bar X]=\mu$$
$$\mathbf{var}(\bar X)=\frac{\sigma^2}{n}$$
Normalize the $\bar X$, 
$$\frac{\bar X-\mu}{\sigma/\sqrt{n}}$$
And we have
$$\lim_{n\rightarrow+\infty}P(\frac{\bar X-\mu}{\sigma/\sqrt{n}}\leq x)=\Phi(x)$$
, where $\Phi(x)$ is the [[Standard normal distribution]]

