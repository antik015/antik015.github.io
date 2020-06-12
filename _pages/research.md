---
layout: archive
title: "Research interests"
permalink: /research/
author_profile: true
---

* Shrinkage priors
* Scalable Bayes
* High dimensional data
* Binary/Count data
* Ecological applications


## Shrinkage priors/Scalable Bayes
* Shrinkage priors [(Polson & Scott, 2010)](https://faculty.chicagobooth.edu/nicholas.polson/research/papers/Bayes1.pdf) have been shown to have nice properties in high dimensional problems. They often outperform frquentist regularization methods [(Bhattachrya, Chakraborty & Mallick, 2016)](https://arxiv.org/abs/1506.04778) and can automatically provide uncertainty quantifications. But standard Markov chain 
Monte Carlo algorithms to sample from the posterior distribution are very scale as a cubic with the dimension of the parameter limiting
the applications of these priors in many applications, for example, in GWAS studies. In [Bhattachrya, Chakraborty & Mallick (2016)](https://arxiv.org/abs/1506.04778), we propose a novel algorithm to sample from the posterior that scales linearly with the dimension. 
Although the algorithm is oroginally developed in a high dimensional regression setting, the same principle can be applied in other 
high dimensional problems such as covariance matrix estimation, factor models, dictionary learning etc. The following image shows the
computing time of an algorithm (black solid line) proposed in [(Rue, 2001)](https://rss.onlinelibrary.wiley.com/doi/abs/10.1111/1467-9868.00288) and that of the proposed algorithm (black dotted line) in logarithmic scale. Clearly, the gains are huge when the dimension (p) increases.
![](https://github.com/antik015/antik015.github.io/blob/master/images/time_comp_resized.png?raw=true)



## Scalable density estimation
* Dirichlet process priors are one of the most popular Bayesian methods for nonparametric density estimation. While researchers have proposed many algorithms for posterior computation, they involve a delicate trade off between good mixing and computation time. Additionally, these methods are not suitable for high dimensional data which lie on lower dimensional manifolds such as data on galaxies, stars etc. In [Chattopadhyay, Chakraborty & Dunson (2020+)](https://arxiv.org/abs/2003.07953) we propose a pseudo Bayes approach combining the algorithmic simplicity of nearest neighbor methods and statistical versataility of Dirichlet process. The method involves in partititoning the data according to nearest neighborhoods and fitting a kernel, typicallu Gaussian, within each neighborhood. The fixed partitioning results in
huge gains in computation time while the final mixture model formulation enables the method to efficiently estimate a wide range of densities. The runtimes of a standard Dirichlet process (DP) mixture model sampler versus the nearest neighbor alternative (NNDP) proposed is shown below. 

![](https://github.com/antik015/antik015.github.io/blob/master/images/runtime_mvt_resized.png?raw=true)

