---
title: "SAAM: Stealthy Adversarial Attack on Monocular Depth Estimation"
collection: publications
permalink: /publications/SAAM
venue: " The IEEE Access, 2024"
date: 2024-01-11
citation: '<b>Amira Guesmi</b>, Muhammad Abdullah Hanif, Bassem Ouni, Muhammad Shafique'
---
[[PDF]]([https://ieeexplore.ieee.org/abstract/document/10388324])


## Abstract
Monocular depth estimation (MDE) is an important task in scene understanding, and significant improvements in its performance have been witnessed with the utilization of convolutional neural networks (CNNs). These models can now be deployed on edge devices, thanks to advancements in CNN optimization, enabling effective depth estimation in safety-critical and security-sensitive systems like robots, rovers, drones, and autonomous cars. However, CNNs used for MDE are susceptible to adversarial attacks, which can be exploited for malicious purposes by generating plausible images containing carefully crafted perturbations that distort the model’s output. To assess the vulnerability of CNN-based depth prediction methods, recent studies have attempted to design adversarial patches specifically targeting MDE. However, these methods have not been powerful enough to fully deceive the vision system in a systemically threatening manner. Their impact is less effective, misleading the depth prediction of only certain parts within the overlapping region of the input image by using conspicuous and eye-catching patterns. In this paper, we investigate the vulnerability of MDE to adversarial patches. We propose a novel S tealthy A dversarial A ttacks on M DE (SAAM) that compromises MDE by either corrupting the estimated distance or causing an object to seamlessly blend into its surroundings. Our experiments demonstrate that the designed stealthy patch successfully causes a CNN to misestimate the depth of objects. In fact, our proposed adversarial patch achieves a significant 60% depth error with 99% ratio of the affected region. Importantly, despite its adversarial nature, the patch maintains a naturalistic appearance, making it inconspicuous to human observers. We believe that this work sheds light on the threat of adversarial attacks in the context of MDE on edge devices. We hope it raises awareness within the community about the potential real-life harm of such attacks and encourages further research into developing more robust and adaptive defense mechanisms.
