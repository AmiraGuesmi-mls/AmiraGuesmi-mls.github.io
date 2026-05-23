---
title: "TriQDef: Disrupting Semantic and Gradient Alignment to Prevent Adversarial Patch Transferability in Quantized Neural Networks"
collection: portfolio
permalink: /project_pages/triqdef/
date: 2026-01-15
venue: "ICLR"
paperurl: "https://openreview.net/forum?id=acQP99PU8y"
authors: "Amira Guesmi, Bassem Ouni, Muhammad Shafique"
excerpt: "A defense framework that disrupts cross-bit structural alignment to prevent patch transferability in quantized neural networks."
topic: "Robustness and Security of Quantized & Approximate Neural Networks"
image: /images/triqdef_method.png
---

## Core Insight
Quantization changes numerical precision, but **does not break the underlying structure of learned representations**.  
Adversarial patches exploit this hidden consistency, remaining transferable across bit-widths.

TriQDef shows that robustness requires **disrupting structural alignment in both features and gradients**.

---

## Links
- **Paper:** [OpenReview](https://openreview.net/forum?id=acQP99PU8y)

---

## Motivation

Quantized Neural Networks (QNNs) are widely deployed in edge and embedded systems due to their efficiency.  
It is often assumed that quantization improves robustness by distorting gradients.

However, we observe:

> Patch-based adversarial attacks remain highly effective across bit-widths — even at 2-bit precision.

<img src="/images/motivation_triqdef.png" alt="Quantization does not stop patch attacks" style="max-width:100%; border-radius:8px;"/>

This reveals a critical gap:
- quantization disrupts *local gradients*
- but preserves *global structure*

---

## Why Does Transferability Persist?

<img src="/images/insight_triqdef.png" alt="Why transferability persists?" style="max-width:100%; border-radius:8px;"/>

Despite low cosine similarity, gradients across bit-widths exhibit **high structural alignment**:
- similar edges
- similar orientation distributions
- similar spatial patterns

This explains why patch attacks transfer:
> they rely on **perceptual structure**, not precise gradient values.

---

## Method Overview

<img src="/images/triqdef_method.png" alt="TriQDef Overview" style="max-width:100%; border-radius:8px;"/>

TriQDef is a **tri-level defense framework** designed to break alignment across quantization levels:

1. **Feature Disalignment Penalty (FDP)**  
   → disrupts semantic consistency across bit-widths  

2. **Gradient Perceptual Dissonance Penalty (GPDP)**  
   → misaligns gradient structure using Edge IoU and HOG similarity  

3. **Bit-Width-Aware Curriculum Training (BACT)**  
   → progressively enforces robustness across quantization levels through curriculum-based training  

Together, these components break the shared structure that enables patch transferability.

---

## Abstract

Quantized Neural Networks (QNNs) are widely deployed in resource-constrained environments due to their efficiency. While quantization distorts gradient landscapes and weakens pixel-level attacks, it provides limited robustness against patch-based adversarial attacks, which remain highly transferable across bit-widths.

We propose **TriQDef**, a quantization-aware defense framework that disrupts cross-bit transferability by targeting both feature and gradient alignment. The framework integrates a Feature Disalignment Penalty (FDP) to enforce semantic inconsistency, a Gradient Perceptual Dissonance Penalty (GPDP) to misalign gradient structure using perceptual metrics, and a Bit-Width-Aware Curriculum Training (BACT) strategy to progressively enforce robustness across quantization levels.

Experiments on CIFAR-10 and ImageNet show that TriQDef reduces attack success rates by over 40% on unseen patch and quantization configurations while maintaining high clean accuracy. These results demonstrate that **structural alignment—not numerical precision—is the key enabler of patch transferability in QNNs**.

---

## Key Contributions

- First systematic study of **patch transferability across quantized neural networks**
- Reveals that **structural alignment persists despite gradient distortion**
- Proposes **TriQDef**, a defense targeting both feature and gradient alignment
- Introduces **perceptual alignment metrics** (Edge IoU, HOG Cosine) to quantify structural similarity
- Achieves **>40% reduction in attack success rate** on unseen patches and quantization settings
- Preserves **high clean accuracy with minimal deployment overhead**

---

## Results

<img src="/images/patch_transferability_triqdef.png" alt="TriQDef reduces transferability" style="max-width:100%; border-radius:8px;"/>

*TriQDef significantly reduces patch transferability across bit-widths.*

<img src="/images/acc_dep_cost_triqdef.png" alt="Accuracy vs cost" style="max-width:100%; border-radius:8px;"/>

*Maintains strong accuracy without increasing deployment cost.*

<img src="/images/sota_vs_triqdef.png" alt="Comparison with SOTA" style="max-width:100%; border-radius:8px;"/>

*Outperforms existing defenses by explicitly targeting structural alignment.*

---

## Why This Matters

TriQDef challenges a common assumption:

> Robustness cannot be achieved by perturbing numerical precision alone.

Instead, it shows:
- vulnerabilities arise from **shared structure**
- transferability is driven by **alignment**
- robustness requires **controlled divergence**

This has implications for:
- edge AI deployment
- quantized and approximate computing
- secure machine learning under hardware constraints

---

## Broader Perspective

TriQDef is part of a broader research direction on:

> **Alignment as the root cause of adversarial transferability**

Across models, architectures, and bit-widths:
- alignment → transferability → vulnerability  
- disruption → divergence → robustness  

This principle underlies my work on:
- quantized neural networks  
- adversarial patches  
- Vision Transformers and cross-architecture attacks  
- multimodal consistency and hallucination  

---

## Citation
```bibtex
@inproceedings{guesmi2026triqdef,
  title={TriQDef: Disrupting Semantic and Gradient Alignment to Prevent Adversarial Patch Transferability in Quantized Neural Networks},
  author={Guesmi, Amira and Ouni, Bassem and Shafique, Muhammad},
  booktitle={International Conference on Learning Representations (ICLR)},
  year={2026}
}
```
