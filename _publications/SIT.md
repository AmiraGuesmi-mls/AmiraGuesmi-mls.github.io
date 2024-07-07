---
title: "SIT: Stochastic Input Transformation to Defend Against Adversarial Attacks on Deep Neural Networks"
collection: publications
permalink: /publications/SIT
venue: " The IEEE Design & Test, 2022"
date: 2022-06-01
citation: '<b>Amira Guesmi</b>, Ihsen Alouani, Mouna Baklouti, Tarek Frikha, Mohamed Abid'
---
[[PDF]]([https://ieeexplore.ieee.org/document/9422778])


## Abstract
Deep Neural Networks (DNNs) have been deployed in a wide range of applications, including safety-critical domains, owing to their proven efficiency in solving complex problems. However, these systems have been shown vulnerable to ad-versarial attacks: carefully crafted perturbations that threaten their integrity and trustworthiness. Several defenses have been recently proposed. However, most of these techniques are costly to deploy since they require retraining and specific fine-tuning procedures. While there are pre-processing defenses that do not require retraining, these were shown to be ineffective against adaptive white-box attacks. In this paper, we propose a model-agnostic defense against adversarial attacks using stochastic pre-processing. Based on a process of down-sampling/up-sampling, we transform the input to a new sample that is: (i) close enough to the initial input to be classified correctly, and (ii) different enough to ignore any potential adversarial noise within it. The proposed defense is generic, easy to deploy and does not require any specific training or fine tuning. We tested our technique comparatively to state-of-the-art defenses under grey-box and strong white-box scenarios. Experimental results show that our defense achieves robustness of up to 94% and 93% against PGD and C&W attacks, respectively, under strong white-box scenario.
