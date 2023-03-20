---
Created: [[2022-10-31]]
Aliases: 
Types: Card
Tags: 
- 
---
# Shannon's entropy
Discrete form:
$$H(p)=\mathbb{E}_{p}[-\ln p(x)]=-\sum_ip_i\ln p_i$$
Continuous form: 
$$H(p)=-\int_{-\infty}^{+\infty}p(x)\ln p(x)dx$$
Practical form: 
$$H(t, D)=-\sum_iP(t=i)\lg P(t=i)$$
$t$ for target features; $D$ for dataset
- measuring the uncertainty of a probability distribution (or the impurity, heterogeneity of a set)
- The higher $Probability$ an outcome has a lower $Entropy$ it implies. 
- If we have $M$ uniform outcomes in total, we need $\lceil\lg M\rceil$ bits ($\lceil\lg Pr\rceil$, also can be seen as the number of uncertainty) at least to encode each outcome. 
## Properties
1. Maximum
$$H(p)=-\sum_{i=1}^nx_i\ln x_i;\ \sum_{i=1}^nx_i=1;\ x_i\geq0$$
Considering the [[Lagrange multiplier]], 
$$L(x, \lambda)=-\sum_{i=1}^nx_i\ln x_i+\lambda(\sum_{i=1}^nx_i-1)$$
$$\frac{\partial L}{\partial x_i}=-\ln x_i-1+\lambda=0|i\in[1, n];\ \sum_{i=1}^nx_i=1$$
$$\text{if }x_i=\frac{1}{n},\ H(p)=\ln n\text{ is the maximum for }H(p).$$
Considering the second [[Derivatives|derivative]], 
$$\frac{\partial^2H}{\partial x_i^2}=-\frac{1}{x_i};\ \frac{\partial^2 H}{\partial x_i\partial x_j}=0,\ i\neq j$$
$$\nabla^2H=\begin{bmatrix}
-\frac{1}{x_1}&0&\cdots&0\\
0&-\frac{1}{x_2}&\cdots&0\\
\vdots&\vdots&\ddots&\vdots\\
0&0&\cdots&-\frac{1}{x_n}
\end{bmatrix}$$
Because the [[Hessian matrix]] is negative definite, [[Shannon's entropy]] is a concave function and has the maximum if $x_i=\frac{1}{n}$. 
2. Minimum
$$x_i=1, x_j=0,\ \forall j\neq i$$
$$H(p)=1\ln 1+(n-1)\cdot0\ln0=0$$
3. If the random variable follows [[Normal distribution]], the entropy has the maximum. 
$$\begin{cases}
\int_{-\infty}^{+\infty}p(x) dx\\
\int_{-\infty}^{+\infty}p(x)\cdot x dx=\mu\\
\int_{-\infty}^{+\infty}p(x)\cdot(x-\mu)^2 dx=\sigma^2\\
\end{cases}$$
The [[Functional]] of [[Shannon's entropy]] is
$$H[p]=-\int_{-\infty}^{+\infty}p(x)\cdot\ln p(x)dx$$
Considering the [[Lagrange multiplier]], 
$$F[p,\alpha,\beta,\gamma]=-\int_{-\infty}^{+\infty}p(x)\ln p(x)dx+\alpha(\int_{-\infty}^{+\infty}p(x)dx-1)+\beta(-\int_{\infty}^{+\infty}p(x) xdx-\mu)+\gamma(\int_{-\infty}^{+\infty}p(x)(x-\mu)^2dx-\sigma^2)$$
The kernel of this [[Functional]] is 
$$L(x,p(x),p'(x))=-p(x)\ln p(x)+\alpha p(x)+\beta xp(x)+\gamma(x-\mu)^2p(x)$$
According to the [[Euler-Lagrange equation]], 
$$\frac{\partial L}{\partial p}-\frac{d}{dx}(\frac{\partial L}{\partial p'})=-(1+\ln p(x))+\alpha+\beta x+\gamma(x-\mu)^2=0$$
$$p(x)=\exp(\gamma(x-\mu)^2+\beta x+\alpha-1)$$
$$\begin{cases}
\alpha=1-\ln(\sqrt{2\pi}\sigma)\\
\beta=0\\
\gamma=-\frac{1}{2\sigma^2}
\end{cases}$$
$$\Rightarrow p(x)=\frac{1}{\sqrt{2\sigma^2}}\exp(-\frac{(x-\mu)^2}{2\sigma^2})$$
$$H(p)=\ln(\sqrt{2\pi\sigma^2}+\frac{1}{2}$$
## Bernoulli distribution as an example
$$H(p)=-p\ln p-(1-p)\ln(1-p)$$
