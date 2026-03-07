---
title: "Defensive Approximation: Securing CNNs using Approximate Computing"
collection: portfolio
permalink: /portfolio/defensive-approximation/
authors: "Amira Guesmi, Ihsen Alouani, Khaled N. Khasawneh, Mouna Baklouti, Tarek Frikha, Mohamed Abid, Nael Abu-Ghazaleh"
venue: "ASPLOS"
paper_url: "https://doi.org/10.1145/3445814.3446747"
date: 2021-04-19
tags: [Adversarial Robustness, Approximate Computing, Hardware Security, CNNs]
excerpt: "A hardware-level defense that leverages approximate computing to improve robustness of CNNs against adversarial attacks while reducing energy consumption."
author_profile: false
topic: "Robustness and Security of Quantized & Approximate Neural Networks"

image: /images/asplos_overview.png


---

## Links
- **Paper:** [Link]({{ [page.paperurl ](https://dl.acm.org/doi/10.1145/3445814.3446747) }})
{% if page.codeurl and page.codeurl != "" %}- **Code:** [GitHub]({{ page.codeurl }}){% endif %}
{% if page.bibtexurl and page.bibtexurl != "" %}- **BibTeX:** [Download]({{ page.bibtexurl }}){% endif %}

## Overview

<img src="{{ page.image | relative_url }}" alt="Defensive Approximation (DA) overview" style="max-width:100%; border-radius: 8px;"/>

**Defensive Approximation (DA)** is the first work to demonstrate that *hardware-supported approximate computing* can be used as an **effective defense against adversarial attacks** on deep neural networks. Instead of modifying training or preprocessing inputs, DA injects **data-dependent approximation noise directly inside CNN computations**, fundamentally disrupting adversarial transferability while preserving accuracy and improving efficiency.


## Abstract

Adversarial attacks pose a serious threat to machine learning systems deployed in safety- and security-critical domains.  
This paper proposes **Defensive Approximation**, a novel defense mechanism that leverages **approximate computing at the hardware level** to improve robustness of convolutional neural networks (CNNs) against adversarial attacks. By replacing exact floating-point multipliers with aggressively approximate ones, the proposed approach introduces **input-dependent perturbations throughout the model**, significantly reducing attack transferability in gray-box, black-box, and even white-box settings.  
Importantly, this robustness is achieved **without retraining**, while simultaneously reducing energy consumption and latency.
Extensive experiments on MNIST and CIFAR-10 demonstrate robustness improvements of up to **99%** against strong transferability-based attacks, with up to **50% energy savings**.


## Key Contributions

- **First hardware-level adversarial defense** using approximate computing  
- Strong robustness against:
  - Transferability attacks  
  - Black-box attacks  
  - White-box attacks  
- No retraining or model modification required  
- Significant **energy and latency reduction**  
- Improves model confidence while preserving accuracy  


## Related Research Directions

This work laid the foundation for later research on:
- Robustness of quantized and approximate neural networks  
- Hardware–software co-design for AI security  
- Transferability disruption via non-deterministic computation  

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
