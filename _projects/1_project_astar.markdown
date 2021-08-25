---
layout: page
title: Hierarchical Clustering Using A*
description: Exact and Approximate Hierarchical Clustering Using A*
img: /assets/img/Astar_icon.png
github: https://github.com/SebastianMacaluso/AstarTrellis
importance: 1
category: work
---

Hierarchical clustering is a critical task in numerous domains. Many approaches are
based on heuristics and the properties of the resulting clusterings are studied post hoc.
However, in several applications, there is a natural cost function that can be used to
characterize the quality of the clustering. In those cases, hierarchical clustering can be
seen as a combinatorial optimization problem. To that end, we introduce a new approach
based on A* search. We overcome the prohibitively large search space by combining
A* with a novel trellis data structure. This combination results in an exact algorithm
that scales beyond previous state of the art, from a search space with 10<sup>12 </sup> trees to 10<sup>15 </sup>
trees, and an approximate algorithm that improves over baselines, even in enormous
search spaces that contain more than 10<sup>1000 </sup> trees. We empirically demonstrate that our
method achieves substantially higher quality results than baselines for a particle physics
use case and other clustering benchmarks. We describe how our method provides
significantly improved theoretical bounds on the time and space complexity of A* for
clustering. The [<u>A* package</u>](https://github.com/SebastianMacaluso/AstarTrellis)  provides all the data structures, algorithms, and experiments for MAP and Z computation for hierarchical clusteringis using A*.

<div class="row justify-content-sm-center">
        <div class="col-sm-7 mt-3 mt-md-0">
        <img class="img-fluid rounded z-depth-1" src="{{ '/assets/img/Astar_trellis.png' | relative_url }}" alt="" title="example image"/>
    </div>
</div>
<div class="caption">
Nested Min Heaps: The A* search space is compactly encoded in the trellis.
Each node stores a min-heap ordering pairs of its children. Each pair encodes a two partition
(e.g. split) of its parents points.
</div>


Publications: 

**Exact and Approximate Hierarchical Clustering Using A***  
Craig S Greenberg, **Sebastian Macaluso**, Nicholas Monath, Avinava Dubey, Patrick Flaherty, Manzil Zaheer, Amr Ahmed, Kyle Cranmer, Andrew McCallum  
37th Conference on Uncertainty in Artificial Intelligence (UAI 2021) [[<u> conference paper </u>]](https://www.auai.org/uai2021/pdf/uai2021.770.pdf) [[<u> arXiv </u>]](https://arxiv.org/abs/2104.07061) [[<u> code </u>]](https://github.com/SebastianMacaluso/AstarTrellis)  