---
title: "DAP: A Dynamic Adversarial Patch for Evading Person Detectors"
collection: portfolio
permalink: /project_pages/dap/
date: 2024-06-01
venue: "CVPR"
paperurl: "https://openaccess.thecvf.com/content/CVPR2024/html/Guesmi_DAP_A_Dynamic_Adversarial_Patch_for_Evading_Person_Detectors_CVPR_2024_paper.html"
codeurl: ""
bibtexurl: ""
authors: "Amira Guesmi, Ruitian Ding, Muhammad Abdullah Hanif, Ihsen Alouani, Bassem Ouni, Muhammad Shafique"
excerpt: "A dynamic adversarial patch that generates printable, naturalistic patterns robust to pose changes, clothing deformation, and real-world transformations."
topic: "Adversarial Machine Learning — Vision & Autonomous Systems"
image: /images/dap_method.png
---

## Core Insight
Physical adversarial patches fail when they are treated as static objects.  
DAP shows that robust physical attacks must account for **pose changes, fabric deformation, and real-world transformations**.

---

## Links
- **Paper:** [CVPR Open Access]({{ page.paperurl }})
- **Demo:** [Link](https://www.youtube.com/watch?v=KgHayArnTBM)
{% if page.codeurl and page.codeurl != "" %}- **Code:** [GitHub]({{ page.codeurl }}){% endif %}
{% if page.bibtexurl and page.bibtexurl != "" %}- **BibTeX:** [Download]({{ page.bibtexurl }}){% endif %}

---

## Motivation

Adversarial patches can fool object detectors, but many existing attacks degrade under real-world conditions.  
This is especially true for clothing-based attacks, where printed patches are affected by body pose, fabric wrinkles, lighting, scale, and viewpoint changes.

DAP asks:

> Can we generate a printable, naturalistic adversarial patch that remains effective under realistic physical transformations?

<img src="/images/attack_robustness_dap.png" alt="Robust patch optimization pipeline" style="max-width:100%; border-radius:8px;"/>

*DAP explicitly optimizes adversarial patches under transformations that approximate real-world deployment conditions.*

---

## Method Overview

<img src="/images/dap_method.png" alt="DAP Overview" style="max-width:100%; border-radius:8px;"/>

DAP is a GAN-free adversarial patch generation framework.  
Instead of relying on a restricted GAN latent space, DAP directly optimizes patch pixels while preserving a naturalistic visual appearance.

The method introduces:
- a similarity-guided optimization objective
- transformation-aware patch training
- a **Creases Transformation (CT)** block to simulate non-rigid fabric deformation
- robustness to scale, rotation, lighting, noise, and clothing wrinkles

---

## Abstract

Patch-based adversarial attacks expose critical vulnerabilities in computer vision systems, especially person detectors used in surveillance, autonomous systems, and edge-based smart cameras. However, many existing physical attacks remain conspicuous or fragile under real-world transformations.

We propose **DAP**, a Dynamic Adversarial Patch framework for generating printable, naturalistic adversarial patterns that evade person detectors under realistic physical conditions. Unlike GAN-based approaches, which are constrained by limited latent spaces, DAP directly optimizes patch pixels while using a similarity metric to preserve a predefined natural appearance.

To address the physical challenges of clothing-based attacks, DAP introduces a **Creases Transformation (CT)** block that simulates non-rigid deformations caused by pose changes and fabric wrinkles. This enables the generated patch to remain effective under scale changes, rotation, brightness and contrast variation, random noise, and clothing deformation.

DAP achieves an attack success rate of **82.28% in the digital setting** against YOLOv7 on INRIA and **65% in the physical setting** against YOLOv3-tiny deployed on edge-based smart cameras.

---

## Key Contributions

- Proposes **DAP**, a GAN-free framework for generating naturalistic printable adversarial patches.
- Shows that directly optimizing patch pixels provides greater flexibility than GAN latent-space optimization.
- Introduces the **Creases Transformation (CT)** block to model non-rigid T-shirt deformation caused by pose and fabric wrinkles.
- Optimizes patch robustness under realistic transformations, including scale, rotation, lighting, noise, and clothing deformation.
- Demonstrates strong attack performance in both digital and physical settings.
- Reveals practical vulnerabilities in person detection systems deployed on edge-based smart cameras.

---

## Results

<img src="/images/dig_perf_dap.png" alt="Digital World Performance" style="max-width:100%; border-radius:8px;"/>

*DAP achieves strong digital-world attack performance, reaching 82.28% attack success against YOLOv7.*

<img src="/images/phys_perf_dap.png" alt="Physical World Performance" style="max-width:100%; border-radius:8px;"/>

*DAP remains effective in the physical world, achieving 65% attack success against YOLOv3-tiny on edge-based smart cameras.*

---

## Why This Matters

DAP shows that adversarial robustness cannot be evaluated only under static digital assumptions.

In real deployments, attacks and defenses must account for:
- moving people
- deformable clothing
- changing camera viewpoints
- lighting variation
- edge-device constraints

This work demonstrates that physically realizable adversarial patches can remain effective when designed with deployment conditions in mind.

---

## Broader Perspective

DAP is part of a broader research direction on **deployment-aware adversarial robustness**.

It shows that transferability and physical robustness depend on preserving adversarial structure under transformation.  
This connects to my broader work on understanding how structural consistency, physical variability, and representation alignment shape the security of real-world AI systems.

---

## Citation

```bibtex
@inproceedings{guesmi2024dap,
  title     = {DAP: A Dynamic Adversarial Patch for Evading Person Detectors},
  author    = {Guesmi, Amira and Ding, Ruitian and Hanif, Muhammad Abdullah and Alouani, Ihsen and Shafique, Muhammad},
  booktitle = {Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition (CVPR)},
  year      = {2024}
}
```
