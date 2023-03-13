---
Created: [[2023-02-22]]
Aliases: AdaDelta
Types: Card
Tags: 
- 
---
# Adaptive delta
$$E[(\nabla f(x))^2]_k=\rho E[(\nabla f(x))^2]_{k-1}+(1-\rho)(\nabla f(x_k))^2$$
$$RMS[\nabla f(x_k)]=\sqrt{E[(\nabla f(x_k))^2]+\epsilon}$$
$$\Delta x_k=-\frac{RMS[\Delta x]_{k-1}}{RMS[\nabla f(x)]_k}\nabla f(x_k)$$
$$E[\Delta x^2]_k=\rho E[\Delta x^2]_{k-1}+(1-\rho)\Delta x_k^2$$
- automatically setting the learning rate
## Initialization
$$E[(\nabla f(x))^2]_0=0$$
$$E[\Delta x^2]_0=0$$
