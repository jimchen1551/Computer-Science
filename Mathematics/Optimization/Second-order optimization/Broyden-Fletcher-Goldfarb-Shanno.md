---
Created: [[2023-03-10]]
Aliases: BFGS
Types: Card
Tags: 
- 
---
# Broyden-Fletcher-Goldfarb-Shanno
$$\Delta g_k\approx H_{k+1}\Delta x_k$$
$$H_{k+1}=H_k+\Delta H_k$$
$$\Rightarrow\Delta g_k=(H_k+\Delta H_k)\Delta x_k$$

$$\Delta H_k=\alpha_ku_ku_k^T+\beta_kv_kv_k^T$$
$$\Rightarrow \Delta g_k=(H_k+\alpha_ku_ku_k^T+\beta_kv_kv_k^T)\Delta x_k$$
$$\Rightarrow \Delta g_k-H_k\Delta x_k=\alpha_ku_k^T\Delta x_ku_k+\beta_kv_k^T\Delta x_kv_k$$
Assume that
$$\alpha_ku_k^T\Delta x_ku_k=\Delta g_k;\ u_k=\Delta g_k$$
$$\beta_kv_k^T\Delta x_kv_k=-H_k\Delta x_k;\ v_k=H_k\Delta x_k$$
, then
$$\Rightarrow \alpha_k\Delta g_k^T\Delta x_k\Delta g_k=\Delta g_k$$
$$\Rightarrow\beta_k(H_k\Delta x_k)^T\Delta x_k(H_k\Delta x_k)=-H_k\Delta x_k$$

Arbitrate that $H_k$ is a **symmetric** matrix, and because $\alpha_k\Delta g_k^T\Delta x_k$ and $\beta_k(H_k\Delta x_k)^T\Delta x_k$ are **scalar**, 
$$\Rightarrow\alpha_k=\frac{1}{\Delta g_k^T\Delta x_k};\ \beta_k=-\frac{1}{(H_k\Delta x_k)^T\Delta x_k}$$

Finally, we got
$$H_{k+1}=H_k+\frac{1}{\Delta g_k^T\Delta x_k}\Delta g_k\Delta g_k^T-\frac{1}{(H_k\Delta x_k)^T\Delta x_k}(H_k\Delta x_k)(H_k\Delta x_k)^T$$
$$\Rightarrow H_{k+1}=H_k+\frac{\Delta g_k\Delta g_k^T}{\Delta g_k^T\Delta x_k}-\frac{(H_k\Delta x_k)(H_k\Delta x_k)^T}{(H_k\Delta x_k)^T\Delta x_k}$$
- a kind of [[Quasi-Newton's method]]
- approximating $H_{k+1}$
- consuming memory (improved version = L-BGFS)
```Pseudocode
Initialize x_0, H_0=I, k=0
while k<N do
	d_k = -H_k^{-1} g_k
	Straight search to get lambda_k
	s_k=lambda_k d_k
	x_{k+1} = x_k + s_k
	if ||g_{k+1}||<epsilon then
		break
	end if
	y_k = g_{k+1} - g_k
	H_{k+1} = H_k + alpha u u^T + beta v v^T
	k += 1
end while
```
