---
title: "AdvRain: Adversarial Raindrops to Attack Camera-Based Smart Vision Systems"
collection: publications
permalink: /publications/ADVRAIN
venue: " Information, 2023"
date: 2024-09-20
citation: '<b>Amira Guesmi</b>, Muhammad Abdullah Hanif, Bassem Ouni, Muhammad Shafique'
---
[[PDF]]([https://ieeexplore.ieee.org/abstract/document/10388324])


## Abstract
Vision-based perception modules are increasingly deployed in many applications, especially autonomous vehicles and intelligent robots. These modules are being used to acquire information about the surroundings and identify obstacles. Hence, accurate detection and classification are essential to reach appropriate decisions and take appropriate and safe actions at all times. Current studies have demonstrated that “printed adversarial attacks”, known as physical adversarial attacks, can successfully mislead perception models such as object detectors and image classifiers. However, most of these physical attacks are based on noticeable and eye-catching patterns for generated perturbations making them identifiable/detectable by the human eye, in-field tests, or in test drives. In this paper, we propose a camera-based inconspicuous adversarial attack (AdvRain) capable of fooling camera-based perception systems over all objects of the same class. Unlike mask-based FakeWeather attacks that require access to the underlying computing hardware or image memory, our attack is based on emulating the effects of a natural weather condition (i.e., Raindrops) that can be printed on a translucent sticker, which is externally placed over the lens of a camera whenever an adversary plans to trigger an attack. Note, such perturbations are still inconspicuous in real-world deployments and their presence goes unnoticed due to their association with a natural phenomenon. To accomplish this, we develop an iterative process based on performing a random search aiming to identify critical positions to make sure that the performed transformation is adversarial for a target classifier. Our transformation is based on blurring predefined parts of the captured image corresponding to the areas covered by the raindrop. We achieve a drop in average model accuracy of more than 45% and 40% on VGG19 for ImageNet dataset and Resnet34 for Caltech-101 dataset, respectively, using only 20 raindrops.
