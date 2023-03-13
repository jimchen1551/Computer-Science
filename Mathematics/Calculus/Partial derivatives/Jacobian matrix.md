---
Created: [[2023-01-29]]
Aliases: 
Types: Card
Tags: 
- 
---
# Jacobian matrix
$$y = \left(\!\begin{array}{c}y_1\\y_2\\\vdots\\y_m\end{array}\!\right)=\left(\!\begin{array}{c}f_1(x_1, x_2, \dots x_n)\\f_2(x_1, x_2, \dots x_n)\\\vdots\\f_m(x_1, x_2, \dots x_n)\end{array}\!\right)$$
$$\frac{\partial y}{\partial x}=\left(\!\begin{array}{c}\nabla y_1^T\\\nabla y_2^T\\\vdots\\\nabla y_m^T\end{array}\!\right)=\begin{bmatrix}\frac{\partial y_1}{\partial x_1}&\frac{\partial y_1}{\partial x_2}&\dots&\frac{\partial y_1}{\partial x_n}\\\frac{\partial y_2}{\partial x_1}&\frac{\partial y_2}{\partial x_2}&\dots&\frac{\partial y_2}{\partial x_n}\\\vdots&\vdots&\ddots&\vdots\\\frac{\partial y_m}{\partial x_1}&\frac{\partial y_m}{\partial x_2}&\dots&\frac{\partial y_m}{\partial x_n}\end{bmatrix}=\begin{bmatrix}y_{1x_1}&y_{1x_2}&\dots&y_{1x_n}\\y_{2x_1}&y_{2x_2}&\dots&y_{2x_n}\\\vdots&\vdots&\ddots&\vdots\\y_{mx_1}&y_{mx_2}&\dots&y_{mx_n}\end{bmatrix}$$
