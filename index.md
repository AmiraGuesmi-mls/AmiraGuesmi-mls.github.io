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

<div style="display:flex; flex-direction:column; gap:18px; margin-bottom:60px;">

  <!-- Image on top -->
  <div style="max-width:600px;">
    <img src="/images/drift.png"
         style="width:100%; border-radius:10px;">
  </div>

  <!-- Text underneath -->
  <div style="max-width:900px;">

    <div style="font-size:0.9rem; font-weight:400; margin-bottom:8px;">
      ICLR 2026:
      <a href="/project_pages/drift/">
        DRIFT: Divergent Response in Filtered Transformations for Robust Adversarial Defense
      </a>
    </div>

    <div style="font-size:0.7rem; line-height:1.6; margin-bottom:12px; text-align:justify;">
      We introduce DRIFT (Divergent Response in Filtered Transformations), a stochastic ensemble of lightweight, learnable filters trained to actively disrupt gradient consensus. Unlike prior randomized defenses that rely on gradient masking, DRIFT enforces gradient dissonance by maximizing divergence in Jacobian- and logit-space responses while preserving natural predictions. Our contributions are threefold: (i) we formalize gradient consensus and provide a theoretical analysis linking consensus to transferability; (ii) we propose a consensus-divergence training strategy combining prediction consistency, Jacobian separation, logit-space separation, and adversarial robustness; and (iii) we show that DRIFT achieves substantial robustness gains on ImageNet across CNNs and Vision Transformers, outperforming state-of-the-art preprocessing, adversarial training, and diffusion-based defenses under adaptive white-box, transfer-based, and gradient-free attacks. DRIFT delivers these improvements with negligible runtime and memory cost, establishing gradient divergence as a practical and generalizable principle for adversarial defense.
    </div>

  </div>

</div>

---

<!-- TriQDef -->

<div style="display:flex; flex-direction:column; gap:18px; margin-bottom:60px;">

  <!-- Image on top -->
  <div style="max-width:600px;">
    <img src="/images/triqdef.png" style="width:100%; border-radius:10px;">
  </div>

  <!-- Text underneath -->
  <div style="max-width:900px;">

    <div style="font-size:0.9rem; font-weight:400; margin-bottom:8px">
      ICLR 2026: 
      <a href="/project_pages/triqdef/">TriQDef: Disrupting Semantic and Gradient Alignment to Prevent Adversarial Patch Transferability in Quantized Neural Networks</a>
    </div>

    <div style="font-size:0.7rem; line-height:1.6; margin-bottom:12px; text-align:justify;">
      We introduce TriQDef, a tri-level quantization-aware defense framework designed to disrupt the transferability of patch-based adversarial attacks across QNNs. TriQDef consists of: (1) a Feature Disalignment Penalty (FDP) that enforces semantic inconsistency by penalizing perceptual similarity in intermediate representations; (2) a Gradient Perceptual Dissonance Penalty (GPDP) that explicitly misaligns input gradients across bit-widths by minimizing structural and directional agreement via Edge IoU and HOG Cosine metrics; and (3) a Joint Quantization-Aware Training Protocol that unifies these penalties within a shared-weight training scheme across multiple quantization levels.
    </div>

    <div>
      <a href="/project_pages/triqdef/">Project</a> |
      <a href="#">Paper</a>
    </div>

  </div>
</div>
---
<!-- TESSER -->
<div style="display:flex; flex-direction:column; gap:18px; margin-bottom:60px;">

  <!-- Image on top -->
  <div style="max-width:600px;">
    <img src="/images/tesser_overview.png" style="width:100%; border-radius:10px; margin-bottom:8px;">
  </div>

  <!-- Text underneath -->
  <div style="max-width:900px;">

    <div style="font-size:0.9rem; font-weight:400; margin-bottom:8px; line-height:1.15;">
      ArXiv 2025: 
      <a href="/project_pages/tesser/">TESSER: Transfer-Enhancing Adversarial Attacks from Vision Transformers</a>
    </div>

    <div style="font-size:0.7rem; line-height:1.6; margin-bottom:12px; text-align:justify;">
      Adversarial transferability remains a critical challenge in evaluating the robustness of deep neural networks. In security-critical applications, transferability enables black-box attacks without access to model internals, making it a key concern for real-world adversarial threat assessment. While Vision Transformers (ViTs) have demonstrated strong adversarial performance, existing attacks often fail to transfer effectively across architectures, especially from ViTs to Convolutional Neural Networks (CNNs) or hybrid models. In this paper, we introduce TESSER -- a novel adversarial attack framework that enhances transferability via two key strategies: (1) Feature-Sensitive Gradient Scaling (FSGS), which modulates gradients based on token-wise importance derived from intermediate feature activations, and (2) Spectral Smoothness Regularization (SSR), which suppresses high-frequency noise in perturbations using a differentiable Gaussian prior. These components work in tandem to generate perturbations that are both semantically meaningful and spectrally smooth.
    </div>

    <div>
      <a href="/project_pages/tesser/">Project</a> |
      <a href="https://arxiv.org/abs/2505.19613">Paper</a>
    </div>

  </div>
</div>

---

<!-- ODDR -->
<div style="display:flex; flex-direction:column; gap:18px; margin-bottom:60px;">

  <!-- Image on top -->
  <div style="max-width:600px;">
    <img src="/images/oddr_overview.png" style="width:100%; border-radius:10px; margin-bottom:8px;">
  </div>

  <!-- Text underneath -->
  <div style="max-width:900px;">

    <div style="font-size:0.9rem; font-weight:400; margin-bottom:8px; line-height:1.15;">
      ICCV 2025: 
      <a href="/project_pages/tesser/">ODDR: Outlier Detection & Dimension Reduction Based Defense Against Adversarial Patches</a>
    </div>

    <div style="font-size:0.7rem; line-height:1.6; margin-bottom:12px; text-align:justify;">
      In this paper, we propose Outlier Detection and Dimension Reduction (ODDR), a comprehensive defense strategy engineered to counteract patch-based adversarial attacks through advanced statistical methodologies. Our approach is based on the observation that input features corresponding to adversarial patches--whether naturalistic or synthetic--deviate from the intrinsic distribution of the remaining image data and can thus be identified as outliers. ODDR operates through a robust three-stage pipeline: Fragmentation, Segregation, and Neutralization. This model-agnostic framework is versatile, offering protection across various tasks, including image classification, object detection, and depth estimation, and is proved effective in both CNN-based and Transformer-based architectures. In the Fragmentation stage, image samples are divided into smaller segments, preparing them for the Segregation stage, where advanced outlier detection techniques isolate anomalous features linked to adversarial perturbations. The Neutralization stage then applies dimension reduction techniques to these outliers, effectively neutralizing the adversarial impact while preserving critical information for the machine learning task.
    </div>

    <div>
      <a href="/project_pages/oddr/">Project</a> |
      <a href="[https://arxiv.org/abs/2505.19613](https://openaccess.thecvf.com/content/ICCV2025/html/Chattopadhyay_ODDR_Outlier_Detection__Dimension_Reduction_Based_Defense_Against_Adversarial_ICCV_2025_paper.html)">Paper</a>
    </div>

  </div>
</div>

---

<!-- DAP -->
<div style="display:flex; flex-direction:column; gap:18px; margin-bottom:60px;">

  <!-- Image on top -->
  <div style="max-width:600px;">
    <img src="/images/DAP_teaser.png" style="width:100%; border-radius:10px;">
  </div>

  <!-- Text underneath -->
  <div style="max-width:900px;">

    <div style="font-size:0.9rem; font-weight:400; margin-bottom:8px; line-height:1.15;">
      CVPR 2024: 
      <a href="/project_pages/dap/">DAP: Dynamic Adversarial Patch</a>
    </div>

    <div style="font-size:0.7rem; line-height:1.6; margin-bottom:12px; text-align:justify;">
    This paper introduces a novel approach that produces a Dynamic Adversarial Patch (DAP) designed to overcome these limitations. DAP maintains a naturalistic appearance while optimizing attack efficiency and robustness to real-world transformations. The approach involves redefining the optimization problem and introducing a novel objective function that incorporates a similarity metric to guide the patch's creation. Unlike GAN-based techniques the DAP directly modifies pixel values within the patch providing increased flexibility and adaptability to multiple transformations. Furthermore most clothing-based physical attacks assume static objects and ignore the possible transformations caused by non-rigid deformation due to changes in a person's pose. To address this limitation aCreases Transformation'(CT) block is introduced enhancing the patch's resilience to a variety of real-world distortions.
    </div>

    <div>
      <a href="/project_pages/dap/">Project</a> |
      <a href="#">Paper</a>
    </div>

  </div>
</div>

---

<!-- SSAP -->
<div style="display:flex; flex-direction:column; gap:18px; margin-bottom:60px;">

  <!-- Image on top -->
  <div style="max-width:600px;">
    <img src="/images/ssap_overview.png" style="width:100%; border-radius:10px;">
  </div>

  <!-- Text underneath -->
  <div style="max-width:900px;">

    <div style="font-size:0.9rem; font-weight:400; margin-bottom:8px; line-height:1.15;">
      IROS 2024: 
      <a href="/project_pages/ssap/">SSAP: A Shape-Sensitive Adversarial Patch</a>
    </div>

    <div style="font-size:0.7rem; line-height:1.6; margin-bottom:12px; text-align:justify;">
    In this paper, we introduce SSAP (Shape-Sensitive Adversarial Patch), a novel approach designed to comprehensively disrupt monocular depth estimation (MDE) in autonomous navigation applications. Our patch is crafted to selectively undermine MDE in two distinct ways: by distorting estimated distances or by creating the illusion of an object disappearing from the system’s perspective. Notably, our patch is shape-sensitive, meaning it considers the specific shape and scale of the target object, thereby extending its influence beyond immediate proximity. Furthermore, our patch is trained to effectively address different scales and distances from the camera.
    </div>

    <div>
      <a href="/project_pages/ssap/">Project</a> |
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
