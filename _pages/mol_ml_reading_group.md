---
title: "Molecular ML Reading Group"
layout: textlay
excerpt: "Molecular ML Reading Group"
sitemap: false
permalink: /mol_ml_reading_group/
---

# Molecular ML Reading Group

The Molecular ML Reading Group aims to explore foundational and recent
applications of machine learning models to modeling molecular system.
The reading group is hosted by [Rosetta Commons](https://www.rosettacommons.org/)
and organized by

* Nick Randolph a PhD
candidate in the Kuhlman Lab at UNC Chapel Hill (nzrandol@unc.edu)
* Matthew O'Meara an Assistant Professor at the University of Michigan
(maom@umich.edu).

<BR><BR>
## Biomolecular Diffusion Models Series
Every-other-week series on Diffusion models

<B> Please fill out the [poll to pick up-coming papers](https://forms.gle/b7pEY4aYrJ4RFdKe7):</B> 

### Next Meeting:

* 10/11/2023 11 am EDT (UTC-4)
* [Zoom link](https://zoom.us/j/99323876996?pwd=bkNwNWZXRmk1bktlTWdBNDRxdXlLdz09)
* [Google Calendar](https://calendar.google.com/calendar/u/0?cid=MmRiZmZjYzAwNGFiZWIyN2Y1ODJiNzU5YzRjMjk4ZGY4MWI1YWE4NTg1MmQ4YWY1NTc3OGYwMzdiNWM5MTEwNEBncm91cC5jYWxlbmRhci5nb29nbGUuY29t)

<br>
<br>
### FrameDiff (9/27)
This week we dug into (Yim, et al., 2023) introducing FrameDiff, a new Diffusion model for protein backbone generation. In this work they
develop the theory of diffusion/denoising machine learning over Remannian manifolds. As a key application they consider each backbone residue as
a rigid frame similar to AlphaFold2. Since each frame has rotational and translational symmetry in 3D, the diffusion should be SE(3) equivariant.
In contrast with RFDiffusion which directly predicts coordinates, in this work they use the stochastic differential equation / score matching
version of diffusion/denoising developed in (Song, et al., 2021). In particular they work out the math for Brownian diffusion on this manifold.
To test their model they train their model directly on a curated subset of the protein databank (unlike RFDiffusion which uses a pre-trained
structure prediction module), and measure the designability, diversity, and novelty of FrameDiff generated backbones. While it was difficult for them
to direclty compare with RFDiffusion because at the time RFDiffusion code was not yet released, it appears to be not quite as performant, but
significantly faster and the model is only 1/4 the size.

* **SE(3) diffusion model with application to protein backbone generation**
Jason Yim, Brian L. Trippe, Valentin De Bortoli, Emile Mathieu, Arnaud Doucet, Regina Barzilay, Tommi Jaakkola
https://arxiv.org/abs/2302.02277

Here are

* [Introductory slides](https://docs.google.com/presentation/d/1xBAvqNyh20Xe3ePdGz4c3h50Iso00trZ/edit?usp=sharing&ouid=101024000819646318057&rtpof=true&sd=true)
* [Video recording](https://youtu.be/S9F-ZBu8Fko?si=T_YGdaon_0rfc4dJ)

<br>
<br>
### Introduction to Diffusion Models (9/13)
Diffusion models is a Deep Learning architecture that has lead to breakthroughs in generating realistic structured data from images, text, and sound.
Diffusion models have also been used to generate proteins and other biomolecular systems. In this first meeting, Nick gives an overview of the basics
of the diffusion model architecture including how to efficiently add noisy data and efficiently train the models by predicting the noise, and generate
samples by iteratively removing the predicted noise. We cover ideas developed in the following works

* Sohl-Dickstein et al. (2015) (https://arxiv.org/abs/1503.03585)
* Yang & Ermon (2019) (https://arxiv.org/abs/1907.05600)
* Ho et al. (2020) (https://arxiv.org/abs/2006.11239)
* Song et al. (2021) (https://arxiv.org/abs/2011.13456)

Here are the

* [Slides](https://docs.google.com/presentation/d/1mdrF-hdZnp1IH6wrDB69p9vmcVaYywGB/edit?usp=sharing&ouid=101024000819646318057&rtpof=true&sd=true)
* [Video recording](https://www.youtube.com/watch?v=qtMRRVL4FYQ)
