---
title: "AdvART: Adversarial Art for Camouflaged Object Detection Attacks"
collection: publications
permalink: /publications/ICIP24ADVART
venue: "The IEEE International Conference on Image Processing (ICIP) 2024, Abu Dhabi, UAE"
date: 2024-06-07
citation: '<b>Amira Guesmi</b>, Ioan Marius Bilasco, Muhammad Shafique, Ihsen Alouani'
---
[[PDF]]([(https://arxiv.org/abs/2303.01734)])


## Abstract
Physical adversarial attacks pose a significant practical threat as it deceives deep learning systems operating in the real world by producing prominent and maliciously designed physical perturbations. Emphasizing the evaluation of naturalness is crucial in such attacks, as humans can readily detect and eliminate unnatural manipulations. To overcome this limitation, recent work has proposed leveraging generative adversarial networks (GANs) to generate naturalistic patches, which may not catch human's attention. However, these approaches suffer from a limited latent space which leads to an inevitable trade-off between naturalness and attack efficiency. In this paper, we propose a novel approach to generate naturalistic and inconspicuous adversarial patches. Specifically, we redefine the optimization problem by introducing an additional loss term to the cost function. This term works as a semantic constraint to ensure that the generated camouflage pattern holds semantic meaning rather than arbitrary patterns. The additional term leverages similarity metrics to construct a similarity loss that we optimize within the global objective function. Our technique is based on directly manipulating the pixel values in the patch, which gives higher flexibility and larger space compared to the GAN-based techniques that are based on indirectly optimizing the patch by modifying the latent vector. Our attack achieves superior success rate of up to 91.19% and 72%, respectively, in the digital world and when deployed in smart cameras at the edge compared to the GAN-based technique.
