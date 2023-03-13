---
Created: [[2023-03-10]]
Aliases: 
Types: Card
Tags: 
- 
---
# Gaussian integral
$$\int_{-\infty}^{\infty}e^{-x^2}dx=\sqrt{\int_{-\infty}^{\infty}e^{-x^2}dx\int_{-\infty}^{\infty}e^{-y^2}dy}$$
$$=\sqrt{\int_{-\infty}^{\infty}\int_{-\infty}^{\infty}e^{-x^2}e^{-y^2}\ dx\ dy}=\sqrt{\int_{-\infty}^{\infty}\int_{-\infty}^{\infty}e^{-(x^2+y^2)}\ dx\ dy}$$
from Cartesian coordinates to polar coordinates
$$=\sqrt{\int_{0}^{2\pi}\int_{0}^{\infty}e^{-r^2}\ dr\ rd\theta}=\sqrt{\frac{1}{2}\int_{0}^{2\pi}\int_{0}^{\infty}e^{-r^2}\ dr^2\ d\theta}$$
$$=\sqrt{-\frac{2\pi}{2}\int_{0}^{\infty}de^{-r^2}}=\sqrt{\pi}$$
