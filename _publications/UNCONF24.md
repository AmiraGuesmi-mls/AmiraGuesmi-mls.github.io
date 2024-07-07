---
title: "Examining Changes in Internal Representations of Continual Learning Models Through Tensor Decomposition"
collection: publications
permalink: /publications/UNCONF24
venue: "ContinualAI Unconference, 2023, Virtual"
date: 2024-06-30
citation: 'Nishant Suresh Aswani, <b>Amira Guesmi</b>, Muhammad Abdullah Hanif, Muhammad Shafique'
---
[[PDF]]([(https://arxiv.org/abs/2405.03244)])


## Abstract
Continual learning (CL) has spurred the development of several methods aimed at consolidating previous knowledge across sequential learning. Yet, the evaluations of these methods have primarily focused on the final output, such as changes in the accuracy of predicted classes, overlooking the issue of representational forgetting within the model. In this paper, we propose a novel representation-based evaluation framework for CL models. This approach involves gathering internal representations from throughout the continual learning process and formulating three-dimensional tensors. The tensors are formed by stacking representations, such as layer activations, generated from several inputs and model `snapshots', throughout the learning process. By conducting tensor component analysis (TCA), we aim to uncover meaningful patterns about how the internal representations evolve, expecting to highlight the merits or shortcomings of examined CL strategies. We conduct our analyses across different model architectures and importance-based continual learning strategies, with a curated task selection. While the results of our approach mirror the difference in performance of various CL strategies, we found that our methodology did not directly highlight specialized clusters of neurons, nor provide an immediate understanding the evolution of filters. We believe a scaled down version of our approach will provide insight into the benefits and pitfalls of using TCA to study continual learning dynamics.
