---
title: "Anomaly Unveiled: Securing Image Classification against Adversarial Patch Attacks"
collection: publications
permalink: /publications/ICIP24ANOMALY
venue: "The IEEE International Conference on Image Processing (ICIP) 2024, Abu Dhabi, UAE"
date: 2024-06-06
citation: 'Nandish Chattopadhyay, <b>Amira Guesmi</b>, Muhammad Shafique'
---
[[PDF]]([(https://arxiv.org/abs/2402.06249)])


## Abstract
Adversarial patch attacks pose a significant threat to the practical deployment of deep learning systems. However, existing research primarily focuses on image pre-processing defenses, which often result in reduced classification accuracy for clean images and fail to effectively counter physically feasible attacks. In this paper, we investigate the behavior of adversarial patches as anomalies within the distribution of image information and leverage this insight to develop a robust defense strategy. Our proposed defense mechanism utilizes a clustering-based technique called DBSCAN to isolate anomalous image segments, which is carried out by a three-stage pipeline consisting of Segmenting, Isolating, and Blocking phases to identify and mitigate adversarial noise. Upon identifying adversarial components, we neutralize them by replacing them with the mean pixel value, surpassing alternative replacement options. Our model-agnostic defense mechanism is evaluated across multiple models and datasets, demonstrating its effectiveness in countering various adversarial patch attacks in image classification tasks. Our proposed approach significantly improves accuracy, increasing from 38.8% without the defense to 67.1% with the defense against LaVAN and GoogleAp attacks, surpassing prominent state-of-the-art methods such as LGS (53.86%) and Jujutsu (60%)
