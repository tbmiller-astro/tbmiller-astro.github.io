---
title: silkscreen
layout: page
categories:
- General
feature_image: "https://upload.wikimedia.org/wikipedia/commons/1/18/True_blue.jpg"
---


Dwarf galaxy, with stellar mass less than one billion solar masses, represent the edge of galaxy formation and are ideal laboratories to study the physics of galaxy formation and dark matter. We know about many such galaxies in the local Universe however there is one persistent issue: We do not have a reliable method to measure distances. This is astronomers dirty little secret and it blocks us from being able to easily investigate the physical nature of these galaxies.

silkscreen is an ambitious project where we (lead by Myself, [Imad Pasha](https://imad-pasha.github.io) and [Ava Polzin](https://avapolzin.github.io) ) are using  machine learning methods to develop more consistent, less biased and widely applicable method -- I know a lot to ask -- for measuring distances to dwarf galaxies. This lead us to combine the forward modelling capabilities of [ArtPop](https://artpop.readthedocs.io/en/latest/) with simulation based inference techniques to develop [silkscreen](https://github.com/tbmiller-astro/silkscreen). We recently published an initial description of the code and its capabilities [here](https://arxiv.org/abs/2407.04091). 

The main issue is that it currently requires simulations and training on a per-galaxy basis, about 100 CPU-hours and 6 hours of GPU time. For a few galaxies this is a reasonable investment however it scales linearly so becomes intractable for large sample of galaxies. Our next goal is to train a contextually broad model, so called amortized in the SBI literature, that where inference can be performed on any galaxy in a survey in a matter of seconds. The ultimate goal is to train these models for LSST, Roman and Euclid as a community resource.