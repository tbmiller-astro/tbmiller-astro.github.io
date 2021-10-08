---
title: Research
layout: page
feature_image: "https://www.dragonflytelescope.org/uploads/1/2/0/1/120152565/background-images/348137435.jpg"
---
### imcascade: Bayesian MGE models

In a recent paper [(Miller & van Dokkum 2021)](https://arxiv.org/abs/2109.13262), we describe imcascade, a Bayesian implementation of the multi-gaussian expansion method for fitting the morphology of galaxies. This represents the galaxy as a mixture of Gaussians, and is a very flexible description of the light proifle. This has some key advantages over the traditional Sersic fitting. Mainly that it is not hamstrung by simplistic parameterizations. This means one can obtrain reliable uncertainties or focus on lower S/N regions of the galaxy, like the outskirts. It also allows the direct study of brightness and colour profiles. There are also some cool numerical tricks like analytic convolution and pixel integration involved. We are currently applying this method to HST data to study colour gradients in galaxis at cosmic noon so check back soon for those results.

The code is availible on [github](https://github.com/tbmiller-astro/imcascade) and [PyPI](https://pypi.org/project/imcascade/). Please reach out if you are intereseted in using this code and have any questions.

### We are not missing light in the outskirts of massive galaxies
Massive galaxies are integral to our understanding of galaxy formation however they are notoriously tricky to observe properly. They are known to have very extended low surface-brightness outskirts which contain a large fraction of their light (>10%). Using the data from the [Dragonfly telephoto array](https://www.dragonflytelescope.org/) and a photometry method designed to take advatage of the DF data, we accurately measured the total flux and colors of nearby massive galaxies taking into account all the light in the outskirts. When comparing to common methods applied to SDSS, we find that our total flux measurement agree but DF measured bluer colors on average. This leads to the perplexing result that when accounting for the light in the outskirts with dragonfly we measure lower stellar masses the other techniques. These results are published in a [paper that appeared in ApJ](https://ui.adsabs.harvard.edu/abs/2021ApJ...909...74M/abstract)

### How to define the size of a galaxy?

As a part of thesis I am studying the sizes of galaxies. Specifically different definitions of the size of a galaxy and how these choise impact our interpretation common scaling relations. Galaxies do not have an edge or cut-off so it is likely impossible to uniquely define the size of a galaxy. The most commonly used measure is the half-light, or effective radius, which is the radius that contains half of the total luminosity. In a recent paper we wrote ( [Miller et al. 2019](https://ui.adsabs.harvard.edu/abs/2019ApJ...872L..14M/abstract) ) we investigate r<sub>80</sub> and r<sub>20</sub> the radii that contain 80% or 20% of a galaxy's total luminosity. In the figure below, taken from the paper, we show that the galaxy size - stellar mass relation looks markedly different depending on which definition of size is used. Specifically when we use r<sub>80</sub> star-forming and quiescent galaxies appear to have nearly the same size at all stellar masses. This is contrary to many previous works which suggest star-forming and quiescent galaxies follow different tracks in the size-mass plane.

| <img src="https://user-images.githubusercontent.com/51385038/100286982-cfc36180-2f41-11eb-81d7-de3aabd1d72b.PNG" alt="drawing" width="700"/> | 
|:--:| 
| Showing the galaxy size -- stellar mass distribution using different definitions of radii from [Miller et al. 2019](https://ui.adsabs.harvard.edu/abs/2019ApJ...872L..14M/abstract) |

### Sub-mm galaxies

During my B.Sc and M.Sc degrees I worked with Scott Chapman on observational and theoretical studies of Sub-mm galaxies.  These are dusty galaxies at z > 2 which posses star formation rates up to 1000 solar masses per year. They are some of the most extreme galaxies ever observed and allow us to study star formation in extreme environments in the early universe. I focused on using these galaxies to signpost early overdensities and proto-clusters in the early universe.

In particular we published a very exciting result in [Nature](https://www.nature.com/articles/s41586-018-0025-2) where we discovered a galaxy cluster at redshift 4.3. This is one of the youngest and most convincing observations of a proto-cluster, which will likely form a massive galaxy cluster by the present day. Originally a bright smudge in observations from the South Pole Telescope, follow-up with the APEX and ALMA telescope revealed the source SPT2349-56 to contain no less then 14 galaxies. Through measurements of the CII and CO(4-3) emission lines we confirm all 14 galaxies reside at the same redshift and within 150 projected kpc of each other. You can read the manuscript [here](https://arxiv.org/abs/1804.09231) or read some awesome press articles from various sources: [BBC](https://www.bbc.com/news/science-environment-43841025), [CBC](https://www.cbc.ca/news/technology/galaxy-cluster-1.4628787) or [LA times](https://www.latimes.com/science/sciencenow/la-sci-sn-galaxy-mega-merger-20180425-story.html)

| <img src="https://public.nrao.edu/wp-content/uploads/2018/04/nrao18cb5b.jpg" alt="drawing" width="350"/> | 
|:--:| 
| Showing the discovery of SPT2349-56 in SPT, LABOCA and ALMA images <br /> Credit: ALMA (ESO/NAOJ/NRAO), T. Miller & S. Chapman et al.; Herschel; South Pole Telescope; (NRAO/AUI/NSF) B. Saxton |

### Self-Friction
Here at Yale I have also worked with Frank van den Bosch on investigating dark matter substructure in numerical simulations. Recently it has become clear the large cosmological simulations do not properly resolve sub-halo and they are prone to troublesome numerical artifacts. Therefore the detailed behavior of sub-halos in these large volume simulations shouldn't be trusted! We have created the [DASH library](https://cosmo.oca.eu/dash/) which is a suite of high resolution simulations to better understand the dynamics of subhalos

We are also working a study exploring the effects of  dynamical self-friction: when a sub-halo's previously stripped material interacts with the still bound remnant causing it to lose angular momentum and decay in radius.  This adds another complication to the already difficult process of modelling galaxy mergers. We have published these results in [Miller et al. 2020](https://ui.adsabs.harvard.edu/abs/2020MNRAS.495.4496M/abstract). Self-friction always leads to orbital decay, sapping angular momentum from the subhalo. While we find that in general self-friction is a 10% effect compared to normal dynamical friction it is important for radial orbits close to their pericentric passage.
