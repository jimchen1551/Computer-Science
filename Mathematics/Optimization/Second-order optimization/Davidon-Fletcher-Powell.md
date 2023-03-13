---
Created: [[2023-03-10]]
Aliases: DFP
Types: Card
Tags: 
- 
---
# Davidon-Fletcher-Powell
$$\Delta x_k\approx H_{k+1}^{-1}\Delta g_k$$
$$H_{k+1}^{-1}=H_k^{-1}+\Delta H_k^{-1}$$
$$\Rightarrow\Delta x_k=(H_k^{-1}+\Delta H_k^{-1})\Delta g_k$$
$$\Rightarrow \Delta H_k^{-1}\Delta g_k=\Delta x_k-H_k^{-1}\Delta g_k$$

$$\Delta H_k^{-1}=\alpha_ku_ku_k^T+\beta_kv_kv_k^T$$
$$\Rightarrow (\alpha_ku_ku_k^T+\beta_kv_kv_k^T)\Delta g_k=\Delta x_k-H_k^{-1}\Delta g_k$$
Assume that
$$\alpha_ku_ku_k^T\Delta g_k=\Delta x_k;\ u_k=\Delta x_k$$
$$\beta_kv_kv_k^T\Delta g_k=-H_k^{-1}\Delta g_k;\ v_k=H_k^{-1}\Delta g_k$$
, then
$$\Rightarrow \alpha_k\Delta x_k\Delta x_k^T\Delta g_k=\alpha_k\Delta x_k^T\Delta g_k\Delta x_k=\Delta x_k$$
$$\Rightarrow\beta_k(H_k^{-1}\Delta g_k)(H_k^{-1}\Delta g_k)^T\Delta g_k=\beta_k(H_k^{-1}\Delta g_k)^T\Delta g_k(H_k^{-1}\Delta g_k)=-H_k^{-1}\Delta g_k$$

Arbitrate that $H_k^{-1}$ is a **symmetric** matrix, and because $\alpha_k\Delta x_k^T\Delta g_k$ and $\beta_k(H_k^{-1}\Delta g_k)^T\Delta g_k$ are **scalar**, 
$$\Rightarrow \alpha_k=\frac{1}{\Delta x_k^T\Delta g_k};\ \beta_k=-\frac{1}{(H_k^{-1}\Delta g_k)^T\Delta g_k}$$

Finally, we got
$$H_{k+1}^{-1}=H_k^{-1}+\frac{1}{\Delta x_k^T\Delta g_k}\Delta x_k\Delta x_k^T-\frac{1}{(H_k^{-1}\Delta g_k)^T\Delta g_k}(H_k^{-1}\Delta g_k)(H_k^{-1}\Delta g_k)^T$$
$$\Rightarrow H_{k+1}^{-1}=H_k^{-1}+\frac{\Delta x_k\Delta x_k^T}{\Delta x_k^T\Delta g_k}-\frac{(H_k^{-1}\Delta g_k)(H_k^{-1}\Delta g_k)^T}{(H_k^{-1}\Delta g_k)^T\Delta g_k}$$
- a kind of [[Quasi-Newton method]]
- approximating $H_{k+1}^{-1}$
```Pseudocode
Initialize x_0, H_0=I, k=0
while k<N do
	d_k = -H_k g_k
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
