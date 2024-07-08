---
title: "Adversarial Attack on Radar-based Environment Perception Systems"
collection: publications
permalink: /publications/ARADAR
venue: "ArXiv"
date: 2022-11-28
citation: '<b>Amira Guesmi</b>, Ihsen Alouani'
---
[[PDF]]([(https://arxiv.org/abs/2211.01112)])


## Abstract
Due to their robustness to degraded capturing conditions, radars are widely used for environment perception, which is a critical task in applications like autonomous vehicles. More specifically, Ultra-Wide Band (UWB) radars are particularly efficient for short range settings as they carry rich information on the environment. Recent UWB-based systems rely on Machine Learning (ML) to exploit the rich signature of these sensors. However, ML classifiers are susceptible to adversarial examples, which are created from raw data to fool the classifier such that it assigns the input to the wrong class. These attacks represent a serious threat to systems integrity, especially for safety-critical applications. In this work, we present a new adversarial attack on UWB radars in which an adversary injects adversarial radio noise in the wireless channel to cause an obstacle recognition failure. First, based on signals collected in real-life environment, we show that conventional attacks fail to generate robust noise under realistic conditions. We propose a-RNA, i.e., Adversarial Radio Noise Attack to overcome these issues. Specifically, a-RNA generates an adversarial noise that is efficient without synchronization between the input signal and the noise. Moreover, a-RNA generated noise is, by-design, robust against pre-processing countermeasures such as filtering-based defenses. Moreover, in addition to the undetectability objective by limiting the noise magnitude budget, a-RNA is also efficient in the presence of sophisticated defenses in the spectral domain by introducing a frequency budget. We believe this work should alert about potentially critical implementations of adversarial attacks on radar systems that should be taken seriously.
