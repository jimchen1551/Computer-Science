---
Created: [[2023-03-10]]
Aliases: MAP, MAPE
Types: Card
Tags: 
- 
---
# Maximum a posteriori
$$\mathbf{M}(q)=\arg\max_{l\in levels(t)}P(t=l|q[1],\dots,q[m])$$
- aka **MAP** prediction
- returning the target level with the highest posterior probability given the state of the descriptive features in the query
- more accurate if the prior probability is known
$$P(t=l|q[1],\dots,q[m])=\eta\cdot P(q[1],\dots,q[m]|t=l)P(t=l)$$
