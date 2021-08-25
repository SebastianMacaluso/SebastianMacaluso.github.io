---
layout: page
title: Computer vision and jets
description: Image based jet physics classifier with a convolutional neural network
img: /assets/img/jetIcon.png
importance: 1
category: work
---

The Large Hadron Collider (LHC) at CERN collides two beams of high-energy protons and produces many new  (unstable) particles. Some of these new particles (quarks and gluons) will undergo a showering process, where they radiate many other quarks and gluons in successive binary splittings. These splittings can be represented with a binary tree, where the energy of the particles decreases after each step. When the energy is below a given threshold, the showering terminates, resulting in a spray of particles that is called a **jet**. The particle detectors only observe the leaves of this binary tree (the jet constituents).

It is important to classify different types of jets, e.g. originated from W, Z and Higgs bosons, as well as top quarks, with respect to the main QCD background. In this project we use computer vision with deep learning to build a classifier for boosted top jets at the LHC, that could also be straightforwardly extended to other types of jets. In particular, we implemented a convolutional neural network (CNN) to identify jet substructure in signal and background events. Our CNN inputs are jet images that consist of five channels, where each of them represents a color. The first three colors are given by the transverse momentum (pT) of neutral particles from the Hadronic Calorimeter (HCAL) towers, the pT of charged particles from the tracking system and the charged particles multiplicity. The last two colors specify the muon multiplicity and b quark tagging information.

<div class="row justify-content-sm-center">
        <div class="col-sm-10 mt-3 mt-md-0">
        <img class="img-fluid rounded z-depth-1" src="{{ '/assets/img/jetImage.png' | relative_url }}" alt="" title="example image"/>
    </div>
</div>
<div class="caption">
Left: typical single jet image in the rapidity vs azimuthal angle plane for the signal after pre-processing. Center and right: signal and background images averaged over 10,000 individual images. Figure taken from "The Machine Learning Landscape of Top Taggers" (https://scipost.org/10.21468/SciPostPhys.7.1.014).
</div>


Publications: 

**Pulling Out All the Tops with Computer Vision and Deep Learning**   
**S. Macaluso** and D. Shih    
Journal of High Energy Physics volume 2018, Article number: 121 (2018) [[<u> journal paper </u>]](https://link.springer.com/content/pdf/10.1007/JHEP10%282018%29121.pdf) [[<u> arXiv </u>]](https://arxiv.org/abs/1803.00107)
