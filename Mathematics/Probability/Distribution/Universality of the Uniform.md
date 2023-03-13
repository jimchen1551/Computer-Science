---
Created: [[2023-03-10]]
Aliases: probability integral transform
Types: Card
Tags: 
- 
---
# Universality of the Uniform
## for random variables
$$Y=g(X);\ X=g^{-1}(Y)$$
$$F_Y(y)=p(Y\leq y)=p(g(X)\leq y)=p(X\leq g^{-1}(y))=F_X(g^{-1}(y))$$
$$f_Y(y)=\frac{dF_X(g^{-1}(y))}{dy}=\frac{dF_X(g^{-1}(y))}{g^{-1}(y)}\frac{g^{-1}(y)}{dy}=f_X(g^{-1}(y))\cdot g^{-1}(y)'$$
## for random vectors
$$Y=g(X);\ X=g^{-1}(Y)$$
$$F_Y(y)=p(Y\leq y)=p(g(X)\leq y)=p(X\leq g^{-1}(y))=\idotsint f_X(x_1, \dots, x_n)dx_1\dots dx_n$$
$$f_Y(y)=f_X(g^{-1}(y))\cdot|\det(\frac{\partial g^{-1}(y)}{\partial y})|$$
