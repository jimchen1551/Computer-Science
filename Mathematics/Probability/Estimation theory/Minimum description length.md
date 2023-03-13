---
Created: [[2023-03-10]]
Aliases: MDL
Types: Card
Tags: 
- 
---
# Minimum description length
$$h_{MDL}=\arg\min_{h\in H}L_{C1}(h)+L_{C2}(D|h)$$
, where $L_C(x)$ is the description length of $x$ under coding $C$; 
$L_{C1}(h)=$ # bits to describe a [[Decision tree]] $h$; 
$L_{C2}(D|h)=$ # bits to describe training data $D$ given $h$; 
- aka **MDL** principle
- preferring the simplest hypothesis
