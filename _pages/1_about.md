---
layout: about
title: About
permalink: /
nav: false
horizontal: false

profile:
  align: left
  image: CentralPark_square.jpg
  


social: true  # includes social icons at the bottom of the page



---


# Sebastian Macaluso

seb.macaluso@nyu.edu <br> 
<br> 
I am a postdoctoral researcher in  <a href="https://twitter.com/kylecranmer">Kyle Cranmer</a>'s group at New York University, at the Center for Data Science & the Center for Cosmology and Particle Physics.
<br>
<br> 
**I AM ON THE JOB MARKET FOR MACHINE LEARNING RESEARCH POSITIONS IN INDUSTRY.**
<br>

I work developing machine learning algorithms, including probabilistic modeling, neural architectures for supervised tasks, as well as unsupervised settings involving combinatorial optimization problems, with applications to natural language processing and structure prediction. These algorithms have practical applications in particle physics, genomics and phylogenetics, among other areas. I'm excited about bringing together techniques from different fields to solve complex problems.

My background is in particle physics and machine learning. I obtained my PhD in physics at the <a href="https://www.physics.rutgers.edu/het/">New High Energy Theory Center</a> at Rutgers University, advised by Prof. <a href="https://physics.rutgers.edu/people/faculty-list/faculty-profile/shih-david">David Shih</a>. During my postdoc and PhD I had the pleasure to collaborate with <a href="https://twitter.com/kylecranmer">Kyle Cranmer</a> (NYU/UWMadison), <a href="https://people.cs.umass.edu/~nmonath/">  Nicholas Monath </a> (Google), <a href="https://scholar.google.com/citations?user=XXPetHMAAAAJ&hl=en"> Craig Greenberg </a> (NIST), <a href="https://johannbrehmer.github.io/">  Johann Brehmer</a> (Qualcomm), <a href="https://physics.rutgers.edu/people/faculty-list/faculty-profile/shih-david">David Shih</a> (Rutgers), <a href="https://scholar.google.com/citations?hl=en&user=_AezOKYAAAAJ&view_op=list_works&sortby=pubdate"> Duccio Pappadopulo </a> (Bloomberg), <a href="https://people.math.umass.edu/~flaherty/member/patrickflaherty/"> Patrick Flaherty </a> (UMass), <a href="http://www.physicsmatt.com/"> Matthew  Buckley  </a> (Rutgers), and more (see <a href="/Papers/">Papers</a> section)!


# Research Interests & experience

I am broadly interested in machine learning explainability, causality and inductive bias, as well as combinatorial optimization, including areas such as (hierarchical) clustering, variational inference, simulations, probabilistic inference, and reinforcement learning.

###### NATURAL LANGUAGE PROCESSING - CLUSTERING - DEEP LEARNING

- Worked on supervised classification and regression of sequence models on tree structured data. I worked on a new perspective that proposes an analogy between  physics data and natural languages. In particular I developed a GPU batch training pipeline on PyTorch for a Recursive (tree based) Neural Network <a href="/projects/3_project_treenin/"><u>TreeNiN</u></a>. Implemented architectures including Network in Network layers, split weights, bi-directional architectures and gated units. The final classifier was among the top three performing algorithms to classify particle physics data (top jets) while having an order of magnitude fewer parameters than the other ones. 
- Developed new algorithms, <a href="/projects/2_project_trellis/"><u>Cluster Trellis</u></a>    and <a href="/projects/1_project_astar/"><u>Hierarchical Clustering with A*</u></a> for (exact) inference in hierarchical clusterings (MAP, partition function, marginals and posterior sampling), seen as a combinatorial optimization problem.  Exact algorithms scale beyond previous state-of-the-art, from a search space with 10<sup>12</sup> trees to 10<sup>15</sup> trees (UAI 2021, AISTATS 2021 and ML4PS @NeurIPS 2020 publications).
- Worked on a reinforcement learning algorithm to find the MAP hierarchical clustering for particle physics datasets, where the leaves are known but the tree structure is latent (ML4PS @NeurIPS 2021). 
- Implemented <a href="/projects/5_project/"><u>beam search and greedy</u></a> algorithms for inference in hierarchical clusterings and developed  <a href="/projects/7_project_visualizations/"><u>visualizations</u></a> for comparisons among them. 
- I am currently working on a paper on a new algorithm for micro-clustering, for tasks such as entity resolution, author name disambiguation and record linkage.

###### COMPUTER VISION - DEEP LEARNING

- Developed a training pipeline to apply state-of-the-art computer vision techniques to particle physics data using Keras and TensorFlow. Designed and implemented an <a href="/projects/4_project_vision/"><u>object classifier</u></a> for physics data based on convolutional neural
networks that improved performance by a factor of 10 over the previous state-of-the-art.
- Generated (from simulations) millions of images and pre-processed them (center, rotate to vertically align the major principal axis, flip, and normalize).

###### NUMERICAL SIMULATIONS AND ANALYSES

- Developed in Pyro <a href="/projects/6_project_ginkgo/"><u>Ginkgo</u></a>: a simplified generative model for particle physics to facilitate research implementing probabilistic, differentiable, dynamic programing and variational inference. It is analogous to ground-truth parse trees with a known language model.
- Ran distributed computing analyses and simulation calculations of 10 TB datasets on hundreds of nodes across the scientific grid.
- Designed and optimized an analysis in C++ that led to discovery sensitivities of new particles
at the Large Hadron Collider. 
