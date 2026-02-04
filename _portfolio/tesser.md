---
title: "TESSER: Transfer-Enhancing Adversarial Attacks from Vision Transformers via Spectral and Semantic Regularization"
collection: portfolio
permalink: /project_pages/tesser/
date: 2025-05-15
venue: "arXiv"
paperurl: "https://arxiv.org/abs/2505.19613"
codeurl: ""
bibtexurl: ""
authors: "Amira Guesmi, Bassem Ouni, Muhammad Shafique" 
excerpt: "A framework that significantly improves black-box adversarial attack transferability from Vision Transformers via spectral and semantic regularization."
topic: "Adversarial Machine Learning — Foundations"

header:
  image: /images/tesser_overview.png
  caption: "Overview of the TESSER framework."
---

## Links
- **Paper:** [arXiv]({{ page.paperurl }})
{% if page.codeurl and page.codeurl != "" %}- **Code:** [GitHub]({{ page.codeurl }}){% endif %}
{% if page.bibtexurl and page.bibtexurl != "" %}- **BibTeX:** [Download]({{ page.bibtexurl }}){% endif %}

## Overview
<img src="{{ page.header.image | relative_url }}" alt="TESSER Overview" style="max-width:100%; border-radius: 8px;"/>

## Abstract

*Adversarial transferability remains a critical challenge in evaluating the robustness of deep neural networks. In security-critical applications, transferability enables
black-box attacks without access to model internals, making it a key concern for real-world adversarial threat assessment. While Vision Transformers (ViTs) have
demonstrated strong adversarial performance, existing attacks often fail to transfer effectively across architectures, especially from ViTs to Convolutional Neural
Networks (CNNs) or hybrid models. In this paper, we introduce TESSER — a novel adversarial attack framework that enhances transferability via two key strategies: (1) Feature-Sensitive Gradient Scaling (FSGS), which modulates gradients
based on token-wise importance derived from intermediate feature activations, and (2) Spectral Smoothness Regularization (SSR), which suppresses high-frequency
noise in perturbations using a differentiable Gaussian prior. These components work in tandem to generate perturbations that are both semantically meaningful
and spectrally smooth. Extensive experiments on ImageNet across 12 diverse architectures demonstrate that TESSER achieves +10.9% higher attack succes rate (ASR) on CNNs and +7.2% on ViTs compared to the state-of-the-art Adaptive Token Tuning (ATT) method. Moreover, TESSER significantly improves robustness
against defended models, achieving 53.55% ASR on adversarially trained CNNs. Qualitative analysis shows strong alignment between TESSER’s perturbations and
salient visual regions identified via Grad-CAM, while frequency-domain analysis reveals a 12% reduction in high-frequency energy, confirming the effectiveness of spectral regularization.*

## Key Contributions
-  We propose TESSER, a novel adversarial attack framework that explicitly couples semantic selectivity and spectral smoothness during optimization, identifying
semantic–spectral compatibility as a previously underexplored and necessary condition for adversarial transferability across heterogeneous architectures.
- We introduce Feature-Sensitive Gradient Scaling (FSGS), a token-aware and depth-sensitive gradient modulation mechanism that dynamically reweights gradients in Attention, QKV, and MLP modules based
on intermediate feature importance, steering perturbations toward semantically meaningful regions while suppressing architecture-specific noise.
- We incorporate Spectral Smoothness Regularization (SSR), a lightweight differentiable spectral prior that suppresses high-frequency perturbation artifacts during optimization, promoting low-frequency structures that generalize effectively across CNNs, ViTs, and adversarially trained models.
- We conduct extensive experiments on ImageNet across 14 diverse architectures, including Vision Transformers, CNNs, hybrid models, and adversarially defended networks, showing that TESSER consistently outperforms state-of-the-art transfer attacks, achieving up to +10.9% higher ASR in challenging black-box and robust settings.
- We provide comprehensive ablation studies, GradCAM-based semantic alignment analyses (Section 4.4), and frequency-domain evaluations (Section 4.5) that validate the necessity and effectiveness of jointly enforcing semantic alignment and spectral smoothness for adversarial transferability.

## Citation
```bibtex
@article{guesmi2025tesser,
  title     = {TESSER: Transfer-Enhancing Adversarial Attacks from Vision Transformers via Spectral and Semantic Regularization},
  author    = {Guesmi, Amira and <Other Authors>},
  journal   = {arXiv},
  volume    = {abs/2505.19613},
  year      = {2025}
}
