---
title: "ODDR: Outlier Detection & Dimension Reduction Based Defense Against Adversarial Patch Attacks"
collection: portfolio
permalink: /project_pages/oddr/
excerpt: "A defense framework that detects and suppresses adversarial patch artifacts via feature outlier modeling and dimensionality reduction."
date: 2025-01-01
venue: "ICCV 2025"
paperurl: "https://openaccess.thecvf.com/content/ICCV2025/html/Chattopadhyay_ODDR_Outlier_Detection__Dimension_Reduction_Based_Defense_Against_Adversarial_ICCV_2025_paper.html"
authors: "Nandish Chattopadhyay, Amira Guesmi, Muhammad Abdullah Hanif, Bassem Ouni, Muhammad Shafique"
topic: "Adversarial Machine Learning — Foundations"

header:
  overview: /images/projects/oddr_overview.png
---

## Links
- **Paper:** [ICCV Open Access]({{ page.paperurl }})
{% if page.codeurl and page.codeurl != "" %}- **Code:** [GitHub]({{ page.codeurl }}){% endif %}
{% if page.bibtexurl and page.bibtexurl != "" %}- **BibTeX:** [Download]({{ page.bibtexurl }}){% endif %}

## Overview

<img src="/images/ICCV_ODDR.png" width="100%">

**ODDR** (Outlier Detection & Dimension Reduction) is a defense framework designed to mitigate the impact of adversarial patch attacks by identifying anomalous feature activations and suppressing their influence on downstream predictions.

Unlike transformation-based defenses that rely on stochastic perturbations, ODDR operates directly in feature space, modeling patch-induced activations as statistical outliers.

---

## Abstract

Adversarial patch attacks introduce localized perturbations that produce disproportionate feature activations in deep neural networks. These anomalous responses propagate through the network and dominate classification decisions, leading to consistent misclassification even under physical-world transformations.

We propose **ODDR**, a defense mechanism that detects and mitigates patch-induced artifacts through a two-stage pipeline:

1. **Outlier Detection** — Identifies abnormal feature responses using statistical deviation modeling.
2. **Dimension Reduction** — Projects features into a compact subspace that suppresses adversarial dominance while preserving semantic information.

Extensive experiments across CNN and Vision Transformer architectures demonstrate that ODDR significantly reduces attack success rates while maintaining strong clean accuracy, outperforming existing preprocessing and transformation-based defenses.

---

## Key Contributions

- First defense to jointly leverage **feature outlier modeling** and **dimension reduction** for patch mitigation.
- Architecture-agnostic — effective across CNNs and Vision Transformers.
- Preserves semantic feature structure while suppressing adversarial artifacts.
- Robust against adaptive and transfer-based patch attacks.

---

## Method Pipeline

The ODDR pipeline operates as follows:

1. Extract intermediate feature maps.
2. Identify anomalous activations via statistical scoring.
3. Apply dimensionality reduction to filter adversarial components.
4. Forward refined features to the classifier.

---

## Experimental Results

ODDR achieves:

- Significant reduction in Patch ASR.
- Improved robustness vs preprocessing defenses.
- Strong cross-architecture generalization.


---

## Citation

```bibtex
@inproceedings{guesmi2025oddr,
  title     = {ODDR: Outlier Detection \& Dimension Reduction Based Defense Against Adversarial Patch Attacks},
  author    = {Guesmi, Amira and Ouni, Bassem and Shafique, Muhammad},
  booktitle = {International Conference on Computer Vision (ICCV)},
  year      = {2025}
}
