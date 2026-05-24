---
title: "ODDR: Outlier Detection & Dimension Reduction Based Defense Against Adversarial Patch Attacks"
collection: portfolio
permalink: /project_pages/oddr/
excerpt: "We show that adversarial patches dominate predictions by creating outlier feature activations. ODDR detects and suppresses these anomalies through feature-space outlier modeling and dimension reduction, restoring robust predictions."
date: 2025-01-01
venue: "ICCV 2025"
paperurl: "https://openaccess.thecvf.com/content/ICCV2025/html/Chattopadhyay_ODDR_Outlier_Detection__Dimension_Reduction_Based_Defense_Against_Adversarial_ICCV_2025_paper.html"
authors: "Nandish Chattopadhyay, Amira Guesmi, Muhammad Abdullah Hanif, Bassem Ouni, Muhammad Shafique"
topic: "Adversarial Machine Learning — Vision & Autonomous Systems"
---

## Links
- **Paper:** [ICCV Open Access]({{ page.paperurl }})
{% if page.codeurl and page.codeurl != "" %}- **Code:** [GitHub]({{ page.codeurl }}){% endif %}
{% if page.bibtexurl and page.bibtexurl != "" %}- **BibTeX:** [Download]({{ page.bibtexurl }}){% endif %}

---

## Key Idea
> **Adversarial patches succeed because they create dominant outlier activations in feature space.**

---

## Motivation: Why Do Patch Attacks Remain Effective?

Adversarial patches introduce localized perturbations that produce **disproportionately strong feature activations**.  
These activations propagate through the network and dominate predictions, making patch attacks highly robust—even under real-world transformations.

<img src="/images/motivation_oddr.png" alt="Adversarial patches create dominant feature activations that override model predictions" width="100%">

---

## Insight: Patches Are Feature-Space Outliers

Patch-induced activations are not just strong—they are **statistically inconsistent** with normal feature distributions.  
This makes them detectable as **outliers in representation space**.

By identifying and suppressing these anomalies, we can neutralize the effect of the patch without degrading the underlying semantic content.

<img src="/images/insight_oddr.png" alt="Adversarial patch features behave as statistical outliers in representation space" width="100%">

---

## Method: ODDR (Outlier Detection & Dimension Reduction)

We propose **ODDR**, a defense framework that operates directly in feature space to suppress adversarial dominance.

The method consists of two key components:

- **Outlier Detection:** Identify abnormal feature activations using statistical deviation modeling  
- **Dimension Reduction:** Project features into a compact subspace that suppresses adversarial influence while preserving semantic information  

This combination enables **targeted suppression of adversarial artifacts** without relying on input transformations.

<img src="/images/pipline_oddr.png" alt="ODDR pipeline: detect anomalous features and suppress them via dimension reduction" width="100%">

---

## Positioning

Unlike preprocessing or transformation-based defenses that attempt to remove perturbations in input space, ODDR operates in **feature space**, directly targeting the internal mechanisms exploited by patch attacks.

By modeling adversarial patches as **distributional anomalies**, ODDR provides a principled and architecture-agnostic defense strategy.

---

## Abstract

Adversarial patch attacks introduce localized perturbations that produce disproportionate feature activations in deep neural networks.  
These anomalous responses propagate through the network and dominate classification decisions, leading to consistent misclassification even under physical-world transformations.

We propose **ODDR**, a defense mechanism that detects and mitigates patch-induced artifacts through a two-stage pipeline:

1. **Outlier Detection** — Identifies abnormal feature responses using statistical deviation modeling  
2. **Dimension Reduction** — Projects features into a compact subspace that suppresses adversarial dominance while preserving semantic information  

By operating directly in feature space, ODDR effectively suppresses patch-induced activations while maintaining the integrity of benign representations.

Extensive experiments across CNN and Vision Transformer architectures demonstrate that ODDR significantly reduces attack success rates while maintaining strong clean accuracy, outperforming existing preprocessing and transformation-based defenses.

---

## Key Contributions

- We show that adversarial patches act as **dominant feature-space outliers**.  
- We introduce **ODDR**, a defense combining outlier detection and dimension reduction.  
- We design a feature-space pipeline that suppresses adversarial activations while preserving semantic structure.  
- We demonstrate strong robustness across CNNs and Vision Transformers under patch attacks.  

---

## Method Pipeline

The ODDR pipeline operates as follows:

1. Extract intermediate feature representations  
2. Identify anomalous activations via statistical scoring  
3. Suppress adversarial components through dimension reduction  
4. Forward refined features to the classifier  

---

## Results: Suppressing Patch Dominance

ODDR significantly reduces the influence of adversarial patches while preserving model accuracy and generalization.

- Strong reduction in Patch ASR  
- Improved robustness compared to preprocessing defenses  
- Consistent performance across architectures and tasks  

<img src="/images/effectiveness_oddr.png" alt="ODDR improves robustness across classification, detection, and depth estimation tasks" width="100%">

<img src="/images/qualitative_oddr.png" alt="ODDR neutralizes adversarial patches and restores correct predictions" width="100%">

<img src="/images/sota_vs_oddr.png" alt="ODDR outperforms state-of-the-art defenses against patch attacks" width="100%">

---

## Citation

```bibtex
@inproceedings{chattopadhyay2025oddr,
  title={Oddr: Outlier detection \& dimension reduction based defense against adversarial patches},
  author={Chattopadhyay, Nandish and Guesmi, Amira and Hanif, Muhammad Abdullah and Ouni, Bassem and Shafique, Muhammad},
  booktitle={Proceedings of the IEEE/CVF International Conference on Computer Vision},
  pages={22999--23008},
  year={2025}
}
```
