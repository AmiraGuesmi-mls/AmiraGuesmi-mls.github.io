---
title: "ROOM: Adversarial Machine Learning Attacks Under Real-Time Constraints"
collection: publications
permalink: /publications/ROOM
venue: " International Joint Conference on Neural Networks (IJCNN), 2022, Padua, Italy"
date: 2022-07-23
citation: <b>Amira Guesmi</b>, Khaled N. Khasawneh, Nael Abu-Ghazaleh, Ihsen Alouani'
---
[[PDF]]([https://ieeexplore.ieee.org/document/9892437])


## Abstract
Advances in deep-learning have enabled a wide range of promising applications. However, these systems are vulnerable to adversarial attacks; adversarially crafted pertur-bations to their inputs could cause them to misclassify. Most state-of-the-art adversarial attack generation algorithms focus primarily on controlling the noise magnitude to make it undetectable. The execution time is a secondary consideration for these attacks and the underlying assumption is that there are no time constraints. However, just-in-time adversarial attacks where an attacker opportunistically generates adversarial examples on-the-fly represent an even more critical threat, especially against real-time applications. Therefore, this paper introduces a new problem: how to systematically generate adversarial noise under real-time constraints? Understanding this problem improves our understanding of the threat these attacks pose to real-time systems and provides security evaluation benchmarks for future defenses. Therefore, first, we conduct a run-time analysis of adversarial generation algorithms. Our analysis show that universal attacks produce a general attack offline, with no online overhead. However, their success rate is limited because of their generality. In contrast, online algorithms, which target a specific input, are computationally expensive, making them inappropriate under time constraints. Thus, we propose ROOM, a novel Real-time Online-Offline attack construction Model where an offline component warms up the online algorithm, making it possible to generate highly successful attacks under time constraints. Our results show that ROOM can achieve high attack success rates under real-time constraints with up to 90x faster adversarial attack generation than state-of-the-art methods. For example, ROOM achieves 100% adversarial attack success rate on MNIST with a throughput of up to 1250 frame per second (FPS), more than 60% success rate with 200 FPS on CIFAR-10 and 60% with 16 FPS on ImageNet.
