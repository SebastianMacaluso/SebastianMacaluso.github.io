---
layout: page
title: Ginkgo
description: Simplified Generative Model for Jets
img: /assets/img/ginkgo.png
importance: 1
category: work
---

Ginkgo is a generative model to aid in machine learning (ML) research for jet physics. Ginkgo is implemented in [<u> Pyro </u>](https://pyro.ai/) and facilitates research with:
 * Dynamic programming
 * Differentialble programming
 * Probabilistic programming
 * Variational inference
 
 The motivation is to build a model that has a tractable likelihood, and is as simple and easy to describe as possible but at the same time captures the essential ingredients of parton shower generators in full physics simulations.  The aim is for the model to have a python implementation with few software dependencies. [<u> Ginkgo </u>](https://github.com/SebastianMacaluso/ginkgo) python package can be found on github and a complete description on [<u> Ginkgo Notes</u>](https://www.overleaf.com/read/pmmcqhyfsctf).

Parton shower generators are software tools that encode a physics model for the simulation of jets that are produced at colliders, e.g. the Large Hadron Collider at CERN.
Jets are a collimated spray of energetic charged and neutral particles. Parton showers generate the particle content of a jet, going through a cascade process, starting from an initial unstable particle. In this description, there is a recursive algorithm that produces binary splittings of an unstable parent particle into two children particles, and a stopping rule. Thus, starting from the initial unstable particle, successive splittings are implemented until all the particles are stable (i.e. the stopping rule is satisfied for each of the final particles). We refer to this final particles as the jet constituents.

As a result of this showering process, there could be many latent paths that may lead to a specific jet (i.e. the set of constituents). Thus, it is natural and straightforward to represent a jet and the particular showering path that gave rise to it as a binary tree, where the inner nodes represent each of the unstable particles and the leaves represent the jet constituents. 



<div class="row justify-content-sm-center">
     <div class="col-sm-6 mt-3 mt-md-1">
        <img class="img-fluid rounded z-depth-1" src="{{ '/assets/img/ginkgoPseudocode.png' | relative_url }}" alt="" title="example image"/>
    </div>
        <div class="col-sm-6 mt-3 mt-md-0">
        <img class="img-fluid rounded z-depth-1" src="{{ '/assets/img/ginkgoTree.png' | relative_url }}" alt="" title="example image"/>
    </div>
</div>
<div class="caption">
    Left: Pseudocode for the algorithm. Right: Tree visualization of a sample jet generated with Ginkgo.
</div>



