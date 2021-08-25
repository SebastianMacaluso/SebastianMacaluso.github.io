---
layout: page
title: TreeNiN
description: Recursive Tree Network in Network (TreeNiN) for Jet Physics
img: /assets/img/dockerTreeNiN.png
github: https://github.com/diana-hep/TreeNiN
importance: 1
category: work
---

In this method, a tree neural network (TreeNN) is trained on particle physics jets. The TreeNN provides a *jet embedding*, which maps a set of 4-momenta into a vector of fixed size and can be trained together with a successive network used for classification or regression. Jet constituents are reclustered to form binary trees, and the topology is determined by the clustering algorithm. 

We introduced a Network in Network generalization of the simple TreeNN architecture proposed in [Louppe et al. 2017](https://arxiv.org/abs/1702.00748), where we add fully connected layers at each node of the binary tree before moving forward to the next level. We refer to this model as TreeNiN. In particular, we add 2 NiN layers with ReLU activations. Also, we split weights between internal nodes and leaves, both for the NiN layers and for the initial embedding of the 7 input features of each node. Finally, we introduce two sets of independent weights for the NiN layers of the left and right children of the root node. Our model has 33,901 trainable parameters. Training is performed over 40 epochs with a minibatch of 128 and a learning rate of 0.002 (decayed by a factor of 0.9 after every epoch), using the cross entropy loss function and Adam as the optimizer.



 We developed a PyTorch implementation to provide GPU acceleration. The [<u>TreeNiN</u>](https://github.com/diana-hep/TreeNiN) package provides all the necessary code and can also be downloaded as a docker container 
  [smacaluso/treenin](https://hub.docker.com/r/smacaluso/treenin)
 This algorithm ranks among the top three on the physics community benchmark comparison: [[<u> The Machine Learning Landscape of Top Taggers </u>]](https://scipost.org/10.21468/SciPostPhys.7.1.014).



