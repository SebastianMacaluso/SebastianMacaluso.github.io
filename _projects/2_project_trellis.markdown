---
layout: page
title: Hierarchical Cluster Trellis
description: Data Structures and Algorithms for Exact Inference in Hierarchical Clustering
img: /assets/img/trellis.png
github: https://github.com/SebastianMacaluso/ClusterTrellis
importance: 1
category: work
---

The Hierarchical Cluster Trellis introduces data structures and algorithms for exact inference in hierarchical clustering. Hierarchical clustering is a fundamental task often used to discover meaningful structures in data, such as phylogenetic trees, taxonomies of concepts, subtypes of cancer, and cascades of particle decays in particle physics. Typically approximate algorithms are used for inference due to the combinatorial number of possible hierarchical clusterings. In contrast to existing methods, the Hierarchical Cluster Trellis introduces novel dynamic-programming algorithms for **exact** inference in hierarchical clustering based on a novel trellis data structure, that can exactly compute the partition function, maximum likelihood hierarchy, and marginal probabilities of sub-hierarchies and clusters. These algorithms scale in time and space proportional to the powerset of N elements which is super-exponentially more efficient than explicitly considering each of the (2N-3)!! possible hierarchies.  

The [<u>ClusterTrellis</u>](https://github.com/SebastianMacaluso/ClusterTrellis) package is a toolkit with ready to use and computationally efficient algorithms to find exact solutions for the MAP hierarchy and partition function (marginal over all possible hierarchies) for any user defined model of hierarchical clustering that fits in the class we consider. The toolkit also provides an algorithm to sample hierarchies from the exact true posterior distribution without enumerating all possible hierarchies. A related library is [Ecole](https://www.ecole.ai/) that aims to expose a number of control problems arising in combinatorial optimization solvers as Markov Decision Processes.

<div class="row justify-content-sm-center">
        <div class="col-sm-10 mt-3 mt-md-0">
        <img class="img-fluid rounded z-depth-1" src="{{ '/assets/img/hierarchical_trellis_diagram_v7.png' | relative_url }}" alt="" title="example image"/>
    </div>
</div>
<div class="caption">
Computing the partition function for the dataset {a,b,c,d}. Left: exhaustive computation, consisting of the summation of (2x4-3)!! =15  energy equations. Right: computation using the trellis.  The sum for the partition function is over 2^{4-1} - 1 = 7 equations, each making use of a memoized partition function value. Colors indicate corresponding computations over siblings in the trellis.
</div>


Publications: 

**Cluster Trellis: Data Structures & Algorithms for Exact Inference in Hierarchical Clustering**  
C. S. Greenberg, **S. Macaluso**, N. Monath, J.-A. Lee, P. Flaherty, K. Cranmer,
A. McGregor, and A. McCallum   
The 24th International Conference on Artificial Intelligence and Statistics (AISTATS 2021) [[<u> conference paper </u>]](http://proceedings.mlr.press/v130/macaluso21a/macaluso21a.pdf) [[<u> arXiv </u>]](https://arxiv.org/abs/2002.11661) [[<u> code </u>]](https://github.com/SebastianMacaluso/ClusterTrellis)  
(Also: The 4th Workshop on Tractable Probabilistic Modeling [[<u> workshop paper </u>]](https://openreview.net/forum?id=imgfvlsXdo3)) 