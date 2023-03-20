---
Created: [[2023-03-17]]
Aliases: KDE, Parzen window
Types: Card
Tags: 
- 
---
# Kernel density estimation
$$P(x)=\frac{1}{nh^d}\sum_{i=1}^nK(\frac{x-x_i}{h})$$
, where $K$ is the **kernel function**, $h$ is the **window radius** of the kernel function, $d$ is the dimension of $x$, and $\frac{1}{nh^d}$ is to make the [[Integrals|integral]] sum up to 1 ([[Law of total probability]])
- a non-parameter estimation technique 
  (no need to have parameters of [[Probability density function|PDF]])
- overlapping a set of standard functions (kernel, $K(x)$) to express [[Probability density function|PDF]]
- kernel function ensuring the function value decrease while $x$ keeps away from $x_i$
- If the samples are denser beside $x$, $x$ yields higher probability, and vice versa. 
## Kernel function
$$P(x)=\lim_{n\rightarrow+\infty}\frac{1}{nh^d}\sum_{i=1}^nK(\frac{x-x_i}{h})=\int_{\mathbb{R}^d}\frac{1}{h^d}K(\frac{x-x_i}{h})dx=1$$
$$\Rightarrow\frac{1}{h^d}\int_{\mathbb{R}^d}K(\frac{x-x_i}{h})dx=\frac{1}{h^d}\int_{\mathbb{R}^d}K(y)|\det(\frac{\partial x}{\partial y})|dy=1$$
$$\because\frac{x-x_i}{h}=y\Rightarrow x=hy+x_i$$
$$\therefore\frac{\partial x}{\partial y}=
\begin{bmatrix}
h&0&\cdots&0\\
0&h&\cdots&0\\
\vdots&\vdots&\ddots&\vdots\\
0&0&\cdots&h
\end{bmatrix}$$
$$\Rightarrow\frac{1}{h^d}\int_{\mathbb{R}^d}K(\frac{x-x_i}{h})dx=\frac{1}{h^d}\int_{\mathbb{R}^d}K(y)h^ddy=\int_{\mathbb{R}^d}K(y)dy=1$$
$$\int_{\mathbb{R}^d}K(y)dy=1$$
- common kernel: 
  1. **Radially symmetric kernel** ($K(x)=c_{k,d}k\|x\|^2$), where $k$ is the profile function
  2. **Epanechnikov kernel** ($K(x)=c_d^{-1}(d+2)(1-\|x\|^2)/2 \text{ if }\|x\|\leq1;\ 0\text{ else}$)
     Epanechnikov profile ($k(x)=1-x\text{ if }0\leq x\leq1;\ 0\text{ else}$)
  3. **Multivariate Gaussian kernel** ($K(x)=(2\pi)^{-\frac{d}{2}}\exp{-\frac{\|x\|^2}{2}}$)
     Gaussian profile ($k(x)=\exp(-\frac{x}{2})$)
