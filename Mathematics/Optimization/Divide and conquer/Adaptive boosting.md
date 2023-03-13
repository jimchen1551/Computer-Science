---
Created: [[2023-03-10]]
Aliases: AdaBoost
Types: Card
Tags: 
- 
---
# Adaptive boosting
$$L(y, F(x))=\exp(-yF(x))$$
$$F(x)=\sum_{i=1}^M\beta_if_i(x)$$
$$(\beta_i, f_i)=\arg\min_{\beta, f}\sum_{i=1}^l\exp(-y_i(F_{j-1}(x_i)+\beta f(x_i)))$$
- training weak classifiers first
- the strong classifier is the weighted sum of well-trained weak classifiers