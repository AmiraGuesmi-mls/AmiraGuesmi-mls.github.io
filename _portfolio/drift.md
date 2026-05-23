---
title: "DRIFT: Divergent Response in Filtered Transformations for Robust Adversarial Defense"
collection: portfolio
permalink: /project_pages/drift/
date: 2026-01-15
venue: "ICLR"
paperurl: "[https://openreview.net/forum?id=REPLACE_WITH_DRIFT_ID](https://openreview.net/forum?id=AYH7uBK1Gg&referrer=%5Bthe%20profile%20of%20Amira%20Guesmi%5D(%2Fprofile%3Fid%3D~Amira_Guesmi1))"
codeurl: ""
bibtexurl: ""
authors: "Amira Guesmi, Muhammad Shafique"
excerpt: "A stochastic differentiable defense framework that breaks gradient consensus via divergent responses across filtered transformations."
topic: "Adversarial Machine Learning — Foundations"

image: /images/drift_method.png

---

## Core Insight

Most defenses fail not because gradients are unavailable, but because they are **too consistent**.

DRIFT identifies **gradient consensus across transformations** as the key driver of adversarial transferability, and shows that robustness requires enforcing **divergence—not randomness**.

---

## Links
- **Paper:** [OpenReview](https://openreview.net/forum?id=AYH7uBK1Gg)

---

## Motivation

Transformation-based defenses attempt to improve robustness by introducing randomness (e.g., resizing, noise, filtering).

However, attackers can still succeed using EOT or BPDA.

Why?

<img src="/images/fail_drift.png" style="max-width:100%; border-radius:8px;"/>

Because:
- transformations change inputs  
- but **preserve gradient structure**

> The gradients remain aligned → attacks remain transferable.

---

## Why Do Transformation Defenses Fail?

<img src="/images/consensus_drift.png" style="max-width:100%; border-radius:8px;"/>

Across different transformations:
- gradients exhibit **high alignment**
- attackers exploit this to construct robust perturbations

This reveals a key principle:

> Robustness is not about randomness — it is about **breaking gradient consensus**.

---

## Method Overview

<img src="/images/idea_drift.png" style="max-width:100%; border-radius:8px;"/>

<img src="/images/drift_method.png" style="max-width:100%; border-radius:8px;"/>

DRIFT is a **stochastic, differentiable filter ensemble** that enforces gradient divergence.

Instead of relying on non-differentiability or masking, DRIFT:

- applies **learnable filtered transformations**
- enforces **divergent responses across filters**
- preserves prediction consistency on clean data

The training objective combines:
- prediction consistency  
- Jacobian divergence  
- logit-space divergence  
- adversarial robustness  

This leads to **structured gradient disalignment**, not noise.

---

## Abstract

Deep neural networks remain highly vulnerable to adversarial examples, particularly when gradients can be reliably estimated. We identify **gradient consensus**—the tendency of randomized transformations to produce aligned gradients—as a key mechanism enabling adversarial transferability.

We propose **DRIFT (Divergent Response in Filtered Transformations)**, a stochastic, differentiable defense framework that enforces gradient divergence across transformation pathways. Unlike prior randomized defenses that rely on gradient masking, DRIFT introduces a learnable filter ensemble trained to maximize divergence in Jacobian and logit responses while preserving clean predictions.

We formalize gradient consensus and theoretically link it to transferability, and propose a consensus-divergence training strategy that combines prediction consistency, Jacobian separation, logit-space separation, and adversarial training. Experiments on ImageNet-scale models, including CNNs and Vision Transformers, show that DRIFT achieves strong robustness against adaptive white-box attacks (BPDA, EOT), transfer-based attacks, and gradient-free attacks, outperforming state-of-the-art transformation-based and stochastic defenses.

These results demonstrate that **enforcing gradient divergence—not randomness—is key to robust adversarial defense**.

---

## Key Contributions

- Introduces **gradient consensus** as a fundamental mechanism underlying adversarial transferability  
- Provides theoretical analysis linking **gradient alignment → transferability**  
- Proposes **DRIFT**, a differentiable filter-ensemble defense enforcing gradient divergence  
- Demonstrates strong robustness against **adaptive white-box attacks (BPDA, EOT)**  
- Achieves state-of-the-art performance across **CNNs and Vision Transformers on ImageNet**  
- Maintains **low computational overhead**, enabling practical deployment  

---

## Results

<img src="/images/stand_drift.png" style="max-width:100%; border-radius:8px;"/>

*DRIFT outperforms existing defenses under standard white-box attacks.*

<img src="/images/adapt_drift.png" style="max-width:100%; border-radius:8px;"/>

*Maintains robustness under strong adaptive attacks (BPDA + EOT).*

<img src="/images/trans_drift.png" style="max-width:100%; border-radius:8px;"/>

*Reduced gradient consensus leads to lower transferability.*

<img src="/images/lightweight_drift.png" style="max-width:100%; border-radius:8px;"/>

*Lightweight and deployable with minimal overhead.*

---

## Why This Matters

DRIFT shifts the perspective on adversarial defense:

> The problem is not that gradients exist — it is that they are **shared**.

By breaking this shared structure:
- transferability is reduced  
- adaptive attacks become harder  
- robustness generalizes across architectures  

This has implications for:
- transformation-based defenses  
- stochastic defenses  
- real-world deployable AI systems  

---

## Broader Perspective

DRIFT is a core component of a broader research direction:

> **Alignment → Transferability → Vulnerability**  
> **Disruption → Divergence → Robustness**

It complements:
- **TriQDef** → breaks cross-bit structural alignment  
- **TESSER** → exploits alignment for transfer attacks  
- **SSAP / DAP** → exploit structure in physical attacks  

---


## Citation
```bibtex
@inproceedings{guesmi2026drift,
  title={DRIFT: Divergent Response in Filtered Transformations for Robust Adversarial Defense},
  author={Guesmi, Amira and Shafique, Muhammad},
  booktitle={International Conference on Learning Representations (ICLR)},
  year={2026}
}
```
