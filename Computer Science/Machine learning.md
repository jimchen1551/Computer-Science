---
Created: [[2022-10-17]]
Aliases: ML
Types: Note
Tags: 
- 
---
# Machine learning
- an automatic process that extracts patterns from data (or past experiences)
- A computer program is said to learn from **experience** ***E*** with respect to some class of **tasks** ***T*** and **performance** measure ***P***, if its performance at tasks in *T*, as measured by  *P*, improves with *E*. 

## Christopher Bishop

| [[Data]]                                              | Content                                                                       |
| ----------------------------------------------------- | ----------------------------------------------------------------------------- |
| [[Independent and identically distributed\|iid]] data | Regression models<br>Classification models                                    |
| sequential data                                       | [[Markov models]]<br>[[Hidden Markov models]]<br>[[Linear Dynamical systems]] |

| Estimations                   | Content                                                                                                                                                                                                          |
| ----------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| [[Parameter estimation]]      | [[Maximum likelihood]]: <br>[[Feedforward network]], [[Least squared error]]<br>[[Maximum a posteriori]]: <br>[[Regularization]], [[Regularized least squared error]]<br>[[Bayesian estimation]]                 |
| [[Non-parametric estimation]] | [[Nearest neighbor]]: <br>[[k-nearest neighbor]], [[k-means]]<br>[[Kernel methods]]: <br>[[Gaussian process]], [[Support vector machine]]<br>[[Spectral methods]]:<br>[[Spectral clustering]], [[Graph network]] |

| Models           | Content                                                                                                                                                                                                                                                               |
| ---------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| [[Probability]]  | [[Conjugate prior]]<br>[[Exponential family]]<br>[[Binomial distribution]] ←→ [[Beta distribution]]<br>[[Multinomial distribution]] ←→ [[Dirichlet distribution]]<br>[[Normal distribution\|Gaussian distribution]] ←→ [[Normal distribution\|Gaussian distribution]] |
| Linear models    | [[Least squared error]]<br>[[Regularized least squared error]]<br>[[Linear regression]]<br>[[Bayesian linear regression]]<br>[[Logistic regression]]<br>[[Bayesian logistic regression]]                                                                              |
| Mixture models   | [[Gaussian mixture model]]<br>[[Expectation maximization]]                                                                                                                                                                                                            |
| Graphical models | [[Bayesian networks]]<br>[[Markov random fields]]                                                                                                                                                                                                                     |
| Combining models | [[Bayesian model averaging]]<br>[[Committees]]<br>[[Boosting]]<br>[[Tree-based models]]<br>[[Conditional mixture models]]                                                                                                                                             |

| [[Latent variables]]      | Content                                                                                                                                                                                                                          |
| ------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Discrete                  | [[K-means]]<br>[[Expectation maximization]]                                                                                                                                                                                      |
| Continuous                | [[Principal component analysis]]<br>[[Independent component analysis]]<br>[[Linear discriminant analysis]]<br>[[Locally linear embedding]]<br>[[Stochastic neighbor embedding]]<br>[[Autoassociative neural networks]]           |
| [[Approximate inference]] | [[Variational inference]]<br>[[Local variational methods]]<br>[[Variational linear regression]]<br>[[Variational logistic regression]]<br>[[Expectation propagation]]                                                            |
| [[Sampling methods]]      | [[Rejection sampling]]<br>[[Adaptive rejection sampling]]<br>[[Importance sampling]]<br>[[Sampling-importance-resampling]]<br>[[Markov Chain Monte Carlo]]<br>[[Gibbs sampling]]<br>[[Slice sampling]]<br>[[Hybrid Monte Carlo]] |

=====================================================

| Machine learning              | Content                                                                                                                                                                                                                                                                              |
| ----------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| [[Parameter estimation]]      | [[Maximum likelihood]]<br>[[Maximum a posteriori]]<br>[[Bayesian estimation]]                                                                                                                                                                                                        |
| [[Non-parametric estimation]] | [[Nearest neighbor]]<br>[[Kernel methods]]: <br>[[Kernel density estimation]]<br>[[Mean shift]]<br>[[Radial basis function networks]]<br>[[Gaussian process]]<br>[[Maximum margin classifiers]]<br>[[Support vector machine]]<br>[[Relevance vector machine]]                        |
| Approximate inference         | [[Variational inference]]<br>[[Local variational methods]]<br>[[Variational linear regression]]<br>[[Variational logistic regression]]<br>[[Expectation propagation]]                                                                                                                |
| [[Sampling methods]]          | [[Rejection sampling]]<br>[[Adaptive rejection sampling]]<br>[[Importance sampling]]<br>[[Sampling-importance-resampling]]<br>[[Markov Chain Monte Carlo]]<br>[[Gibbs sampling]]<br>[[Slice sampling]]<br>[[Hybrid Monte Carlo]]                                                     |
| [[Latent variables]]          | Discrete: <br>[[Expectation maximization]]<br>Continuous: <br>[[Principal component analysis]]<br>[[Independent component analysis]]<br>[[Linear discriminant analysis]]<br>[[Locally linear embedding]]<br>[[Stochastic neighbor embedding]]<br>[[Autoassociative neural networks]] |
| Linear models                 | [[Least squared error]]<br>[[Regularized least squared error]]<br>[[Linear regression]]<br>[[Bayesian linear regression]]<br>[[Logistic regression]]<br>[[Bayesian logistic regression]]                                                                                             |
| Mixture models                | [[Gaussian mixture model]]<br>[[Expectation maximization]]                                                                                                                                                                                                                           |
| Graphical models              | [[Bayesian networks]]<br>[[Markov random fields]]                                                                                                                                                                                                                                    |
| Combining models              | [[Bayesian model averaging]]<br>[[Committees]]<br>[[Boosting]]<br>[[Tree-based models]]<br>[[Conditional mixture models]]                                                                                                                                                            |
| Sequential data               | [[Markov models]]<br>[[Hidden Markov models]]<br>[[Linear Dynamical systems]]                                                                                                                                                                                                        |

## Wen-Chen Chiu

| Machine Learning                                           | Content                                                                                                                                                                                                                                                                                                                                                                                                                                              |
| ---------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Supervised** learning<br>(aka **Discriminative** models) | Regression: <br>[[Gaussian process]]<br>Classification: <br>[[Support vector machine]]                                                                                                                                                                                                                                                                                                                                                               |
| **Unsupervised** learning<br>(aka **Generative** models)   | Clustering: <br>[[K-means]]<br>[[Nearest neighbor]]<br>[[Expectation maximization]]<br>[[Spectral clustering]]<br>[[Hierarchical clustering]]<br>[[Density-based spatial clustering of applications with noise]]<br>Embedding: <br>(aka dimensionality reduction)<br>[[Principal component analysis]]<br>[[Independent component analysis]]<br>[[Linear discriminant analysis]]<br>[[Locally linear embedding]]<br>[[Stochastic neighbor embedding]] |

## John Kelleher
- [[Data]]
	- [[Analytics Base Table]]
	- [[Data Quality Report]]
	- [[Data Quality Issues]]
	- [[Data Visualization]]
	- [[Data Preparation]]

| Classes                        | Techniques                                                                                     | Model                                                                                                                           |
| ------------------------------ | ---------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------- |
| [[Information-based learning]] | [[Information theory]]<br>[[Information gain]]<br>[[Information gain ratio]]<br>[[Gini index]] | [[Decision tree]]<br>[[Regression tree]]<br>[[ID3]]<br>[[CART]]                                                                 |
| [[Similarity-based learning]]  | [[Feature space]]<br>[[Distance matric]]<br>[[Feature selection]]                              | [[Nearest neighbor]]<br>[[k-nearest neighbor]]                                                                                  |
| [[Probability-based learning]] | [[Probability]]<br>[[Joint probability distribution]]<br>[[Smoothing]]                         | [[Naive Bayes model]]<br>[[Bayesian networks]]                                                                                   |
| [[Error-based learning]]       | [[Error function]]<br>[[Error surface]]<br>[[Gradient descent]]                                | [[Linear regression]]<br>[[Logistic regression]]<br>[[Multivariable linear regression]]<br>[[Multinominal logistic regression]] |

## Reference book
- Pattern Recognition and Machine Learning by Christopher M. Bishop
- Fundamentals of Machine Learning for Predictive Data Analytics by John D. Kelleher, Brian Mac Namee, and Aoife D'Arcy





