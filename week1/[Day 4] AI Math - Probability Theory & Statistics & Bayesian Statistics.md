# [Day 4] AI Math - Probability Theory & Statistics & Bayesian Statistics

## 1. Probability Theory
* Stochastic/Random Variable
  * Discrete vs Continuous
    * Discrete
      * A discrete stochastic/random variable takes on a finite or countably infinite set of values
      $$ \mathbb{P}(X \in A) = \sum_{x \in A} P(X = x) $$
    * Continuous
      * A continuous stochastic/random variable takes on an infinite number of values within a range.
      $$ \mathbb{P}(X \in A) = \int_{A} P(x) dx $$
* Conditonal Probability
  * P(A|B) = the probability of A given B
* Monte Carlo Sampling
  * Monte Carlo methods, or Monte Carlo experiments, are a broad class of computational algorithms that rely on repeated random sampling to obtain numerical results. The underlying concept is to use randomness to solve problems that might be deterministic in principle. They are often used in physical and mathematical problems and are most useful when it is difficult or impossible to use other approaches. Monte Carlo methods are mainly used in three problem classes: optimization, numerical integration, and generating draws from a probability distribution. [1]

## 2. Statistics
* Sample vs Population
  <img src="https://b1879915.smushcdn.com/1879915/wp-content/uploads/2015/03/Population-Parameter.png?lossy=0&strip=1&webp=1" width=80%>[2]
* Maximum Likelihood Estimation (MLE)
  * In statistics, maximum likelihood estimation (MLE) is a method of estimating the parameters of an assumed probability distribution, given some observed data. [3]
  * In paractice, log likelihood is used to simplify the optimization problem and provides some computational advantages.
* Statiscal Distance
  * Total Variation Distance
  * Kullback-Leibler Divergence
  * Wasserstein Distance

## 3. Bayesian Statistics
* Conditonal Probability
  $$ P(A \cap B) = P(B)P(A|B) = P(A)P(B|A)$$
  <img src="https://statsandr.com/blog/the-7-formulas-in-probability-that-every-data-scientist-should-know_files/the-7-concepts-and-formulas-in-probability-that-every-data-scientist-should-know.png" width=80%>[4]
  * Be careful when inferring causality

<!-- Reference -->
[1]: https://en.wikipedia.org/wiki/Monte_Carlo_method

[2]: https://sixsigmadsi.com/glossary/population-parameter/

[3]: https://en.wikipedia.org/wiki/Maximum_likelihood_estimation

[4]: https://statsandr.com/blog/the-9-concepts-and-formulas-in-probability-that-every-data-scientist-should-know/