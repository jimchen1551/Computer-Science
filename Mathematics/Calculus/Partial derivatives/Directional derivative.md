---
Created: [[2023-01-29]]
Aliases: 
Types: Card
Tags: 
- 
---
# Directional derivative
$$\nabla_vf=\frac{df_v}{dt}=\lim_{t\rightarrow0}\frac{f(x+tv)-f(x)}{t}$$
$$df_v=f\left(\!\begin{array}{c}x_1+dv_1\\\vdots\\x_n+dv_n\end{array}\!\right)-f\left(\!\begin{array}{c}x_1\\\vdots\\x_n\end{array}\!\right)=\sum_{i\in[1,n]}v_i\cdot\partial_{x_i}f=\sum_{i\in[1,n]}\frac{\partial f}{\partial x_i}\cdot v_idx_i=(\nabla f)^Tvdt$$
$$\frac{df_v}{dt}=v\cdot\nabla f$$
