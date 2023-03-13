---
Created: [[2023-03-10]]
Aliases: 
Types: Card
Tags: 
- 
---
# Covariance
$$\mathbf{cov}(X, Y)=\mathbb{E}[(X-\mathbb{E}[X])(Y-\mathbb{E}[Y])]$$
## Properties
$$\mathbf{cov}(X, Y)=\mathbf{cov}(Y, X)$$
$$\mathbf{cov}(X, Y)=\mathbb{E}[XY]-\mathbb{E}[X]\mathbb{E}[Y]$$
$$\mathbf{cov}(X, X)=\mathbf{var}(X)$$
$$\mathbf{cov}(X, c)=0$$
$$\mathbf{cov}(aX, bY)=ab\cdot\mathbf{cov}(X, Y)$$
$$\mathbf{cov}(X+c, Y+d)=\mathbf{cov}(X, Y)$$
for [[Independent and identically distributed|iid]], 
$$\mathbf{cov}(X, Y)=0$$
## Covariance matrix
$$\Sigma=\begin{bmatrix}
\mathbf{cov}(x_1, x_1)&\cdots&\mathbf{cov}(x_1, x_n)\\
\vdots&\ddots&\vdots\\
\mathbf{cov}(x_n, x_1)&\cdots&\mathbf{cov}(x_n, x_n)
\end{bmatrix}$$
