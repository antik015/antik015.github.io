---
layout: archive
title: "Research"
permalink: /research/
author_profile: true
---

<style>
.research-intro {
  max-width: 760px;
  margin-bottom: 2.2rem;
}

.research-item {
  display: grid;
  grid-template-columns: minmax(0, 1fr) minmax(0, 1fr);
  gap: 2.2rem;
  align-items: center;
  padding: 2.4rem 0;
  border-top: 1px solid #d9d4c8;
}

.research-item:first-of-type {
  border-top: 0;
  padding-top: 0.5rem;
}

.research-item--reverse .research-visual {
  order: 2;
}

.research-item--reverse .research-copy {
  order: 1;
}

.research-copy h2 {
  margin-top: 0;
  padding-bottom: 0;
  border-bottom: 0;
  font-size: 1.55rem;
}

.research-copy p {
  margin-bottom: 0.85rem;
}

.research-links {
  margin-top: 1rem;
  font-size: 0.88rem;
}

.research-visual {
  margin: 0;
}

.research-visual img {
  width: 100%;
  height: auto;
  display: block;
  background: #fff;
  border: 1px solid #ded9cf;
}

.research-visual iframe {
  width: 100%;
  height: 340px;
  display: block;
  border: 1px solid #ded9cf;
  background: #fff;
}

.research-visual--triptych {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  gap: 0.35rem;
}

.research-visual--pair {
  display: grid;
  grid-template-columns: 1fr 1fr;
  gap: 0.35rem;
}

.research-caption {
  margin-top: 0.55rem;
  color: #777168;
  font-size: 0.76rem;
  line-height: 1.4;
}

@media (max-width: 800px) {
  .research-item {
    grid-template-columns: 1fr;
    gap: 1.2rem;
  }

  .research-item--reverse .research-visual,
  .research-item--reverse .research-copy {
    order: initial;
  }

  .research-visual {
    order: 1 !important;
  }

  .research-copy {
    order: 2 !important;
  }

  .research-visual iframe {
    height: 430px;
  }
}
</style>

<p class="research-intro">My research develops statistical and computational methodology for complex, high-dimensional probability models, with an emphasis on Bayesian inference, graphical models, and Monte Carlo methods.</p>

<div class="research-item">
  <figure class="research-visual">
    <img src="https://raw.githubusercontent.com/antik015/sFO-MLA/main/Reproducibility/W2_30.png" alt="Sliced Wasserstein distance comparison for stochastic first-order Mirror Langevin sampling">
    <figcaption class="research-caption">Two-loop sFO-MLA compared with fixed-step implementations through sliced Wasserstein distance.</figcaption>
  </figure>
  <div class="research-copy">
    <h2>Stochastic Mirror Langevin Sampling</h2>
    <p>Stochastic first-order Mirror Langevin algorithms enable sampling from constrained distributions when gradients are available only through noisy estimates. A warm-started two-loop scheme progressively decreases the step size, allowing the sampler to move beyond the discretization error floor of fixed-step implementations while retaining efficient mixing.</p>
    <p class="research-links"><a href="https://arxiv.org/abs/2610.09402">Paper</a> &middot; <a href="https://github.com/antik015/sFO-MLA">Code</a></p>
  </div>
</div>

<div class="research-item research-item--reverse">
  <figure class="research-visual">
    <iframe src="https://arxiv.org/pdf/2610.09070#page=19&zoom=page-width" title="Covariate-dependent ordinal preference networks from the CR-MRF paper"></iframe>
    <figcaption class="research-caption">Fitted MovieLens edge networks under the joint MLE across gender and age groups (Figure S1).</figcaption>
  </figure>
  <div class="research-copy">
    <h2>Covariate-Dependent Graphical Models for Ordinal Preferences</h2>
    <p>Covariate-dependent consecutive-ratio Markov random fields provide a joint model for multivariate ordinal preferences. The framework preserves the original ordinal ratings while allowing both marginal preference effects and dependence among items to vary with covariates, with direct connections to classical pairwise-comparison and ranking models.</p>
    <p class="research-links"><a href="https://arxiv.org/abs/2610.09070">Paper</a> &middot; <a href="https://github.com/antik015/CR-MRF-ordinal-preference-data">Code</a></p>
  </div>
</div>

<div class="research-item">
  <figure class="research-visual">
    <div class="research-visual--triptych">
      <img src="https://arxiv.org/html/2404.17763v3/Isingp20_theta0.png" alt="True Ising parameter matrix">
      <img src="https://arxiv.org/html/2404.17763v3/Isingp20_theta_lasso.png" alt="Penalized maximum likelihood estimate of Ising parameter matrix">
      <img src="https://arxiv.org/html/2404.17763v3/Isingp20_theta_plasso.png" alt="Penalized maximum pseudo-likelihood estimate of Ising parameter matrix">
    </div>
    <figcaption class="research-caption">True interaction structure and corresponding likelihood- and pseudo-likelihood-based estimates for an Ising model.</figcaption>
  </figure>
  <div class="research-copy">
    <h2>Likelihood-Based Inference for Intractable Graphical Models</h2>
    <p>Likelihood-based inference for exponential-family graphical models is made computationally feasible despite the presence of intractable normalizing constants. By exploiting the tractable independence model underlying the graphical model, the approach supports full maximum-likelihood and Bayesian inference and can improve parameter estimation and graph recovery relative to conventional pseudo-likelihood methods.</p>
    <p class="research-links"><a href="https://arxiv.org/abs/2404.17763">Paper</a> &middot; <a href="https://github.com/antik015/ExponentialGM">Code</a></p>
  </div>
</div>

<div class="research-item research-item--reverse">
  <figure class="research-visual">
    <div class="research-visual--pair">
      <img src="https://arxiv.org/html/2404.03152v3/v_bart_sept23.png" alt="Posterior predictive mean for the Schwarzschild velocity output">
      <img src="https://arxiv.org/html/2404.03152v3/v_obsd.png" alt="Observed Schwarzschild velocity data">
    </div>
    <figcaption class="research-caption">Posterior predictive mean and observed physical measurements from the Schwarzschild-model calibration.</figcaption>
  </figure>
  <div class="research-copy">
    <h2>Orthogonal Bayesian Calibration</h2>
    <p>Posterior projection provides a Bayesian route to computer-model calibration under an orthogonality constraint on the discrepancy function. This construction addresses identifiability between calibration parameters and model discrepancy while allowing flexible nonparametric priors and extending naturally to multivariate physical systems.</p>
    <p class="research-links"><a href="https://arxiv.org/abs/2404.03152">Paper</a> &middot; <a href="https://github.com/antik015/OCal">Code</a></p>
  </div>
</div>
