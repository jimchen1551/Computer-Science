---
Created: [[2023-01-27]]
Aliases: NM
Types: Card
Tags: 
- 
---
# Newton method
$$\text{if }x_n\text{ is the }n^{th}\text{ guess for the solution of }f(x)=0,$$
$$\text{then }(n+1)^{th}\text{ guess is }x_{n+1}=x_n-\frac{f(x_n)}{f'(x_n)}\text{ provided that }f'(x_n)\text{ exists}$$
## For optimization
Second-order Taylor expansion:
$$f(x+\Delta x)=f(x)+\nabla f(x)^T\Delta x+\frac{1}{2}\Delta x^T\nabla^2f(x)\Delta x+o\|\Delta x^2\|$$
→ taking the [[Gradient]] of this equation
$$\nabla f(x+\Delta x)\approx\nabla f(x)+\nabla^2f(x)\Delta x$$
→ because we're finding the optimum where $x=x+\Delta x$ and $\nabla f(x+\Delta x)=0$
$$\nabla f(x)+\nabla^2f(x)\Delta x\approx0$$
$$\Rightarrow \Delta x=-(\nabla^2f(x))^{-1}\nabla f(x)=-H^{-1}\nabla f(x)$$
, where $-H^{-1}\nabla f(x)$ is called Newton direction
- converge faster than [[Gradient descent]]
- more expansive computation (computing [[Gradient]] and [[Hessian matrix]] and its inverse matrix for each iteration)
- however, the [[Hessian matrix]] might not be invertible; hence, we take the [[Quasi-Newton method]] to approximate the inverse of the [[Hessian matrix]]
```Pseudocode
Initialize x_0, k = 0
while k<N do
	Calculate g_k and H_k
	if ||g_k||<epsilon then
		break
	end if 
	d_k = -H_k^{-1} g_k
	x_{k+1} = x_k + alpha d_k
	k += 1
end while
```
