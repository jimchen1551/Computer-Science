---
Created: [[2023-01-28]]
Aliases: partial derivative
Types: Card
Tags: 
- 
---
# Partial derivatives
## Definition
### Partial change in variables
$$\partial x_i = dx_i$$
$$\partial f(x) = f(:, x_i+\partial x_i,:)-f(:, x_i, :)$$
### Partial derivative
$$f_{x_i}=\frac{\partial f}{\partial x_i}=\frac{f(:, x_i+\partial x_i,:)-f(:, x_i, :)}{\partial x_i}$$
$$\partial_{x_i}f=f_{x_i}\cdot dx_i$$
### Higher-order partial derivative
$$f_{xy}=\frac{\partial}{\partial y}(\frac{\partial f}{\partial x})=\frac{\partial^2f}{\partial y\partial x}$$
### Other derivatives

| Other derivatives          | Notation                        | Definition                                                  |
| -------------------------- | ------------------------------- | ----------------------------------------------------------- |
| [[Differential]]           | $df$                            | $\sum f_x\cdot dx$                                          |
| [[Gradient]]               | $\nabla f$                      | $(f_{x_1}, f_{x_2}, \dots, f_{x_n})^T$                      |
| [[Directional derivative]] | $\nabla_vf$                     | $v\cdot \nabla f$                                           |
| [[Hessian matrix]]         | $\nabla^2 f$ / $H(f)$           | $(\nabla f_{x_1}, \nabla f_{x_2}, \dots, \nabla f_{x_n})^T$ |
| [[Jacobian matrix]]        | $\frac{\partial f}{\partial x}$ | $(\nabla y_1^T, \nabla y_2^T, \dots, \nabla y_m^T)^T$       |

## Properties
1. $$f_{xy}=f_{yx}$$
2. $$\frac{df}{dt}=\frac{\partial f}{\partial x}\cdot\frac{dx}{dt}+\frac{\partial f}{\partial y}\cdot\frac{dy}{dt}$$
3. $$y=Ax\Rightarrow\frac{\partial y}{\partial x}=A;\ \nabla a_i^Tx=a_i$$
4. $$y=x^TAx=\sum_{p=1}^n\sum_{q=1}^na_{pq}x_px_q$$$$\frac{\partial y}{\partial x_i}=\sum_{p=1}^na_{pi}x_p+\sum_{q=1}^na_{iq}x_q=a_{:i}x+a_{i:}^Tx\Rightarrow\nabla x^TAx=(A^T+A)x$$
5. $$\nabla^2x^TAx=\nabla(\nabla x^TAx)=\nabla(A^T+A)x=A+A^T$$
6. $$\nabla_xz=\left(\!\begin{array}{c}\sum_{j=1}^m\frac{\partial z}{\partial y_j}\frac{\partial y_j}{\partial x_1}\\\sum_{j=1}^m\frac{\partial z}{\partial y_j}\frac{\partial y_j}{\partial x_2}\\\vdots\\\sum_{j=1}^m\frac{\partial z}{\partial y_j}\frac{\partial y_j}{\partial x_n}\end{array}\!\right)=\begin{bmatrix}\frac{\partial y_1}{\partial x_1}&\frac{\partial y_2}{\partial x_1}&\dots&\frac{\partial y_m}{\partial x_1}\\\frac{\partial y_1}{\partial x_2}&\frac{\partial y_2}{\partial x_2}&\dots&\frac{\partial y_m}{\partial x_2}\\\vdots&\vdots&\ddots&\vdots\\\frac{\partial y_1}{\partial x_n}&\frac{\partial y_2}{\partial x_n}&\dots&\frac{\partial y_m}{\partial x_n}\end{bmatrix}\left(\!\begin{array}{c}\frac{\partial z}{\partial y_1}\\\frac{\partial z}{\partial y_2}\\\vdots\\\frac{\partial z}{\partial y_m}\end{array}\!\right)=(\frac{\partial y}{\partial x})^T\nabla_yz$$
7. if $y=\phi(x)$ is $\mathbf{R}^n\rightarrow\mathbf{R}^n$ and $|\frac{\partial y}{\partial x}|\neq0$ (x and y are linear-independent), 
   1. $x=\phi^{-1}(y)$ exists
   2. $\nabla y_i(x)^T\frac{\partial x}{\partial y_i}=1$
   3. $\nabla y_i(x)^T\frac{\partial x}{\partial y_j}=0$
      $$\Rightarrow\frac{\partial y}{\partial x}\cdot \frac{\partial x}{\partial y}=I_{n\times n}$$
## Partial differential equation
- [[Heat equation]]
- [[Wave equation]]
- [[Transport equation]]
- [[Burgers equation]]
- [[Laplace equation]]
## Mathematical optimization
- [[Lagrange multiplier]]
