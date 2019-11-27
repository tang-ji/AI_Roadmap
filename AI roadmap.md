# Probability

## Basic

### 	Basic Term

- [x] Expectation

- [x] Mean - Median

- [x] Variance - Bias

- [x] Covariance - Correlation

  #### 	Distance

  - [ ] Manhattan

    $L^1$ distance

    [the taxicab distance](https://en.wikipedia.org/wiki/Taxicab_geometry) between $(p_{1},p_{2})$ and $(q_{1},q_{2})$ is $ |p_{1}-q_{1}|+|p_{2}-q_{2}|$.

  - [ ] Euclidean

    $L^2$ distance

  - [ ] Mahalanobis

    The **Mahalanobis distance** is a measure of the distance between a point P and a distribution D. It is a multi-dimensional generalization of the idea of measuring how many standard deviations away P is from the mean of D. This distance is zero if P is at the mean of D, and grows as P moves away from the mean along each principal component axis.

    The Mahalanobis distance of an observation $\vec {x}=(x_{1},x_{2},x_{3},\dots ,x_{N})^{T}$ from a set of observations with mean $\vec {\mu }=(\mu _{1},\mu _{2},\mu _{3},\dots ,\mu _{N})^{T}$ and covariance matrix *S* is defined as:

    $ D_{M}({\vec {x}})=\sqrt {({\vec {x}}-{\vec {\mu }})^{T}S^{-1}({\vec {x}}  -{\vec {\mu }})} $

    Mahalanobis distance can also be defined as a dissimilarity measure between two random vectors $\vec {x}$ and $\vec {y}$ of the same distribution with the covariance matrix *S*.

    If the covariance matrix is diagonal, then the resulting distance measure is called a *standardized Euclidean distance*:

    $d(\vec{x},\vec{y})= \sqrt{\sum_{i=1}^N  {(x_i - y_i)^2 \over s_{i}^2}}$

  - [ ] Correlation

  ### Sample Space

  ### Random Variable

  ### Probability Distribution

  - [x] Uniform
  
  - [x] Gaussian
  
  - [x] Bernoulli
  
    $\Pr(X=1)=p=1-\Pr(X=0)=1-q$
  
  - [x] Binomial
  
     $f(k,n,p)=\Pr(k;n,p)=\Pr(X=k)={\binom {n}{k}}p^{k}(1-p)^{n-k}$
  
    Mean: $np$  Variance: $np(1-p)$
  
  - [x] MultiNomial
  
  - [ ] Categorical
  
  - [ ] Dirichlet

  - [ ] Beta

  - [ ] Gamma
  
  - [ ] Exponential
  
  - [ ] Poisson
  
  - [ ] Chi-squared
  
  - [ ] Student-t 
  
  - [ ] t-SNE
  
  - [ ] Central Limit Theorem
  
  - [ ] degree of freedom
  
  - [ ] GMM - EM algorithm
  
  - [ ] PDF
  
  - [ ] CDF
  
  ### Independence
  
  ### Conjucate

## Sampling

- [x] Monte Carlo Method

- [x] Markov Chain

  Reducibility:  $\Pr(X_{n_{ij}}=j\mid X_{0}=i)=p_{ij}^{(n_{ij})}>0$

  Stationary distribution: $\pi \mathbf {P} =\pi$

- [x] MCMC

- [ ] Gibbs

   to sample $x_{j}^{(i+1)}$, we update it according to the distribution specified by $p\left(x_{j}^{(i+1)}|x_{1}^{(i+1)},\dots ,x_{j-1}^{(i+1)},x_{j+1}^{(i)},\dots ,x_{n}^{(i)}\right)$

## Information Theory

- [ ] KL Divergence

   the Kullback–Leibler divergence of $Q$ from $P$ is defined:  $D_{\text{KL}}(P\parallel Q)=\sum_{x\in {\mathcal {X}}}P(x)\log \left({\frac {P(x)}{Q(x)}}\right)$

- [ ] Cross Entropy

   The cross entropy of the distribution $q$ relative to a distribution $p$:  

  $H(p,q)=-\operatorname {E} _{p}[\log q]=\sum_{x\in {\mathcal {X}}}p(x)\log q(x) = H(p) + D_{KL}(p\parallel q)$ 

- [ ] Shannon Entropy

- [ ] Uncertainty

## Model

## Baysian







