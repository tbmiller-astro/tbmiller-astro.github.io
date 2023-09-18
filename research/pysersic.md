---
title: pysersic
layout: page
categories:
- General
feature_image: "https://raw.githubusercontent.com/pysersic/pysersic/main/misc/pysersic.png"
---

Sersic profile fitting is an invaluable tool in observational extragalactic astronomy. It underpins the morphology and photometry measurements of every modern survey and nearly all research studies. In essence, it is a forward modelling techniques utilizing the parametric Sersic profile to describe the observed light distribution of galaxies. Based on this simple premise there are many different implementations. One of those implementations is pysersic, which my colleague [Imad](https://imad-pasha.github.io/) and I developed. I'm a little biased of course, but I think it's pretty great! 

The goal of pysersic is to put Sersic fitting in a Bayesian inference framework and utilize the recently developed jax library. Developed by google for machine learning, jax greatly speeds up computations, compared to normal python, allows code to seamlessly run on GPU's and TPUs. Last but not least, it also tracks gradients. This last part is crucial for fast Bayesian inference utilizing modern, gradient based samplers such as Hamiltonian Monte Carlo. All this combines so that pysersic can calculate posteriors of morphological parameters and fast!

We designed to be simple to use for fitting one, or more sources simultaneously. This package is still quite young and development is on-going. While the basic functionality is working and tested we are always adding new features and improving the implementations so please reach our if you have ides for how to improve pysersic. 

For more info please read the [paper describing pysersic](https://joss.theoj.org/papers/10.21105/joss.05703). All development happens on [github](https://github.com/pysersic/pysersic).