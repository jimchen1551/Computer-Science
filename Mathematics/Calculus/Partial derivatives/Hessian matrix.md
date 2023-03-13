---
Created: [[2023-01-29]]
Aliases: 
Types: Card
Tags: 
- 
---
# Hessian matrix
$$\nabla^2f(x)=\nabla(\nabla f(x))=\left(\!\begin{array}{c}\nabla(\frac{\partial f}{\partial x_1})\\\vdots\\\nabla(\frac{\partial f}{\partial x_n})\end{array}\!\right) = \begin{bmatrix}\frac{\partial^2f}{\partial x_1^2}&\dots&\frac{\partial^2f}{\partial x_n\partial x_1}\\\vdots&\ddots&\vdots\\\frac{\partial^2f}{\partial x_1\partial x_n}&\dots&\frac{\partial^2f}{\partial x_n^2}\end{bmatrix} = \begin{bmatrix}f_{x_1x_1}&\dots&f_{x_1x_n}\\\vdots&\ddots&\vdots\\f_{x_nx_1}&\dots&f_{x_nx_n}\end{bmatrix}$$
