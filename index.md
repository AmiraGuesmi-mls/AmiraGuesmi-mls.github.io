---
layout: single
title: ""
permalink: /
author_profile: true
---

I lead research on AI security and trustworthy machine learning, with a focus on adversarial attacks and defenses, robustness under deployment constraints, and secure perception systems. My work bridges theory, system-level design, and real-world evaluation, targeting vision, autonomous, embedded, and multimodal AI systems.

---

## 🔥 News

- **2026.01**: 🎉 2 papers accepted at **ICLR 2026**
- **2025.11**: 🎉 1 paper accepted at **DATE 2026**
- **2025.10**: 🎉 Selected as Top Reviewer at **NeurIPS 2025** 
- **2025.06**: 🎉 1 paper accepted at **ICCV 2025**
- **2024.06**: 🎉 1 paper accepted at **IROS 2024**
- **2024.06**: 🎉 3 papers accepted at **ICIP 2024**
- **2024.02**: 🎉 1 paper accepted at **CVPR 2024**
- **2024.02**: 🎉 1 paper accepted at **DAC 2024** 


---

## Research Overview

My research aims to advance the security, robustness, and trustworthiness of machine learning systems under adversarial threats and realistic deployment constraints. I study how architecture choices (e.g., Vision Transformers), quantization and approximation, physical-world effects, and multimodal interactions shape both vulnerabilities and defenses. A recurring theme in my work is breaking brittle alignment—semantic, gradient, or representational—to improve robustness while preserving efficiency and deployability.

---

## Selected Research Projects

Below are representative research projects spanning adversarial machine learning, robustness, and secure AI systems.  

---

<!-- DRIFT -->
<div style="display:flex; gap:32px; margin-bottom:60px; align-items:flex-start;">

  <div style="min-width:400px; max-width:400px;">
    <img src="/images/drift.png" style="width:100%; border-radius:10px;">
  </div>

  <div>

    <div style="font-size:0.9rem; font-weight:400; margin-bottom:8px; line-height:1.15;">
      ICLR 2026: 
      <a href="/project_pages/drift/">DRIFT: Divergent Response in Filtered Transformations</a>
    </div>

    <div style="font-size:0.7rem; line-height:1.6; margin-bottom:12px; text-align:justify;">
      DRIFT is a stochastic ensemble defense that disrupts gradient consensus across transformations, significantly reducing adversarial transferability while preserving clean accuracy.
    </div>

    <div>
      <a href="/project_pages/drift/">Project</a> |
      <a href="#">Paper</a>
    </div>

  </div>
</div>

---

<!-- TriQDef -->

<div style="display:flex; gap:32px; margin-bottom:60px; align-items:flex-start;">

  <div style="min-width:400px; max-width:400px;">
    <img src="/images/triqdef.png" style="width:100%; border-radius:10px;">
  </div>

  <div>

    <div style="font-size:0.9rem; font-weight:400; margin-bottom:8px; line-height:1.15;">
      ICLR 2026: 
      <a href="/project_pages/triqdef/">TriQDef: Disrupting Semantic and Gradient Alignment to Prevent Adversarial Patch Transferability in Quantized Neural Networks</a>
    </div>

    <div style="font-size:0.7rem; line-height:1.6; margin-bottom:12px; text-align:justify;">
      Disrupts semantic and gradient alignment across quantized models to prevent patch transferability.
    </div>

    <div>
      <a href="/project_pages/triqdef/">Project</a> |
      <a href="#">Paper</a>
    </div>

  </div>
</div>
---
<!-- TESSER -->
<div style="display:flex; gap:32px; margin-bottom:60px; align-items:flex-start;">

  <div style="min-width:400px; max-width:400px;">
    <img src="/images/tesser_overview.png" style="width:100%; border-radius:10px; margin-bottom:8px;">
  </div>

  <div>

    <div style="font-size:0.9rem; font-weight:400; margin-bottom:8px; line-height:1.15;">
      ArXiv 2025: 
      <a href="/project_pages/tesser/">TESSER: Transfer-Enhancing Adversarial Attacks from Vision Transformers</a>
    </div>

    <div style="font-size:0.7rem; line-height:1.6; margin-bottom:12px; text-align:justify;">
      TESSER introduces spectral and semantic regularization to enhance adversarial transferability from Vision Transformers to CNNs and hybrid architectures, achieving state-of-the-art black-box attack performance across diverse model families.
    </div>

    <div>
      <a href="/project_pages/tesser/">Project</a> |
      <a href="https://arxiv.org/abs/2505.19613">Paper</a>
    </div>

  </div>
</div>

---

<!-- ODDR -->
<div style="display:flex; gap:32px; margin-bottom:60px; align-items:flex-start;">

  <div style="min-width:400px; max-width:400px;">
    <img src="/images/oddr_overview.png" style="width:100%; border-radius:10px; margin-bottom:8px;">
  </div>

  <div>

    <div style="font-size:0.9rem; font-weight:400; margin-bottom:8px; line-height:1.15;">
      ICCV 2025: 
      <a href="/project_pages/tesser/">ODDR: Outlier Detection & Dimension Reduction Based Defense Against Adversarial Patches</a>
    </div>

    <div style="font-size:0.7rem; line-height:1.6; margin-bottom:12px; text-align:justify;">
      Outlier Detection and Dimension Reduction (ODDR) is a comprehensive defense strategy engineered to counteract patch-based adversarial attacks through advanced statistical methodologies.
    </div>

    <div>
      <a href="/project_pages/oddr/">Project</a> |
      <a href="[https://arxiv.org/abs/2505.19613](https://openaccess.thecvf.com/content/ICCV2025/html/Chattopadhyay_ODDR_Outlier_Detection__Dimension_Reduction_Based_Defense_Against_Adversarial_ICCV_2025_paper.html)">Paper</a>
    </div>

  </div>
</div>

---

<!-- DAP -->
<div style="display:flex; gap:32px; margin-bottom:60px; align-items:flex-start;">

  <div style="min-width:400px; max-width:400px;">
    <img src="/images/DAP_teaser.png" style="width:100%; border-radius:10px;">
  </div>

  <div>

    <div style="font-size:0.9rem; font-weight:400; margin-bottom:8px; line-height:1.15;">
      CVPR 2024: 
      <a href="/project_pages/dap/">DAP: Dynamic Adversarial Patch</a>
    </div>

    <div style="font-size:0.7rem; line-height:1.6; margin-bottom:12px; text-align:justify;">
      Patch-based adversarial attacks were proven to compromise the robustness and reliability of computer vision systems. However their conspicuous and easily detectable nature challenge their practicality in real-world setting. To address this recent work has proposed using Generative Adversarial Networks (GANs) to generate naturalistic patches that may not attract human attention. However such approaches suffer from a limited latent space making it challenging to produce a patch that is efficient stealthy and robust to multiple real-world transformations. This paper introduces a novel approach that produces a Dynamic Adversarial Patch (DAP) designed to overcome these limitations. DAP maintains a naturalistic appearance while optimizing attack efficiency and robustness to real-world transformations. The approach involves redefining the optimization problem and introducing a novel objective function that incorporates a similarity metric to guide the patch's creation. Unlike GAN-based techniques the DAP directly modifies pixel values within the patch providing increased flexibility and adaptability to multiple transformations. Furthermore most clothing-based physical attacks assume static objects and ignore the possible transformations caused by non-rigid deformation due to changes in a person's pose. To address this limitation aCreases Transformation'(CT) block is introduced enhancing the patch's resilience to a variety of real-world distortions.
    </div>

    <div>
      <a href="/project_pages/dap/">Project</a> |
      <a href="#">Paper</a>
    </div>

  </div>
</div>


---

## 🏆 Awards & Honors

- **Outstanding Reviewer**, NeurIPS 2025.
- **Best Senior Researcher Award**, eBRAIN Lab, NYUAD, 2023.
- **Erasmus+ Scholarship**, France, 2019.
- **DAAD Scholarship**: Advanced Technologies based on IoT (ATIoT), Germany, 2018.
- **DAAD Scholarship**: Young ESEM Program (Embedded Systems for Energy Management), Germany, 2016.

---

## 🧑‍🏫 Academic Service & Community

- Reviewer: ICLR, NeurIPS, ICCV, CVPR, AAAI, ECCV, DAC, DATE, ICIP; IEEE TIFS, TCSVT, TCAD,  
- Organizer & Speaker: Tutorial: *ML Security in Autonomous Systems*, IROS 2024  

---

## 📬 Contact & Links

- **Email**: ag9321@nyu.edu  

I am always open to collaborations on **AI security, adversarial robustness, and trustworthy ML systems**.
