---
title: imcascade
layout: page
categories:
- General
feature_image: "http://trafyx.com/wp-content/uploads/2016/10/gxphot.png"
---

To measure the sizes of distant galaxies one must account for telescope systematics like the point-spread function. This is usually accomplished using a forward modelling procedure using parameterized models such as a Sersic profile, for the galaxy. This is a restrictive parameterization which may not match reality and can lead to biased results with unknown systematic errors.

#### Moving beyond the Sersic profile

In a recent study [(Miller & van Dokkum 2021)](https://arxiv.org/abs/2109.13262), we develop and describe imcascade, a Bayesian implementation of the multi-gaussian expansion method for fitting the morphology of galaxies. This represents the galaxy as a mixture of Gaussians, and is a very flexible description of the light proifle. This has some key advantages over the traditional Sersic fitting. Mainly that it is not hamstrung by simplistic parameterizations. This means one can obtrain reliable uncertainties or focus on lower S/N regions of the galaxy, like the outskirts. It also allows the direct study of brightness and colour profiles. There are also some cool numerical tricks like analytic convolution and pixel integration involved. We have applied this method to [HST data](/research/gal_size/) to study colour gradients in galaxies at z=2 and are working on applying it to early JWST imaging! 

The code is availible on [github](https://github.com/tbmiller-astro/imcascade) and [PyPI](https://pypi.org/project/imcascade/). Please reach out if you are intereseted in using this code and have any questions.