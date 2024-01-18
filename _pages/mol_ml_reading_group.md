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
Every-other-week series on Diffusion and other molecular ML models
* **Next meeting: 1/31/2024 11 am EST (UTC-5)**
* [Zoom link](https://zoom.us/j/99323876996?pwd=bkNwNWZXRmk1bktlTWdBNDRxdXlLdz09)
* [Google Calendar](https://calendar.google.com/calendar/u/0?cid=MmRiZmZjYzAwNGFiZWIyN2Y1ODJiNzU5YzRjMjk4ZGY4MWI1YWE4NTg1MmQ4YWY1NTc3OGYwMzdiNWM5MTEwNEBncm91cC5jYWxlbmRhci5nb29nbGUuY29t)



<br>
<br>
### Frame2Seq (1/17/2024)
This week Deniz Akpinaroglu from the Kortemme Lab at UCSF presented her recent work on Frame2seq
* **Structure-conditioned masked language models for protein sequence design generalize beyond the native sequence space** 
Deniz Akpinaroglu, Kosuke Seki, Amy Guo, Eleanor Zhu, Mark J. S. Kelly, Tanja Kortemme
DOI: 10.1101/2023.12.15.571823

Here is the:
* [paper](https://www.biorxiv.org/content/10.1101/2023.12.15.571823)
* [code](https://github.com/dakpinaroglu/Frame2seq)
* [Talk Recording](https://youtu.be/fTcg3vdEPHU?si=GEYzeN9uu2mQgCFt)

<br>
<br>
### GENIE (12/6/2023)
This week Yeqing Lin from the [AlQuraishi lab](https://www.aqlab.io/) at Columbia joined us to discuss [Genie](https://github.com/aqlaboratory/genie), a diffusion based model for protein structure prediction that equivariantly diffuses over oriented residue clouds.
* **Generating Novel, Designable, and Diverse Protein Structures by Equivariantly Diffusing Oriented Residue Clouds**
Yeqing Lin, Mohammed AlQuraishi
DOI: 10.48550/arXiv.2301.12485

Here is the:
* [Paper](https://arxiv.org/abs/2301.12485)
* [Code](https://github.com/aqlaboratory/genie)
* [Talk Recording](https://youtu.be/91m1JA7zUNo)
* [talk Slides](https://bit.ly/3uQq4WE) 

<br>
<br>
### Umol (11/22/2023)
This week [Patrick Bryant](https://www.scilifelab.se/researchers/patrick-bryant/) from Frank Noé's lab at FU Berlin and starting his own group soon at Stockholm University/Science for Life Laboratory joined us to discuss [Umol](https://www.biorxiv.org/content/10.1101/2023.11.03.565471v1), a deep learning based ligand docking method. He gives some interesting details about trying to train a variant of AlphaFold2 that considers small molecule atoms and balancing the more abundant constraints from the mulitple sequence alignment with the less abundant constraints for the ligand geometry.

* **Structure prediction of protein-ligand complexes from sequence information with Umol**
Patrick Bryant, Atharva Kelkar, Andrea Guljas, Cecilia Clementi, and Frank Noé
DOI: 10.1101/2023.11.03.565471

Here is the:
* [Paper](https://doi.org/10.1101/2023.11.03.565471)
* [Code](https://github.com/patrickbryant1/Umol)
* [Collab Notebook](https://colab.research.google.com/github/patrickbryant1/Umol/blob/master/Umol.ipynb)
* [Talk Recording](https://youtu.be/flsNV36AtAU)

<br>
<br>
### FlowFold (11/08/2023)
This week Joey Bose, Tara Akhound-Sadegh, and colleagues join us to present FoldFlow (Bose et al., 2023), a conditional flow matching model for protein backbone generation. Using insights from differential geometry they improve the training of flows on the Riemannian manifold over a collection of protein backbone frames. They achieve SOTA performance on non-pretrained de novo backbone generation for a number of metrics.

* **SE(3)-Stochastic Flow Matching for Protein Backbone Generation**
Avishek Joey Bose, Tara Akhound-Sadegh, Kilian Fatras, Guillaume Huguet, Jarrid Rector-Brooks, Cheng-Hao Liu, Andrei Cristian Nica, Maksym Korablyov, Michael Bronstein, Alexander Tong
DOI: 10.48550/arXiv.2310.16802

Here is the:
* [Paper](https://doi.org/10.48550/arXiv.2310.16802)
* [Code](https://github.com/DreamFold/FoldFlow)
* [Recording](https://youtu.be/JqKzTdhW7fY)

<br>
<br>
### RoseTTAFold All-Atom (10/25/2023)
This week we Rohith Krishna, a graduate student in the Baker Lab at UW, joins us to present RoseTTAFold All-Atom (Krishna, et al., 2023).
This work generalizes the RoseTTA Fold "three-track architecture" to handle non-protein molecules. They then use this
for a range of different applications including re-training RFDiffusion to enable predicting ligand and cofactor binding.


* **[Generalized Biomolecular Modeling and Design with RoseTTAFold All-Atom](https://doi.org/10.1101/2023.10.09.561603)**
Rohith Krishna, Jue Wang, Woody Ahern, Pascal Sturmfels, Preetham Venkatesh, Indrek Kalvet, Gyu Rie Lee, Felix S Morey-Burrows, Ivan Anishchenko, Ian R Humphreys, Ryan McHugh, Dionne Vafeados, Xinting Li, George A Sutherland, Andrew Hitchcock, C Neil Hunter, Minkyung Baek, Frank DiMaio, David Baker
DOI: 10.1101/2023.10.09.561603

Here is the
* [Video recording](https://youtu.be/PARZP6GWJ0w?si=2UJwSuhAw-8QCVjF)

<br>
<br>
### RFDiffusion (10/11/2023)
This week we discuss RFDiffusion (Watson, et al., 2023), a diffusion denoising model based on RoseTTAFold to generate realistic protein protein backbones. Nick Randolf gives an overview of the method and we discuss the method details.

* **[De novo design of protein structure and function with RFdiffusion](https://doi.org/10.1038/s41586-023-06415-8)**
Joseph L. Watson, David Juergens, Nathaniel R. Bennett, Brian L. Trippe, Jason Yim, Helen E. Eisenach, Woody Ahern, Andrew J. Borst, Robert J. Ragotte, Lukas F. Milles, Basile I. M. Wicky, Nikita Hanikel, Samuel J. Pellock, Alexis Courbet, William Sheffler, Jue Wang, Preetham Venkatesh, Isaac Sappington, Susana Vázquez Torres, Anna Lauko, Valentin De Bortoli, Emile Mathieu, Sergey Ovchinnikov, Regina Barzilay, Tommi S. Jaakkola, Frank DiMaio, Minkyung Baek & David Baker
Nature 620, 1089–1100 (2023).
DOI: 10.1038/s41586-023-06415-8

Here are the
* [slides](https://bit.ly/46Terw4)
* [Video recording](https://youtu.be/agiHi6hOE3Q)

<br>
<br>
### FrameDiff (9/27/2023)
This week we dug into (Yim, et al., 2023) introducing FrameDiff, a new Diffusion model for protein backbone generation. In this work they
develop the theory of diffusion/denoising machine learning over Remannian manifolds. As a key application they consider each backbone residue as
a rigid frame similar to AlphaFold2. Since each frame has rotational and translational symmetry in 3D, the diffusion should be SE(3) equivariant.
In contrast with RFDiffusion which directly predicts coordinates, in this work they use the stochastic differential equation / score matching
version of diffusion/denoising developed in (Song, et al., 2021). In particular they work out the math for Brownian diffusion on this manifold.
To test their model they train their model directly on a curated subset of the protein databank (unlike RFDiffusion which uses a pre-trained
structure prediction module), and measure the designability, diversity, and novelty of FrameDiff generated backbones. While it was difficult for them
to direclty compare with RFDiffusion because at the time RFDiffusion code was not yet released, it appears to be not quite as performant, but
significantly faster and the model is only 1/4 the size.

* **[SE(3) diffusion model with application to protein backbone generation](https://arxiv.org/abs/2302.02277)**
Jason Yim, Brian L. Trippe, Valentin De Bortoli, Emile Mathieu, Arnaud Doucet, Regina Barzilay, Tommi Jaakkola
DOI: 10.48550/arXiv.2302.02277


Here are

* [Introductory slides](https://docs.google.com/presentation/d/1xBAvqNyh20Xe3ePdGz4c3h50Iso00trZ/edit?usp=sharing&ouid=101024000819646318057&rtpof=true&sd=true)
* [Video recording](https://youtu.be/S9F-ZBu8Fko?si=T_YGdaon_0rfc4dJ)

<br>
<br>
### Introduction to Diffusion Models (9/13/2023)
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
