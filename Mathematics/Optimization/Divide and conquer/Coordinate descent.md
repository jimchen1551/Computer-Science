---
Created: [[2023-03-10]]
Aliases: CD
Types: Card
Tags: 
- 
---
# Coordinate descent
```Pseudocode
Initialize x_0
while no convergence do
	for i in [1, n] do
		Solve min_{x_i}f(x)
	end for
end while
```
- optimizing only one variable in each iteration