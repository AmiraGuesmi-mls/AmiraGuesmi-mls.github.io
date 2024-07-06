---
title: "Exploring the Interplay of Interpretability and Robustness in Deep Neural Networks: A Saliency-guided Approach"
collection: publications
permalink: /publications/SPVis
venue: "ICIP: Security and Privacy of Machine Learning-based Vision Processing in Autonomous Systems (SPVis), 2024, Abu Dhabi, UAE"
date: 2024-06-27
citation: '<b>Amira Guesmi</b>, Nishant Suresh Aswani, Muhammad Shafique'
---
[[PDF]]([(https://arxiv.org/abs/2405.06278)])



## Abstract
Adversarial attacks pose a significant challenge to deploying deep learning models in safety-critical applications. Maintaining model robustness while ensuring interpretability is vital for fostering trust and comprehension in these models. This study investigates the impact of Saliency-guided Training (SGT) on model robustness, a technique aimed at improving the clarity of saliency maps to deepen understanding of the model's decision-making process. Experiments were conducted on standard benchmark datasets using various deep learning architectures trained with and without SGT. Findings demonstrate that SGT enhances both model robustness and interpretability. Additionally, we propose a novel approach combining SGT with standard adversarial training to achieve even greater robustness while preserving saliency map quality. Our strategy is grounded in the assumption that preserving salient features crucial for correctly classifying adversarial examples enhances model robustness, while masking non-relevant features improves interpretability. Our technique yields significant gains, achieving a 35% and 20% improvement in robustness against PGD attack with noise magnitudes of 0.2 and 0.02 for the MNIST and CIFAR-10 datasets, respectively, while producing high-quality saliency maps.
