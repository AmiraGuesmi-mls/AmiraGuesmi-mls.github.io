---
title: "ODDR: Outlier Detection & Dimension Reduction Based Defense Against Adversarial Patches"
collection: publications
permalink: /publications/ODDR
venue: "ArXiv"
date: 2023-11-20
citation: 'Nandish Chattopadhyay, <b>Amira Guesmi</b>, Muhammad Abdullah Hanif, Bassem Ouni, Muhammad Shafique'
---
[[PDF]]([(https://arxiv.org/abs/2311.12084)])


## Abstract
Adversarial attacks are a major deterrent towards the reliable use of machine learning models. A powerful type of adversarial attacks is the patch-based attack, wherein the adversarial perturbations modify localized patches or specific areas within the images to deceive the trained machine learning model. In this paper, we introduce Outlier Detection and Dimension Reduction (ODDR), a holistic defense mechanism designed to effectively mitigate patch-based adversarial attacks. In our approach, we posit that input features corresponding to adversarial patches, whether naturalistic or otherwise, deviate from the inherent distribution of the remaining image sample and can be identified as outliers or anomalies. ODDR employs a three-stage pipeline: Fragmentation, Segregation, and Neutralization, providing a model-agnostic solution applicable to both image classification and object detection tasks. The Fragmentation stage parses the samples into chunks for the subsequent Segregation process. Here, outlier detection techniques identify and segregate the anomalous features associated with adversarial perturbations. The Neutralization stage utilizes dimension reduction methods on the outliers to mitigate the impact of adversarial perturbations without sacrificing pertinent information necessary for the machine learning task. Extensive testing on benchmark datasets and state-of-the-art adversarial patches demonstrates the effectiveness of ODDR. Results indicate robust accuracies matching and lying within a small range of clean accuracies (1%-3% for classification and 3%-5% for object detection), with only a marginal compromise of 1%-2% in performance on clean samples, thereby significantly outperforming other defenses.
