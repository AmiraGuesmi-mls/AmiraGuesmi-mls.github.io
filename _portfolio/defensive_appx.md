---
title: "Defensive Approximation: Securing CNNs using Approximate Computing"
collection: portfolio
permalink: /project_pages/defensive_appx/
authors: "Amira Guesmi, Ihsen Alouani, Khaled N. Khasawneh, Mouna Baklouti, Tarek Frikha, Mohamed Abid, Nael Abu-Ghazaleh"
venue: "ASPLOS"
paperurl: "https://doi.org/10.1145/3445814.3446747"
date: 2021-04-19
tags: [Adversarial Robustness, Approximate Computing, Hardware Security, CNNs]
excerpt: "We show that approximate computing can act as a security primitive by injecting input-dependent noise into neural computations. Defensive Approximation leverages hardware-level approximation to disrupt adversarial transferability while improving efficiency."
author_profile: false
topic: "Robustness and Security of Quantized & Approximate Neural Networks"
image: /images/da_method.png
---

## Links
- **Paper:** [Link]({{ page.paperurl }})
{% if page.codeurl and page.codeurl != "" %}- **Code:** [GitHub]({{ page.codeurl }}){% endif %}
{% if page.bibtexurl and page.bibtexurl != "" %}- **BibTeX:** [Download]({{ page.bibtexurl }}){% endif %}

---

## Key Idea
> **Approximate computing is not just a constraint — it can be used as a security primitive to disrupt adversarial attacks.**

---

## Motivation: Why Are Neural Networks Vulnerable?

Adversarial attacks exploit the **deterministic and precise nature** of neural network computations.  
Small, carefully crafted perturbations propagate consistently through layers, enabling reliable attack transferability across models and settings.

<img src="/images/motivation_da.png" alt="Deterministic computations enable adversarial perturbations to propagate consistently" style="max-width:100%; border-radius: 8px;"/>

---

## Insight: Approximation Disrupts Adversarial Consistency

Approximate computing introduces **input-dependent, non-deterministic perturbations** inside neural computations.  
These perturbations break the precise propagation patterns that adversarial attacks rely on, reducing their effectiveness and transferability.

<img src="/images/insight_da.png" alt="Approximate computation injects noise that disrupts adversarial propagation" style="max-width:100%; border-radius: 8px;"/>

---

## Method: Defensive Approximation (DA)

We propose **Defensive Approximation (DA)**, a hardware-level defense that integrates approximate computing directly into CNN operations.

Instead of modifying training or preprocessing inputs, DA:
- replaces exact multipliers with **approximate arithmetic units**
- injects **data-dependent perturbations during computation**
- disrupts adversarial signal propagation across layers  

This enables robustness **without retraining or architectural changes**, while simultaneously improving efficiency.

<img src="/images/implement_da.png" alt="DA integrates approximate multipliers into CNN computations to inject controlled noise" style="max-width:100%; border-radius: 8px;"/>

---

## Positioning

Unlike traditional defenses that operate in input space (preprocessing) or model space (training), DA operates at the **hardware level**, directly modifying the computation itself.

This reframes approximate computing from a performance optimization tool into a **robustness and security mechanism**, bridging hardware design and adversarial machine learning.

---

## Abstract

Adversarial attacks pose a serious threat to machine learning systems deployed in safety- and security-critical domains.  
We propose **Defensive Approximation (DA)**, a novel defense mechanism that leverages approximate computing at the hardware level to improve the robustness of convolutional neural networks (CNNs) against adversarial attacks.

By replacing exact floating-point multipliers with aggressively approximate ones, DA introduces **input-dependent perturbations throughout the computation pipeline**, disrupting adversarial signal propagation and reducing attack transferability in gray-box, black-box, and even white-box settings.

Importantly, this robustness is achieved **without retraining**, while also reducing energy consumption and latency.

Extensive experiments on MNIST and CIFAR-10 demonstrate robustness improvements of up to **99%** against strong transferability-based attacks, along with up to **50% energy savings**.

---

## Key Contributions

- We show that **approximate computing can act as a security primitive** against adversarial attacks.  
- We introduce **Defensive Approximation (DA)**, a hardware-level defense integrated into CNN computations.  
- We demonstrate strong robustness across **white-box, black-box, and transfer-based attacks**.  
- We achieve robustness **without retraining or architectural modification**.  
- We provide simultaneous gains in **energy efficiency and latency reduction**.  

---

## Mechanism: How DA Improves Robustness

DA injects controlled perturbations into intermediate computations, disrupting the alignment and propagation of adversarial signals across layers.

<img src="/images/mechanism_da.png" alt="Approximation disrupts adversarial signal propagation across layers" style="max-width:100%; border-radius: 8px;"/>

---

## Results: Robustness Meets Efficiency

DA achieves strong adversarial robustness while improving system efficiency:

- Up to **99% reduction in attack success rate**  
- Robustness across multiple threat models  
- Up to **50% energy savings**  
- Minimal impact on clean accuracy  

<img src="/images/rsults_da.png" alt="DA improves robustness while reducing energy and latency" style="max-width:100%; border-radius: 8px;"/>

---

## Impact and Research Directions

This work established a new perspective on robustness at the intersection of hardware and machine learning, enabling:

- Robustness in **quantized and approximate neural networks**  
- **Hardware–software co-design** for AI security  
- Transferability disruption via **non-deterministic computation**  

---

## Citation
```bibtex
@inproceedings{guesmi2021defensive,
  title={Defensive approximation: securing cnns using approximate computing},
  author={Guesmi, Amira and Alouani, Ihsen and Khasawneh, Khaled N and Baklouti, Mouna and Frikha, Tarek and Abid, Mohamed and Abu-Ghazaleh, Nael},
  booktitle={Proceedings of the 26th ACM international conference on architectural support for programming languages and operating systems},
  pages={990--1003},
  year={2021}
}
```
