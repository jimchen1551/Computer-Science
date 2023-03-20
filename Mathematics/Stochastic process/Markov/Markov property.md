---
Created: [[2023-03-18]]
Aliases: 
Types: Note
Tags: 
- 
---
# Markov property

$$P(X_t|X_0,\cdots X_{t-1})=P(X_t|X_{t-1})$$
$$P(X_0, \cdots, X_t)=P(X_t|X_{t-1})P(X_{t-1}|X_{t-2})\cdots P(X_1|X_0)P(X_0)$$
- first-order Markov model (memoryless)
- only depend on the previous state and not depend on further states
- [[Markov chain]]: discrete-time Markov chain
	- Time-homogeneous: only one state-transition matrix for all the time
- [[Markov process]]: continuous-time Markov chain

|                 | Discrete state space                            | Continuous state space                                |
| --------------- | ----------------------------------------------- | ----------------------------------------------------- |
| Discrete-time   | [[Markov chain]] <br>on a countable state space | [[Markov chain]]<br> on a measurable state space      |
| Continuous-time | Continuous-time <br>[[Markov process]]          | Continuous stochastic process<br>with Markov property |
