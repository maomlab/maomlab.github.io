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

**[Other AI in Chemistry Lecture Series](#other-ai-in-chemistry-lectures-series)**


<BR><BR>
## Biomolecular ML Models Series
Every-other-week series on Diffusion and other molecular ML models
* **Next meeting: 4/24/2024 11-12 pm EDT (UTC-5)**
* [Zoom link](https://zoom.us/j/99323876996?pwd=bkNwNWZXRmk1bktlTWdBNDRxdXlLdz09)
* [Google Calendar](https://calendar.google.com/calendar/u/0?cid=MmRiZmZjYzAwNGFiZWIyN2Y1ODJiNzU5YzRjMjk4ZGY4MWI1YWE4NTg1MmQ4YWY1NTc3OGYwMzdiNWM5MTEwNEBncm91cC5jYWxlbmRhci5nb29nbGUuY29t)

<br>
<br>
### Joint Multi-domain Pre-training (4/10/2024)
[Nima Shoghi](https://nima.sh/) from joins us to discuss [Joint Multi-domain Pre-training](https://doi.org/10.48550/arXiv.2310.16802), exploring the feasability of leverating large-scale simulation data for chemical property and materials prediction tasks. Nima is currently a researcher at the  High Performance Computer Architecture Lab at Georgia Tech and did the work he presented while an AI resident at Meta Fundamental AI Research (FAIR).

* [**From Molecules to Materials: Pre-training Large Generalizable Models for Atomic Property Prediction**](https://doi.org/10.48550/arXiv.2310.16802) Nima Shoghi, Adeesh Kolluru, John R. Kitchin, Zachary W. Ulissi, C. Lawrence Zitnick, Brandon M. Wood. Accepted at ICLR23 arXiv preprint arXiv:2310.16802, 2023.

Here are the:
* [Paper](https://doi.org/10.48550/arXiv.2310.16802)
* [Talk](https://youtu.be/HCtBvtHO5Gk)
* [Slides](https://nima.sh/jmp-molecularml-presentation/1)

<br>
<br>
### Introduction to Flow Matching (3/27/2024)
Matt O'Meara presented a chalk talk style introduction to **Flow Matching** a simplified generalization of denoising diffusion models. The work coveres
background and basics of Flow Matching for molecular modeling.

This talk draws from the following material 
* (Lipman et al. 2022) [Flow Matching for Generative Modeling](https://doi.org/10.48550/arXiv.2210.02747)
** [Lecture](https://youtu.be/5ZSwYogAxYg?si=TEzCycee-34JmrZl), [slides](https://drive.google.com/file/d/1Dkl_NEo1YpoDByxJLuNbqqA493-4NdCY/view)
* (Albergo et al. 2023) [Stochastic Interpolants: A Unifying Framework for Flows and Diffusions](https://doi.org/10.48550/arXiv.2303.08797)
* (Tong et al. 2023) [Improving and generalizing flow-based generative models with minibatch optimal transport](https://doi.org/10.48550/arXiv.2302.00482)
** [Lecture](https://youtu.be/UhDtH7Ia9Ag?si=jNJ3Y3vwDyfM4DVC)
* (Bose et al. 2023) [SE(3)-Stochastic Flow Matching for Protein Backbone Generation](https://doi.org/10.48550/arXiv.2310.02391)
** [Lecture1](https://www.youtube.com/watch?v=t1Pqdl6RB2I), [Lecture2](https://youtu.be/JqKzTdhW7fY?si=lVMnSaLgdTo3-cK4)
** [TorchCFM](https://github.com/atong01/conditional-flow-matching)
* (Campbell et al. 2024)[Generative Flows on Discrete State-Spaces: Enabling Multimodal Flows with Applications to Protein Co-Design](https://doi.org/10.48550/arXiv.2402.04997)

Here is the:
* [talk](https://youtu.be/EpuPamnggiQ)


<br>
<br>
### Keypoint Diffusion (3/13/2024)
Ian Dunn from David Koes lab at the University of Pittsburgh joined us to present [**Keypoint Diffusion**](https://openreview.net/forum?id=Z4ia7s2tpV)
* **[Accelerating Inference in Molecular Diffusion Models with Latent Representations of Protein Structure](https://openreview.net/forum?id=Z4ia7s2tpV)** Ian Dunn, David Koes, NeurIPS 2023 GenBio Workshop Spotlight

Here are the:
* [Paper](https://openreview.net/forum?id=Z4ia7s2tpV)
* [Code](https://github.com/Dunni3/keypoint-diffusion)
* [Talk](https://youtu.be/MqDgxkKNRZE)

<br>
<br>
### Protpardelle (2/28/2024)
Alex Chu from Po-Ssu Huang's lab joined us to present [**Protpardelle**](https://www.biorxiv.org/content/10.1101/2023.05.24.542194v1.full)
* **[An all-atom protein generative model](https://www.biorxiv.org/content/10.1101/2023.05.24.542194v1.full)**  Alexander E. Chu, Lucy Cheng, Gina El Nesr, Minkai Xu, Po-Ssu Huang, DOI: 10.1101/2023.05.24.542194

Here are the:
* [Paper](https://www.biorxiv.org/content/10.1101/2023.05.24.542194v1.full)
* [Code](https://github.com/ProteinDesignLab/protpardelle)
* [Webapp](https://huggingface.co/spaces/ProteinDesignLab/protpardelle)
* [Talk](https://youtu.be/jy3Qr8g4SU8)


<br>
<br>
### ProteinGenerator (2/14/2024)
This week [Sidney Lisanza](https://www.bakerlab.org/members-old/sidney-lisanza/) from the Baker Lab joined us to present [**ProteinGenerator**](https://github.com/RosettaCommons/protein_generator)
* **["Joint Generation of Protein Sequence and Structure with RoseTTAFold Sequence Space Diffusion"](https://doi.org/10.1101/2023.05.08.539766)** Lisanza SL,  Gershon JM, Tipps S, Arnoldt L, Hendel S, Sims JN, Li X DOI: 10.1101/2023.05.08.539766

Here are the:
* [Paper](https://www.biorxiv.org/content/10.1101/2023.05.08.539766v1)
* [Code](https://github.com/RosettaCommons/protein_generator)
* [Webapp](https://huggingface.co/spaces/merle/PROTEIN_GENERATOR)
* [Talk](https://youtu.be/T6zMqormGP0)
* [Slides](https://bit.ly/ProteinGenerator)

<br>
<br>
### EvoDiff (1/31/2024)
This week [Sarah Alamdari](https://www.sarahalamdari.com/) a data scientist at [Microsoft Research](https://www.microsoft.com/en-us/research/theme/biomedical-ml/) presented [**EvoDiff**](https://github.com/microsoft/evodiff)
* **[Protein generation with evolutionary diffusion: Sequence is all you need](https://www.biorxiv.org/content/10.1101/2023.09.11.556673)** Sarah Alamdari, Nitya Thakkar, Rianne van den Berg, Alex X. Lu, Nicolo Fusi1, Ava P. Amini, Kevin K. Yang DOI: 10.1101/2023.09.11.556673v1

Here are the:
* [Paper](https://www.biorxiv.org/content/10.1101/2023.09.11.556673)
* [Code](https://github.com/microsoft/evodiff)
* [Talk](https://youtu.be/QxjCqZVbSek?si=cHQyBRBDYvEHfUi0)
* [Slides](https://bit.ly/3Sn569D)


<br>
<br>
### Frame2Seq (1/17/2024)
This week Deniz Akpinaroglu from the Kortemme Lab at UCSF presented her recent work on Frame2seq
* **Structure-conditioned masked language models for protein sequence design generalize beyond the native sequence space** 
Deniz Akpinaroglu, Kosuke Seki, Amy Guo, Eleanor Zhu, Mark J. S. Kelly, Tanja Kortemme
DOI: 10.1101/2023.12.15.571823

Here are the:
* [Paper](https://www.biorxiv.org/content/10.1101/2023.12.15.571823)
* [Code](https://github.com/dakpinaroglu/Frame2seq)
* [Talk Recording](https://youtu.be/fTcg3vdEPHU?si=GEYzeN9uu2mQgCFt)
* [Slides](https://drive.google.com/file/d/1zN8mRIObKoMRfC2DIedm0KPy9uiI0Jc5/view?usp=drive_link)

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
* [Talk](https://youtu.be/91m1JA7zUNo)
* [Slides](https://bit.ly/3uQq4WE) 

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
* [Talk](https://youtu.be/flsNV36AtAU)

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
* [Talk](https://youtu.be/JqKzTdhW7fY)

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
* [Talk](https://youtu.be/PARZP6GWJ0w?si=2UJwSuhAw-8QCVjF)

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

<hr>
## Other AI in Chemistry Lectures series
[VantAI](https://www.vant.ai/)
* Generative AI in Drug Discovery Lecture Series
** [Website](https://www.genaiindrugdiscovery.com/), [YouTube Channel](https://www.youtube.com/playlist?list=PLAXC54QmQTfz5Pk_3yq9RfLaU0b13lWgF)

[Valence Labs](https://www.youtube.com/@valence_labs/playlists)
* M2D2: Molecular Modeling and Drug Discovery [website](https://portal.valencelabs.com/m2d2), [YouTube](https://www.youtube.com/playlist?list=PLoVkjhDgBOt11Q3wu8lr6fwWHn5Vh3cHJ)
* 2023 Molecular Machine Learning Conference [website](https://logconference.org/), [YouTube](https://www.youtube.com/playlist?list=PLoVkjhDgBOt1ipeEq5XPoWV9MbyLwwRl1)
* Causality, Abstraction, Reasoning, & Extrapolation [website](https://portal.valencelabs.com/care), [Youtube](https://www.youtube.com/playlist?list=PLoVkjhDgBOt3YFQC_8NIwJStWNbyd5Ms-)
* Graphs and Geometry Reading Group [website](https://portal.valencelabs.com/logg), [YouTube](https://www.youtube.com/playlist?list=PLoVkjhDgBOt2UwOm70DAuxHf1Jc9ijmzl)

[Boston Protein Design and Modeling Club](https://www.bpdmc.org/)
* BPDMC hosts a monthly meeting that begins with dinner, drinks, and an hour-long scientific program. We have seminars, tutorials and workshops, and the occasional moderated group discussion after a major breakthrough is announced. The scientific program is followed by an hour (or so) for additional discussion and networking.
* [YouTube](https://www.youtube.com/@bpdmc/videos)

[ML for protein engineering seminar series](https://www.ml4proteinengineering.com/)
* A bi-weekly seminar series focused on recent work in machine learning for protein engineering. 
* [YouTube](https://www.youtube.com/@mlforproteinengineeringsem6420/videos)
