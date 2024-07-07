---
title: "Exploring Machine Learning Privacy/Utility Trade-Off from a Hyperparameters Lens"
collection: publications
permalink: /publications/PRIVACY23
venue: " International Joint Conference on Neural Networks (IJCNN), 2023, Queensland, Australia"
date: 2023-06-18
citation: 'Ayoub Arous, <b>Amira Guesmi</b>, Muhammad Abdullah Hanif, Muhammad Shafique'
---
[[PDF]]([https://ieeexplore.ieee.org/abstract/document/10191743])


## Abstract
Machine Learning (ML) architectures have been applied to several applications that involve sensitive data, where a guarantee of users' data privacy is required. Differentially Private Stochastic Gradient Descent (DPSGD) is the state-of-the-art method to train privacy-preserving models. However, DPSGD comes at a considerable accuracy loss leading to sub-optimal privacy/utility trade-offs. Towards investigating new ground for better privacy-utility trade-off, this work questions; (i) if models' hyperparameters have any inherent impact on ML models' privacy-preserving properties, and (ii) if models' hyperparameters have any impact on the privacy/utility trade-off of differentially private models. We propose a comprehensive design space exploration of different hyperparameters such as the choice of activation functions, the learning rate and the use of batch normalization. Interestingly, we found that utility can be improved by using Bounded RELU as activation functions with the same privacy-preserving characteristics. With a drop-in replacement of the activation function, we achieve new state-of-the-art accuracy on MNIST (96.02%), FashionMnist (84.76%), and CIFAR-10 (44.42%) without any modification of the learning procedure fundamentals of DPSGD.
