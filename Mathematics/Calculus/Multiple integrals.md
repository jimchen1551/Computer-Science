---
Created: [[2023-01-29]]
Aliases: multiple integral
Types: Card
Tags: 
- 
---
# Multiple integrals
## Definition
### Double integral
$$V=\iint_Df(x, y)\ dA$$
$$\iint_Rf(x, y)dA=\int_a^b\int_c^df(r\cos{\theta}, r\sin{\theta})\ rd\theta\ dr$$
$$\iint_Rf(x)\ g(y)\ dA=\int_a^bf(x)\ dx\int_c^dg(y)\ dy$$
#### Fubini's theorem
$$\iint_Rf(x, y)\ dA=\int_a^b\int_c^df(x, y)\ dy\ dx=\int_c^d\int_a^bf(x, y)\ dx\ dy$$
### Triple integral
$$\iiint_Ef(x, y, z)dV=\int_e^f\int_c^d\int_a^bf(\rho\sin\phi\cos\theta, \rho\sin\phi\sin\theta, \rho\cos\phi)\ \rho\sin\phi d\theta\ \rho d\phi\ d\rho$$
### Multiple integral
$$\int_Df(x)\ dx=\idotsint_Df(x_1,\dots,x_n)\ dx_1\dots dx_n$$
## Properties
if $x=\phi(y)$ is $\mathbf{R}^n\rightarrow\mathbf{R}^n$ and $|\frac{\partial x}{\partial y}|\neq0$ (x and y are linear-independent), 
$$\idotsint_Df(x)\ dx=\idotsint_Df(\phi(y))\ |\frac{\partial x}{\partial y}|\ dy$$
