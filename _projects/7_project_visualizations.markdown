---
layout: page
title: Visualizations
description: 1D and 2D heat clustermap visualizations of binary trees
img: /assets/img/heatMap_icon.png
github: https://github.com/SebastianMacaluso/VisualizeBinaryTrees
importance: 1
category: work
---



The visualization package for binary trees, [<u>VisualizeBinaryTrees</u>](https://github.com/SebastianMacaluso/VisualizeBinaryTrees), was developed for this project. There are two types of visualizations.


## 1D Tree-only visualizations

Given a tree structure, *1D tree-only* plots of the tree (with nodes and edges). 

<div class="row justify-content-sm-center">
        <div class="col-sm-7 mt-3 mt-md-0">
        <img class="img-fluid rounded z-depth-1" src="{{ '/assets/img/1D_tree_comparison.png' | relative_url }}" alt="" title="example image"/>
    </div>
</div>
<div class="caption">
1D Tree-only comparison of a sample tree generated with Ginkgo (https://github.com/SebastianMacaluso/ginkgo). We compare the truth-level tree (bottom) with the kt clustering algorithm (kt clustering is a popular greedy algorithm used in particle physics that minimizes a heuristic). The horizontal ordering of the leaves corresponds to the order in which the leaves are accessed when traversing the truth-level tree. 
</div>


## 2D heat clustermaps visualizations


Given a tree structure, 2D heat clustermaps visualizations are created.
 
1) If only one tree is given as input, both rows and columns are ordered according to that tree.

2) If two trees, **A** and **B** are given as input, the visualization can show the heat data map of tree **A**, with columns ordered according to **A**  and rows according to **B**  or viceversa.

Given a pair of tree leaves {i,j} and the number of steps needed for each leaf to reach their closest common ancestor {S_i,S_j}, the heat map scale represents the maximum number of steps, i.e. max{S_i,S_j}.


<div class="row justify-content-sm-center">
        <div class="col-sm-7 mt-3 mt-md-0">
        <img class="img-fluid rounded z-depth-1" src="{{ '/assets/img/heatMap.png' | relative_url }}" alt="" title="example image"/>
    </div>
</div>
<div class="caption">
Heat clustermap plot of the tree corresponding to a dataset generated with Ginkgo (https://github.com/SebastianMacaluso/ginkgo).
</div>