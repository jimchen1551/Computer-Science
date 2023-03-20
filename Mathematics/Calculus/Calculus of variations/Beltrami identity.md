---
Created: [[2023-03-19]]
Aliases: 
Types: Card
Tags: 
- 
---
# Beltrami identity
$$F-y'\frac{\partial F}{\partial y'}=C$$
- applied when [[functional]] $F(x, y, y')$ doesn't explicitly on $x$
## Derivation
1. Multiply both sides of the [[Euler-Lagrange equation]] by $y'$. 
   $$y'\frac{\partial F}{\partial y}-y'\frac{d}{dx}(\frac{\partial F}{\partial y'})=0$$
2. Consider the [[differential]], $$dF=[\frac{\partial F}{\partial x}+\frac{\partial F}{\partial y}y'+\frac{\partial F}{\partial y'}y'']dx$$
   Then, $$y'\frac{\partial F}{\partial y}=\frac{dF}{dx}-\frac{\partial F}{\partial x}-\frac{\partial F}{\partial y'}y''$$
3. Subtrate 2 into 1, $$\frac{dF}{dx}-\frac{\partial F}{\partial x}-[y''\frac{\partial F}{\partial y'}+y'\frac{d}{dx}(\frac{\partial F}{\partial y'})]=0$$$$\frac{dF}{dx}-\frac{\partial F}{\partial x}-\frac{d}{dx}(y'\frac{\partial F}{\partial y'})=0$$$$\frac{dF}{dx}-\frac{d}{dx}(y'\frac{\partial F}{\partial y'})=\frac{\partial F}{\partial x}$$$$\frac{d}{dx}(F-y'\frac{\partial F}{\partial y'})=\frac{\partial F}{\partial x}=0$$So, $$F-y'\frac{\partial F}{\partial y'}=C$$