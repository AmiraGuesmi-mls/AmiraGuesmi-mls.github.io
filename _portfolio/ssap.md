---
title: "SSAP: A Shape-Sensitive Adversarial Patch for Monocular Depth Estimation"
collection: portfolio
permalink: /project_pages/ssap/
excerpt: "A shape-aware adversarial patch that reveals fundamental vulnerabilities in geometric perception systems."
date: 2024-01-01
venue: "IROS"
paperurl: "https://ieeexplore.ieee.org/document/10802252"
authors: "Amira Guesmi, Muhammad Abdullah Hanif, Ihsen Alouani, Bassem Ouni, Muhammad Shafique"
topic: "Adversarial Machine Learning — Vision & Autonomous Systems"
image: /images/ssap_method.png
image1: /images/clas_vs_mon_ssap.png
image2: /images/motivation_ssap.png
image3: /images/quant_ssap.png
image4: /images/qual_ssap.png
---

## Core Insight
Monocular depth estimation models rely on **global geometric and shape priors**, not just local pixel evidence.  
SSAP exploits this property to propagate adversarial influence across the entire object, enabling **global geometric distortion from a localized perturbation**.

---

## Links
- **Paper:** [IROS]({{ page.paperurl }})
{% if page.codeurl and page.codeurl != "" %}- **Code:** [GitHub]({{ page.codeurl }}){% endif %}
{% if page.bibtexurl and page.bibtexurl != "" %}- **BibTeX:** [Download]({{ page.bibtexurl }}){% endif %}

---

## Motivation

Modern adversarial attacks primarily target classification and detection systems through **pixel-local perturbations**.  
However, monocular depth estimation (MDE) fundamentally differs: it relies on **global consistency and geometric reasoning**.

This raises a critical question:

> Can a localized perturbation disrupt the *entire perceived geometry* of an object?

<img src="/images/clas_vs_mon_ssap.png" alt="Attacks on Classification/Detection vs. MDE" style="max-width:100%; border-radius:8px;">

*Traditional attacks remain localized, whereas depth estimation depends on global structure.*

<img src="/images/motivation_ssap.png" alt="Limitation of SOTA" style="max-width:100%; border-radius: 8px;"/>

*Existing methods fail to exploit shape priors, limiting their impact on geometric perception.*

---

## Method Overview

<img src="/images/ssap_method.png" alt="SSAP Overview" style="max-width:100%; border-radius: 8px;"/>

SSAP introduces a **shape-aware adversarial optimization framework** that leverages object-level priors.

Instead of affecting only the patch region, SSAP:
- exploits **structural dependencies in depth estimation**
- propagates perturbation influence across the **entire object surface**
- induces **global depth distortion and structural misinterpretation**

---

## Abstract

Monocular Depth Estimation (MDE) is critical for autonomous systems, enabling scene understanding and safe navigation. Despite advances in deep learning–based depth models, their robustness to adversarial manipulation remains largely unexplored.

We propose **SSAP**, a Shape-Sensitive Adversarial Patch that targets the geometric reasoning process of depth estimation models. Unlike conventional adversarial patches that affect only overlapping pixels, SSAP exploits **shape priors** to propagate distortion across the full spatial extent of the target object.

By optimizing a penalized depth loss under realistic transformations (scale, rotation, viewpoint, illumination), SSAP induces severe depth misestimation and even object disappearance. Across CNN- and Transformer-based architectures, SSAP achieves depth errors exceeding 0.5 while affecting up to 99% of the object region.

These results reveal a critical vulnerability: **geometric perception in deep models can be globally manipulated through localized perturbations**.

---

## Key Contributions

- **First shape-sensitive adversarial patch for monocular depth estimation**, moving beyond classification/detection-focused attacks  
- Demonstrates **global geometric distortion from a local perturbation** via shape-aware optimization  
- Introduces a **penalized depth loss formulation** tailored to maximize structural misestimation  
- Ensures **physical robustness** under scale, rotation, viewpoint, and illumination variations  
- Validates effectiveness across **CNN and Transformer-based depth models**  
- Reveals **severe safety risks**, including object disappearance and large distance misestimation  

---

## Results

<img src="/images/quant_ssap.png" alt="Quantitative Results" style="max-width:100%; border-radius: 8px;"/>

<img src="/images/qual_ssap.png" alt="Qualitative Results" style="max-width:100%; border-radius: 8px;"/>

SSAP induces large-scale depth errors, exceeding 0.5 and affecting up to **99% of the object region**.

Crucially, the attack is not localized:
- it **alters the global geometry of the scene**
- causes **object disappearance**
- leads to **severe distance misestimation**

These effects highlight a fundamental weakness in depth perception models:  
they rely on structural priors that can be **systematically exploited**.

---

## Why This Matters

Unlike classification errors, failures in depth estimation directly impact:

- **Distance perception**
- **Collision avoidance**
- **Navigation safety**

SSAP demonstrates that:
> Deep models do not merely misclassify — they can **misinterpret the geometry of the world**.

This poses serious risks for:
- autonomous driving systems  
- robotics and embodied AI  
- real-world perception pipelines  

---

## Broader Perspective

This work is part of a broader research direction on:

> **Understanding how structural priors and representation alignment influence robustness in AI systems**

SSAP shows that:
- exploiting structure → enables powerful attacks  
- controlling structure → is key to building robust systems  

---

## Citation
```bibtex
@inproceedings{guesmi2024ssap,
  title     = {SSAP: A Shape-Sensitive Adversarial Patch for Comprehensive Disruption of Monocular Depth Estimation},
  author    = {Guesmi, Amira and Hanif, Muhammad Abdullah and Alouani, Ihsen and Ouni, Bassem and Shafique, Muhammad},
  booktitle = {IEEE/RSJ International Conference on Intelligent Robots and Systems (IROS)},
  year      = {2024}
}
