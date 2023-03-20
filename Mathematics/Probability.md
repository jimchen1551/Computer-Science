---
Created: [[2022-10-17]]
Aliases: 
Types: Note
Tags: 
- 
---
# Probability
| Probability              | Content                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       |
| ------------------------ | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Random events            | [[Conditional probability]]<br>[[Law of total probability]]<br>[[Bayes' theorem]]<br>[[Boole's inequality]]<br>[[Bonferroni's inequality]]                                                                                                                                                                                                                                                                                                                                                                                                                                    |
| Random variables         | [[Probability mass function]]<br>[[Probability density function]]<br>[[Cumulative distribution function]]<br>[[Conjugate prior]]<br>[[Expectation]]<br>[[Variance]]<br>[[Moment]]<br>[[Law of total expectation]]<br>[[Law of total variance]]<br>[[Jensen's inequality]]<br>[[Markov's inequality]]<br>[[Chernoff's inequality]]                                                                                                                                                                                                                                             |
| Random vectors           | [[Marginal probability mass function]]<br>[[Marginal probability density function]]<br>[[Marginal cumulative distribution function]]<br>[[Conditional probability density function]]<br>[[Conditional cumulative distribution function]]<br>[[Moment-generating function]]<br>[[Covariance]]<br>[[Correlation]]<br>[[Independent and identically distributed]]                                                                                                                                                                                                                |
| Probability distribution | [[Universality of the Uniform]]<br>Discrete variables:<br>[[Uniform distribution]]<br>[[Bernoulli distribution]]<br>[[Binomial distribution]]<br>[[Multinomial distribution]]<br>[[Beta distribution]]<br>[[Geometric distribution]]<br>[[Pascal distribution]]<br>[[Poisson distribution]]<br>Continuous variables: <br>[[Uniform distribution]]<br>[[Exponential distribution]]<br>[[Gamma distribution]]<br>[[Normal distribution]]<br>[[Standard normal distribution]]<br>[[Multivariate normal distribution]]<br>[[Rayleigh distribution]]<br>[[Gaussian mixture model]] |
| Limit theorems           | [[Chebyshev's inequality]]<br>[[Law of large numbers]]<br>[[Central limit theorem]]                                                                                                                                                                                                                                                                                                                                                                                                                                                                                           |

## Axioms
1. $P(A)\geq0,\forall A\in S$
   
2. $P(S)=1$
   
3. $P(\cup_{i=1}^nA_i)=\sum_{i=1}^nP(A_i),\forall A_i \text{ mutually exclusive where }i\in [1, n]$

## Properties
1. $P(\phi)=0$
   $S\cap\phi=\phi\rightarrow\text{mutual exclusivity}$
   $S=S\cup\phi\rightarrow P(S)=P(S\cup\phi)=P(S)+P(\phi)$
   
2. $P(A)=1-P(A^C)$
   $A\cap A^C=\phi\rightarrow \text{mutual exclusivity}$
   $S=A\cup A^C\rightarrow P(S)=P(A)+P(A^C)$
   
3. $P(A)=P(A-B)+P(A\cap B)$
   $(A-B)\cap (A\cap B)=\phi\rightarrow \text{mutual exclusivity}$
   $A=(A-B)\cup (A\cap B)\rightarrow P(A)=P(A-B)+P(A\cap B)$
   
4. Principle of inclusion and exclusion (PIE)
   $P(A\cup B)=P(A)+P(B)-P(A\cap B)$
