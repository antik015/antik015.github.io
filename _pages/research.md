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
1. Shrinkage priors [(Polson & Scott, 2010)](https://faculty.chicagobooth.edu/nicholas.polson/research/papers/Bayes1.pdf) have been shown to have nice properties in high dimensional problems. They often outperform frquentist regularization methods [(Bhattachrya, Chakraborty & Mallick, 2016)](https://arxiv.org/abs/1506.04778) and can automatically provide uncertainty quantifications. But standard Markov chain 
Monte Carlo algorithms to sample from the posterior distribution are very scale as a cubic with the dimension of the parameter limiting
the applications of these priors in many applications, for example, in GWAS studies. In [Bhattachrya, Chakraborty & Mallick (2016)](https://arxiv.org/abs/1506.04778), we propose a novel algorithm to sample from the posterior that scales linearly with the dimension. 
Although the algorithm is oroginally developed in a high dimensional regression setting, the same principle can be applied in other 
high dimensional problems such as covariance matrix estimation, factor models, dictionary learning etc. 

[!Time comparison](https://github.com/antik015/antik015.github.io/blob/master/files/time_comp.pdf?raw=true)

