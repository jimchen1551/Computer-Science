---
Created: [[2023-03-19]]
Aliases: 
Types: Card
Tags: 
- 
---
# Euler-Lagrange equation
$$\frac{\partial F}{\partial y}-\frac{d}{dx}(\frac{\partial F}{\partial y'})=0$$
## Derivation
1. Find $y=f(x)$ such that the [[Functional]] $$I=\int_{x_1}^{x_2}F(x, y, y')dx$$ is stationary.
   - Boundary conditions: $y_1=f(x_1)$ and $y_2=f(x_2)$
2. Define $$\bar{y}(x)=y(x)+\epsilon\eta(x)$$, where $\eta(x)$ is an arbitrary function that is asserted to be $\eta(x_1)=\eta(x_2)=0$. 
   - $\bar{y}$ satisfies the same boundary conditions as $y$. 
   - $\bar{y}$ represents a family of curves. 
3. Find the particular $\bar{y}$ which makes $$I(\epsilon)=\int_{x_1}^{x_2}F(x, \bar{y}, \bar{y}')dx$$ stationary. 
   - Since $I$ depends only on $\epsilon$, to make $I$ stationary, according to [[Fermat's theorem (stationary point)]], $$\left.\frac{dI}{d\epsilon}\right|_{\epsilon=0}=0$$$$\int_{x_1}^{x_2}F(x, \bar{y}, \bar{y}')dx=0$$$$\int_{x_1}^{x_2}\left.\frac{\partial}{\partial\epsilon}F(x, \bar{y}, \bar{y}')\right|_{\epsilon=0}dx=0$$$$\int_{x_1}^{x_2}\left.\frac{\partial F}{\partial \bar{y}}\frac{\partial \bar{y}}{\partial \epsilon}+\frac{\partial F}{\partial \bar{y}'}\frac{\partial \bar{y}'}{\partial \epsilon}\right|_{\epsilon=0}dx=0$$$$\int_{x_1}^{x_2}\left.\frac{\partial F}{\partial \bar{y}}\eta+\frac{\partial F}{\partial \bar{y}'}\eta'\right|_{\epsilon=0}dx=0$$According to [[Integration by parts]], $$\int_{x_1}^{x_2}\frac{\partial F}{\partial \bar{y}'}\eta'dx=\int_{x_1}^{x_2}\frac{\partial F}{\partial \bar{y}'}d\eta=\int_{x_1}^{x_2}d(\frac{\partial F}{\partial \bar{y}'}\eta)-\int_{x_1}^{x_2}\eta\  d(\frac{\partial F}{\partial \bar{y}'})$$$$=\frac{\partial F}{\partial \bar{y}'}\left.\Delta\eta\right|_{x_1}^{x_2}-\int_{x_1}^{x_2}\eta \frac{d}{dx}(\frac{\partial F}{\partial \bar{y}'})dx=0-\int_{x_1}^{x_2}\eta \frac{d}{dx}(\frac{\partial F}{\partial \bar{y}'})dx$$So, $$\int_{x_1}^{x_2}\left.\eta[\frac{\partial F}{\partial \bar{y}}-\frac{d}{dx}(\frac{\partial F}{\partial \bar{y}'})]\right|_{\epsilon=0}dx=0$$And because if $\epsilon=0$, $y=\bar{y}$, $$\int_{x_1}^{x_2}\eta[\frac{\partial F}{\partial y}-\frac{d}{dx}(\frac{\partial F}{\partial y'})]dx=0$$Finally, because $\eta$ is an arbitrary function, the only way to get these results is $$\frac{\partial F}{\partial y}-\frac{d}{dx}(\frac{\partial F}{\partial y'})=0$$
