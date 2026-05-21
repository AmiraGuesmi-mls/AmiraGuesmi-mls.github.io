---
layout: single
title: ""
permalink: /
author_profile: true
---

I lead research on AI security and trustworthy machine learning, with a focus on adversarial attacks and defenses, robustness under deployment constraints, and secure perception systems. My work bridges theory, system-level design, and real-world evaluation, targeting vision, autonomous, embedded, and multimodal AI systems.

---

## 🔥 News
- **2026.05**: I've received a **Silver Reviewer Award** from **ICML 2026**
- **2026.01**: 🎉 2 papers accepted at **ICLR 2026**
- **2025.11**: 🎉 1 paper accepted at **DATE 2026**
- **2025.10**: I've been selected as **Top Reviewer** at **NeurIPS 2025** 
- **2025.06**: 🎉 1 paper accepted at **ICCV 2025**
- **2024.06**: 🎉 1 paper accepted at **IROS 2024**
- **2024.06**: 🎉 3 papers accepted at **ICIP 2024**
- **2024.02**: 🎉 1 paper accepted at **CVPR 2024**
- **2024.02**: 🎉 1 paper accepted at **DAC 2024** 


---

## Research Overview

My research aims to advance the security, robustness, and trustworthiness of machine learning systems under adversarial threats and realistic deployment constraints. I study how architecture choices, quantization and approximation, physical-world effects, and multimodal interactions shape both vulnerabilities and defenses. 

I work on the following research topics:

- Adversarial Machine Learning and Robust Optimization
- Security of Autonomous and Embodied AI Systems
- Deployment-Aware and Edge AI Security
- Explainability and Interpretability for Robustness
- Security, Jailbreaks and Hallucination in Large Language and Vision–Language Models
- Privacy and Robustness of Multimodal AI Agents

---

## Selected Research Projects

Below are representative research projects spanning adversarial machine learning, robustness, and secure AI systems.  

---

<!-- DRIFT -->

<div style="display:flex; flex-direction:column; gap:18px; margin-bottom:60px;">

  <!-- Image on top -->
  <div style="max-width:600px;">
    <img src="/images/drift_method.png"
         style="width:100%; border-radius:10px;">
  </div>

  <!-- Text underneath -->
  <div style="max-width:900px;">

    <div style="font-size:0.9rem; font-weight:400; margin-bottom:8px;">
      ICLR 2026:
      <a href="/project_pages/drift/">
        DRIFT: Divergent Response in Filtered Transformations for Robust Adversarial Defense
      </a>
        <p style="font-size:0.9em; font-style:italic; color:#555;">
          Authors: <u><b>Amira Guesmi</b></u>, Muhammad Shafique
        </p>
    </div>

    <div style="font-size:0.9rem; line-height:1.6; margin-bottom:12px; text-align:justify;">
      Shows that adversarial robustness can be achieved by breaking gradient consensus rather than masking gradients, introducing stochastic filter ensembles that induce controlled divergence across model responses and remain effective under adaptive attacks.
    </div>

    <div>
      <a href="/project_pages/drift/">Project</a> |
      <a href="#">Paper</a>
    </div>
    
  </div>

</div>

---

<!-- TriQDef -->

<div style="display:flex; flex-direction:column; gap:18px; margin-bottom:60px;">

  <!-- Image on top -->
  <div style="max-width:600px;">
    <img src="/images/triqdef_method.png" style="width:100%; border-radius:10px;">
  </div>

  <!-- Text underneath -->
  <div style="max-width:900px;">

    <div style="font-size:0.9rem; font-weight:400; margin-bottom:8px">
      ICLR 2026: 
      <a href="/project_pages/triqdef/">TriQDef: Disrupting Semantic and Gradient Alignment to Prevent Adversarial Patch Transferability in Quantized Neural Networks
          </a>
        <p style="font-size:0.9em; font-style:italic; color:#555;">
          Authors: <u><b>Amira Guesmi</b></u>, Bassem Ouni, Muhammad Shafique
        </p>
    </div>

    <div style="font-size:0.9rem; line-height:1.6; margin-bottom:12px; text-align:justify;">
      Reveals that adversarial patch transferability in quantized models is driven by hidden structural consistency across bit-widths, and proposes mechanisms to explicitly disrupt this alignment at both feature and gradient levels.
    </div>

    <div>
      <a href="/project_pages/triqdef/">Project</a> |
      <a href="#">Paper</a>
    </div>

  </div>
</div>

---
<!-- BCR -->
<div style="display:flex; flex-direction:column; gap:18px; margin-bottom:60px;">

  <!-- Image on top -->
  <div style="max-width:600px;">
    <img src="/images/bcr.png" style="width:100%; border-radius:10px; margin-bottom:8px;">
  </div>

  <!-- Text underneath -->
  <div style="max-width:900px;">

    <div style="font-size:0.9rem; font-weight:400; margin-bottom:8px; line-height:1.15;">
      ArXiv 2025: 
      <a href="/project_pages/bcr/">Do Not Leave a Gap: Hallucination-Free Object Concealment in Vision-Language Models
          </a>
        <p style="font-size:0.9em; font-style:italic; color:#555;">
          Authors: <u><b>Amira Guesmi</b></u>, Muhammad Shafique
        </p>
    </div>

    <div style="font-size:0.9rem; line-height:1.6; margin-bottom:12px; text-align:justify;">
    Demonstrates that hallucination in vision-language models is driven by representational gaps rather than object absence, and introduces Background-Consistent Re-encoding to enforce continuity and prevent hallucinated content.
    </div>

    <div>
      <a href="/project_pages/bcr/">Project</a> |
      <a href="[https://arxiv.org/abs/2505.19613](https://arxiv.org/abs/2603.15940)">Paper</a>
    </div>

  </div>
</div>


---
<!-- TESSER -->
<div style="display:flex; flex-direction:column; gap:18px; margin-bottom:60px;">

  <!-- Image on top -->
  <div style="max-width:600px;">
    <img src="/images/tesser_method.png" style="width:100%; border-radius:10px; margin-bottom:8px;">
  </div>

  <!-- Text underneath -->
  <div style="max-width:900px;">

    <div style="font-size:0.9rem; font-weight:400; margin-bottom:8px; line-height:1.15;">
      ArXiv 2025: 
      <a href="/project_pages/tesser/">TESSER: Transfer-Enhancing Adversarial Attacks from Vision Transformers
          </a>
        <p style="font-size:0.9em; font-style:italic; color:#555;">
          Authors: <u><b>Amira Guesmi</b></u>, Bassem Ouni, Muhammad Shafique
        </p>
    </div>

    <div style="font-size:0.9rem; line-height:1.6; margin-bottom:12px; text-align:justify;">
      Establishes that adversarial transferability depends on preserving shared spectral and semantic structures, and introduces a framework that explicitly enforces this alignment to improve cross-model attack generalization.
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
    <img src="/images/oddr_method.png" style="width:100%; border-radius:10px; margin-bottom:8px;">
  </div>

  <!-- Text underneath -->
  <div style="max-width:900px;">

    <div style="font-size:0.9rem; font-weight:400; margin-bottom:8px; line-height:1.15;">
      ICCV 2025: 
      <a href="/project_pages/oddr/">ODDR: Outlier Detection & Dimension Reduction Based Defense Against Adversarial Patches
          </a>
        <p style="font-size:0.9em; font-style:italic; color:#555;">
          Authors: Nandish Chattopadhyay*, <u><b>Amira Guesmi*</b></u>, Muhammad Abdullah Hanif, Bassem Ouni, Muhammad Shafique
        </p>
    </div>

    <div style="font-size:0.9rem; line-height:1.6; margin-bottom:12px; text-align:justify;">
      Frames adversarial patches as feature-space outliers, and introduces a dimension reduction framework that suppresses their influence by removing structurally inconsistent features while preserving clean model behavior.
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
    <img src="/images/dap_method.png" style="width:100%; border-radius:10px;">
  </div>

  <!-- Text underneath -->
  <div style="max-width:900px;">

    <div style="font-size:0.9rem; font-weight:400; margin-bottom:8px; line-height:1.15;">
      CVPR 2024: 
      <a href="/project_pages/dap/">DAP: A Dynamic Adversarial Patch for Evading Person Detectors
          </a>
        <p style="font-size:0.9em; font-style:italic; color:#555;">
          Authors: <u><b>Amira Guesmi</b></u>, Ruitian Ding, Muhammad Abdullah Hanif, Ihsen Alouani, Muhammad Shafique
        </p>
    </div>

    <div style="font-size:0.9rem; line-height:1.6; margin-bottom:12px; text-align:justify;">
    Developed a dynamic adversarial patch framework for wearable, printable T-shirt attacks, enabling person hiding from smart surveillance systems under real-world pose changes, fabric deformation, and physical deployment variations.
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
    <img src="/images/ssap_method.png" style="width:100%; border-radius:10px;">
  </div>

  <!-- Text underneath -->
  <div style="max-width:900px;">

    <div style="font-size:0.9rem; font-weight:400; margin-bottom:8px; line-height:1.15;">
      IROS 2024: 
      <a href="/project_pages/ssap/">SSAP: A Shape-Sensitive Adversarial Patch for Monocular Depth Estimation
          </a>
        <p style="font-size:0.9em; font-style:italic; color:#555;">
          Authors: <u><b>Amira Guesmi</b></u>, Muhammad Abdullah Hanif, Ihsen Alouani, Bassem Ouni, Muhammad Shafique
        </p>
    </div>

    <div style="font-size:0.9rem; line-height:1.6; margin-bottom:12px; text-align:justify;">
    Introduced a shape-sensitive adversarial patch framework that extends attack impact from localized regions to full-object disruption, enabling stronger and more comprehensive degradation of depth estimation in autonomous perception systems.
    </div>

    <div>
      <a href="/project_pages/ssap/">Project</a> |
      <a href="#">Paper</a>
    </div>

  </div>
</div>

---
## 💼 Experience

*Oct 2022 – Present*: Research Team Lead, Engineering Division, New York University Abu Dhabi (NYUAD), UAE  

*Nov 2021 – Aug 2022*: Postdoctoral Researcher, IEMN-DOAE Laboratory, CNRS-8520, Polytechnic University Hauts-de-France, France  

---

## 📖 Education

*Mar 2018 - Oct 2021*: Ph.D. in Computer Systems Engineering, National School of Engineers of Sfax, Tunisia
  
*Sep 2013 - Jun 2016*: Engineer Degree in Computer Science & Electrical Engineering, National School of Engineers of Sfax (ENIS), Tunisia  
 
---

## 🏆 Awards & Honors

- **Silver Reviewer Award**, ICML 2026.
- **Top Reviewer Award**, NeurIPS 2025.
- **Best Senior Researcher Award**, eBRAIN Lab, NYUAD, 2023.
- **Erasmus+ Scholarship**, France, 2019.
- **DAAD Scholarship**: Advanced Technologies based on IoT (ATIoT), Germany, 2018.
- **DAAD Scholarship**: Young ESEM Program (Embedded Systems for Energy Management), Germany, 2016.

---

## 🧑‍🏫 Academic Service & Community

- **Conference Reviewer**: ICML, ICLR, NeurIPS, ICCV, CVPR, AAAI, ECCV, DAC
- **Journal Reviewer**: IEEE TIFS, TCSVT, TCAD, Access 
- **Organizer & Speaker**: Tutorial: *ML Security in Autonomous Systems*, IROS 2024  

---

## 📬 Contact & Links

- **Email**: ag9321@nyu.edu  

I am always open to collaborations on **AI security, adversarial robustness, and trustworthy ML systems**.
