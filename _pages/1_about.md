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

sebastian.macaluso@telefonica.com <br> 
<br> 
Senior researcher at <a href="https://www.telefonica.com/en/sustainability-innovation/innovation/telefonica-research/">Telefonica Research</a> developing novel deep reinforcement learning, deep learning and quantum computing algorithms to tackle problems involving management and orchestration of telecom networks, cryptography, human-computer interaction, clustering and recommender systems. I am also leading Horizon Europe proposals submission and co-advising PhD and Masters students.
<br>
<br>
Previously, I was a postdoctoral researcher in  <a href="https://twitter.com/kylecranmer">Kyle Cranmer</a>'s group at New York University, at the Center for Cosmology and Particle Physics & the Center for Data Science until recently, working at the intersection of particle physics and machine learning, with emphasis on deep learning techniques on structured data, statistical inference and combinatorial optimization.
<br>






My background is in deep learning, particle physics and statistical inference. I obtained my PhD in physics at the <a href="https://www.physics.rutgers.edu/het/">New High Energy Theory Center</a> at Rutgers University, advised by Prof. <a href="https://physics.rutgers.edu/people/faculty-list/faculty-profile/shih-david">David Shih</a>. During my postdoc and PhD I had the pleasure to collaborate with <a href="https://twitter.com/kylecranmer">Kyle Cranmer</a> (NYU/UWMadison), <a href="https://people.cs.umass.edu/~nmonath/">  Nicholas Monath </a> (Google), <a href="https://scholar.google.com/citations?user=XXPetHMAAAAJ&hl=en"> Craig Greenberg </a> (NIST), <a href="https://johannbrehmer.github.io/">  Johann Brehmer</a> (Qualcomm), <a href="https://physics.rutgers.edu/people/faculty-list/faculty-profile/shih-david">David Shih</a> (Rutgers), <a href="https://scholar.google.com/citations?hl=en&user=_AezOKYAAAAJ&view_op=list_works&sortby=pubdate"> Duccio Pappadopulo </a> (Bloomberg), <a href="https://people.math.umass.edu/~flaherty/member/patrickflaherty/"> Patrick Flaherty </a> (UMass), <a href="http://www.physicsmatt.com/"> Matthew  Buckley  </a> (Rutgers), and more (see <a href="/Papers/">Papers</a> section)!


# Research Interests & Past Experience

I am broadly interested in deep reinforcement learning, deep learning, statistical modeling and quantum computing algorithms, involving discrete combinatorial optimization, LLMs and natural language processing, (hierarchical) clustering, regression, classification, recommender systems, management and orchestration tasks. 

I developed machine/deep learning algorithms, including probabilistic modeling, neural architectures for supervised tasks, as well as unsupervised settings involving combinatorial optimization problems. Potential applications include natural language processing (NLP), such as record linkage or semantic parsing and structure prediction, both in NLP as well as natural sciences such as jet sub-structure in particle physics or phylogenetic trees.



#### Natural Language Processing - Clustering - Deep Learning

- Worked on supervised classification and regression of sequence models on tree structured data. I worked on a new perspective that proposes an analogy between  physics data and natural languages. In particular, I developed a GPU batch training pipeline on PyTorch for a Recursive (tree based) Neural Network, <a href="/projects/3_project_treenin/"><u>TreeNiN</u></a>. I implemented architectures including Network in Network layers, split weights, bi-directional architectures and gated units. The final classifier was among the top three performing algorithms for particle physics data (top jets) while having an order of magnitude fewer parameters than the other ones. Also, I am interested in the interplay between inductive bias and the generality of the deep learning model.
- Developed new algorithms, <a href="/projects/2_project_trellis/"><u>Cluster Trellis</u></a>    and <a href="/projects/1_project_astar/"><u>Hierarchical Clustering with A*</u></a> for (exact) inference in hierarchical clusterings (MAP, partition function, marginals and posterior sampling), seen as a combinatorial optimization problem.  These exact algorithms resulted in a super-exponential improvement on the time complexity compared to brute force methods and scale beyond previous state-of-the-art, from a search space with 10<sup>12</sup> trees to 10<sup>15</sup> trees [[<u> UAI 2021 </u>]](https://www.auai.org/uai2021/pdf/uai2021.770.pdf), [[<u> AISTATS 2021 </u>]](http://proceedings.mlr.press/v130/macaluso21a/macaluso21a.pdf) and  [[<u> ML4PS @NeurIPS 2020 </u>]](https://ml4physicalsciences.github.io/2020/files/NeurIPS_ML4PS_2020_70.pdf).
- Introduced the quantum trellis, a classical data structure and dynamic programming algorithm to efficiently compute the un-normalized probability density (marginal likelihood) including all interference effects, given a fixed number of tree leaves.  I paired the trellis with an MCMC-based sampling strategy using the emcee library. This provides a potential path forward for classical computers and a strong baseline for approaches based on
quantum computing [[<u> ML4PS @NeurIPS 2021 </u>]](https://ml4physicalsciences.github.io/2021/files/NeurIPS_ML4PS_2021_107.pdf).
- Worked on a reinforcement learning algorithm to find the MAP hierarchical clustering on simulated particle physics datasets, where the leaves are known but the tree structure is latent [[<u> ML4PS @NeurIPS 2020 </u>]](https://ml4physicalsciences.github.io/2020/files/NeurIPS_ML4PS_2020_2.pdf). 
- Implemented <a href="/projects/5_project/"><u>beam search and greedy</u></a> algorithms for inference in hierarchical clusterings and developed  <a href="/projects/7_project_visualizations/"><u>visualizations</u></a> for comparisons among them. 
- I am currently working on a paper on a new algorithm for micro-clustering, with potential applications on tasks such as entity resolution, author name disambiguation and record linkage.

#### Computer Vision - Deep Learning 

- Developed a training pipeline to apply state-of-the-art computer vision techniques to particle physics data using Keras and TensorFlow. Designed and implemented an <a href="/projects/4_project_vision/"><u>object classifier</u></a> for physics data based on convolutional neural
networks that improved performance by a factor of 10 over the previous state-of-the-art.
- Generated (from simulations) millions of images and pre-processed them (center, rotate to vertically align the major principal axis, flip, and normalize).

#### Numerical Simulations and Analyses

- Developed in Pyro <a href="/projects/6_project_ginkgo/"><u>Ginkgo</u></a>: a simplified generative model for particle physics to facilitate research implementing probabilistic, differentiable, dynamic programing and variational inference. It is analogous to ground-truth parse trees with a known language model.
- Ran distributed computing analyses and simulation calculations of 10 TB datasets on hundreds of nodes across the scientific grid.
- Designed and optimized an analysis in C++ that led to discovery sensitivities of new particles
at the Large Hadron Collider. 

#### External Projects 

- Implemented topic modeling (LDA) to group incoming messages for an EdTech startup. Performed data preprocessing (cleaning, tokenization, bigram and trigram models, stop words, lemmatization), clustering and visualization of topics.


# Education

- Ph.D. in Physics,  Department of Physics & Astronomy, Rutgers University, USA, 2012-2018. Ph.D. advisor Prof. David Shih.

- Licenciatura en Ciencias Fisicas (B.A. in Physics), University of Buenos Aires, Argentina, 2011.


# Publications

See <a href="/Papers/">Papers</a> section.

# Awards

- Seal of Excellence, European Comission, HORIZON-EIC-2023-PATHFINDEROPEN.
- Spotlight talk, ``Exact and Approximate Hierarchical Clustering Using A*", UAI 2021.
- NVIDIA GPU Grant, Dec. 2018.
- Richard J. Plano Outstanding Teaching Assistant Award, Rutgers University, 2014.

# Reviewer

- NeurIPS (MLPS).
- Journal of High Energy Physics (JHEP).
- European Physical Journal C.


# Organizing Committee Member at Workshops 

- Third international workshop on Machine Learning for Jet Physics, <a href="https://indico.cern.ch/event/809820/overview">[ML4Jets2020]</a>, New York University, USA, January 15-17, 2020.

# Invited Seminar Speaker

See <a href="/Talks/">Talks</a> section.

# Teaching Experience

- Elements of Physics 161, Rutgers University: Fall 2012.
- Extended General Physics 201, Rutgers University: Spring 2013, 2014.
- Physics 203, Rutgers University: Summer 2013, 2014. Fall 2013.
- Physics 204, Rutgers University: Summer 2013.








