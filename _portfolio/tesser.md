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

image: /images/tesser_method.png
---

## Core Insight

Adversarial transferability fails when perturbations are **too specific** to the source model.

TESSER shows that transferable attacks must preserve **shared semantic and spectral structure**, not just maximize loss on a surrogate model.

---

## Links
- **Paper:** [arXiv](https://arxiv.org/abs/2505.19613)

---

## Motivation

Adversarial transferability enables black-box attacks by allowing perturbations crafted on one model to generalize to others.

However, transferability is limited across architectures:
- Vision Transformers → CNNs  
- CNNs → Transformers  

<img src="/images/fail_tesser.png" style="max-width:100%; border-radius:8px;"/>

Why?

Because standard attacks:
- overfit to **local, architecture-specific features**
- rely on **high-frequency artifacts** that do not generalize

---

## What Enables Transferability?

<img src="/images/requires_tesser.png" style="max-width:100%; border-radius:8px;"/>

Transferable perturbations must preserve:

- **Semantic alignment** → focus on meaningful features  
- **Spectral consistency** → avoid high-frequency noise  

> Transferability emerges from **shared structure across models**.

---

## Intuition

<img src="/images/fsgs_tesser.png" style="max-width:100%; border-radius:8px;"/>

**Feature-Sensitive Gradient Scaling (FSGS)**  
→ reallocates gradients toward semantically meaningful tokens  
→ suppresses non-transferable low-level features  

<img src="/images/ssr_tesser.png" style="max-width:100%; border-radius:8px;"/>

**Spectral Smoothness Regularization (SSR)**  
→ suppresses high-frequency components  
→ promotes smoother, more transferable perturbations  

---

## Method Overview

<img src="/images/tesser_method.png" style="max-width:100%; border-radius:8px;"/>

TESSER is a unified framework combining:

1. **FSGS**  
   → controls *where* gradients act (semantic structure)

2. **SSR**  
   → controls *how* perturbations behave (frequency structure)

Together, they enforce perturbations that are:
- semantically aligned  
- spectrally coherent  
- robust across architectures  

---

## Abstract

Adversarial transferability enables black-box attacks by allowing perturbations crafted on a surrogate model to generalize to unseen targets. However, transferability remains limited across architectures, particularly from Vision Transformers (ViTs) to Convolutional Neural Networks (CNNs), due to over-reliance on local, architecture-specific features and high-frequency, non-transferable artifacts.

We propose **TESSER (Transfer-Enhancing Semantic and Spectral Regularization)**, a unified adversarial attack framework that improves transferability by jointly controlling gradient allocation and spectral structure. TESSER integrates **Feature-Sensitive Gradient Scaling (FSGS)**, which rebalances gradients toward semantically meaningful features, and **Spectral Smoothness Regularization (SSR)**, which suppresses high-frequency components to promote smoother and more transferable perturbations.

Together, these mechanisms produce perturbations that are semantically aligned and spectrally coherent, reducing overfitting to surrogate-specific patterns. Experiments on ImageNet across diverse architectures—including ViTs, CNNs, hybrid models, and adversarially trained networks—show that TESSER consistently outperforms state-of-the-art transfer-based attacks.

These results demonstrate that **transferability is governed by shared semantic and spectral structure, rather than raw optimization strength**.

---

## Key Contributions

- Identifies **semantic misalignment and spectral artifacts** as key barriers to transferability  
- Proposes **FSGS**, a token-level gradient modulation strategy for semantic alignment  
- Introduces **SSR**, a differentiable regularization for spectral coherence  
- Unifies semantic and spectral control into a single framework  
- Achieves state-of-the-art transferability across **ViTs, CNNs, and hybrid models**  
- Provides analysis linking **structure → transferability → generalization**  

---

## Results

<img src="/images/result_tesser.png" style="max-width:100%; border-radius:8px;"/>

*TESSER consistently outperforms state-of-the-art transfer-based attacks.*

<img src="/images/qualitative_tesser.png" style="max-width:100%; border-radius:8px;"/>

*Produces perturbations that are semantically aligned and spectrally smooth.*

---

## Why This Matters

TESSER reframes adversarial attack design:

> Strong attacks are not those that maximize loss —  
> but those that preserve **shared structure across models**.

This has implications for:
- black-box attack design  
- robustness evaluation  
- cross-architecture generalization  

---

## Broader Perspective

TESSER complements a broader research framework:

- **TESSER** → exploits alignment to improve transferability  
- **DRIFT** → breaks gradient alignment to improve robustness  
- **TriQDef** → breaks structural alignment across quantization  

Together:

> Alignment → Transferability → Vulnerability  
> Disruption → Divergence → Robustness  

---


## Citation
```bibtex
@article{guesmi2025tesser,
  title     = {TESSER: Transfer-Enhancing Adversarial Attacks from Vision Transformers via Spectral and Semantic Regularization},
  author    = {Guesmi, Amira and <Other Authors>},
  journal   = {arXiv},
  volume    = {abs/2505.19613},
  year      = {2025}
}
```
