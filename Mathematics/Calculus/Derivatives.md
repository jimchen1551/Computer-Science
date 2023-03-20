---
Created: [[2023-01-27]]
Aliases: derivative
Types: Card
Tags: 
- 
---
# Derivatives
## Definition
### Change in variables
$$\Delta x=x'-x_0$$
$$\Delta f(x)=f(x')-f(x_0)$$
### Differential change in variables
- taking [[Limits]] on change in variables
$$dx=\lim_{\Delta x\rightarrow0}\Delta x=(x+dx)-(x)$$
$$df(x)=\lim_{\Delta x\rightarrow0}\Delta f(x)=f(x+dx)-f(x)$$
### Derivative
$$f'(x)=\frac{df(x)}{dx}=\lim_{\Delta x\rightarrow0}\frac{\Delta f(x)}{\Delta x}=\frac{f(x+dx)-f(x)}{(x+dx)-(x)}$$
$$df(x)=f'(x)\cdot dx$$
### Higher order derivative
$$f^{(n)}(x)=\frac{d^nf(x)}{dx^n}=\frac{df^{(n-1)}(x)}{dx}$$
## Properties
1. $$\frac{dc}{dx}=0$$
2. $$\frac{d[c\cdot f(x)]}{dx}=c\cdot\frac{df(x)}{dx}$$
3. $$\frac{dx^n}{dx}=nx^{n-1}$$
4. $$\frac{d[f(x)\pm g(x)]}{dx}=\frac{df(x)}{dx}\pm\frac{dg(x)}{dx}$$
5. $$\frac{d[f(x)\cdot g(x)]}{dx}=\frac{df(x)}{dx}\cdot g(x)+f(x)\cdot\frac{dg(x)}{dx}$$
6. $$\frac{d[f(g(x))]}{dx}=\frac{df(g(x))}{dg(x)}\cdot\frac{dg(x)}{dx}$$
## Rules and theorems
- [[Extreme value theorem]]
- [[Mean value theorem]]
- [[Newton's method]]
