---
layout: page
title: Code and Data Products
feature_image: "https://www.predictiveanalyticsworld.com/patimes/wp-content/uploads/2019/10/kdnuggets-image.jpg"
---

# Code
Please look at my [github profile](https://github.com/tbmiller-astro) to see all the projects I'm currently working on. I briefly describe some of my main projects here:

### [How to measure distances?](/research/silkscreen.md)

I am the lead developer of silkscreen, a novel simulation based inference approach to measuring distances of dwarf galaxies. We recently published a paper describing the concept along with some applications but we are hoping to expand and improve the implementation. Our ultimate goal is a robust method to measure distances to dwarf galaxies from large surveys like LSST, Roman and Euclid.

#### [Sersic fitting for the 2020's and beyond](/research/pysersic/)

I am a co-lead developer of pysersic, a new Bayesian implementation of a old method. Parameteric profile fitting is a stable in extragalactic astronomy to study the morphology of galaxies, and there are many codes designed to do so. The benefits of pysersic are that is is written fully in python, utilizing [jax](https://github.com/google/jax) for faster execution, ability to run on GPUs and gradient tracking. We utilize gradient information for lightning quick Bayesian inference, in most cases you can get full posterior on your laptop in less than 30 seconds. 

We designed pysersic to be simple to use but still customizable were necessary! All the development is hosted on [github](https://github.com/pysersic/pysersic). Feel free to reach out if you have any questions or issues!

### [imcascade: A more flexibale alternative for studying galaxy morphology](/research/imcascade.md)
During my PhD I developed imcascade (fitting IMages with a CASCADE of gaussians, described [here](https://arxiv.org/abs/2109.13262) ). It is a Bayesian implementation of the multi-gaussian expansion method for fitting the morphology of galaxies. The python implementation is availible on [github](https://github.com/tbmiller-astro/imcascade) and [PyPI](https://pypi.org/project/imcascade/). Please see the docs for an in-depth example and also reach out if you are intereseted in using this code and have issues or any questions.

# Data

### Galaxy photometry in the DWFS
Please find a [link](https://github.com/tbmiller-astro/tbmiller-astro.github.io/blob/main/assets/Miller2020_DWFS_galphot.dat?raw=true) to a catalog of photometry measurements for massive galaxies in the Dragonfly Wide Field Survey from [Miller et al. (2020)](https://arxiv.org/abs/2010.07310). The photometry is measured by integrating the 1-D profile as described in the paper and is converted to the SDSS filter system. Total magnitudes for the g and r band reported as well as the g-r color. Please cite the above paper if you use this data and reach out if you have any questions.
