<style>
.page__content p,
.page__content li {
  font-size: 0.90rem;
  line-height: 1.4;
}

.page__content p {
  margin-bottom: 0.7em;
}

.page__content li {
  margin-bottom: 0.15em;
}
</style>

I work on **robustness, security, and trustworthy AI**, with a focus on understanding how AI systems behave beyond controlled settings and how their vulnerabilities emerge across models, modalities, and deployment conditions.
My research spans machine learning, computer vision, multimodal AI, robotics, and computer systems, with work published at top-tier venues including **ICLR, CVPR, ICCV, ECCV, IROS, ASPLOS, DAC, and DATE**.
A recurring theme in my research is understanding what carries across AI systems—in gradients, representations, semantics, or computational structure—and how these shared properties can make models both effective and vulnerable. I study these questions across adversarial transferability, physical-world attacks, quantized and approximate models, and, more recently, vision-language and multimodal systems.
Rather than treating these as separate problems, I approach them through a common lens: understanding what transfers across models, representations, and deployment settings, and how it can be leveraged or disrupted to build more robust systems.

My research includes:

- **Adversarial Transferability** — understanding why adversarial examples transfer across architectures and how shared representations, gradients, and semantics influence transfer.
- **Robust & Efficient AI** — designing defenses that remain effective under quantization, approximate computing, and hardware/deployment constraints.
- **Physical-World AI Security** — studying attacks and defenses under real-world transformations such as viewpoint, deformation, distance, and environmental variation.
- **Multimodal & VLM Security** — investigating hallucination, adversarial manipulation, jailbreaking, and cross-modal inconsistencies in vision-language models.

More broadly, my goal is to uncover the computational principles that govern robustness and failure in modern AI systems, and use these insights to build AI that is reliable, interpretable, and robust under real-world conditions.

<p align="center">
<strong>20+ Publications</strong> · <strong>550+ Citations</strong> · <strong>h-index 12</strong> · <strong>10+ Researchers Mentored</strong>
</p>

<!-- <img src="/images/homepage_fig.png" style="width:100%; border-radius:10px;"> -->
---

## 🔥 News
- **2026.07**: I've received an **Outstanding Reviewer Award** from **ECCV 2026**
- **2026.07**: My paper had been selected for an ECCV 2026 **Oral Presentation**
- **2026.06**: 🎉 1 paper accepted at **ECCV 2026**
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
## Selected Research Projects

Below are representative research projects spanning adversarial machine learning, robustness, and secure AI systems.  

---
<!-- BCR -->
<div style="display:flex; flex-direction:column; gap:18px; margin-bottom:60px;">

  <!-- Image on top -->
  <div style="max-width:600px;">
    <img src="/images/BCR_eccv.png" style="width:100%; border-radius:10px; margin-bottom:8px;">
  </div>

  <!-- Text underneath -->
  <div style="max-width:900px;">

    <div style="font-size:0.9rem; font-weight:400; margin-bottom:8px; line-height:1.15;">
      ECCV 2026: 
      <a href="/project_pages/bcr/">Do Not Leave a Gap: Hallucination-Free Object Concealment in Vision-Language Models
          </a>
        <p style="font-size:0.9em; font-style:italic; color:#555;">
          Authors: <u><b>Amira Guesmi</b></u>, Muhammad Shafique
        </p>
    </div>

    <div style="font-size:0.9rem; line-height:1.6; margin-bottom:12px; text-align:justify;">
    Shows that suppression-based attacks in vision-language models create representational discontinuities that lead to hallucination. Introduces a re-encoding strategy that restores consistency between regions and prevents these failures.
    </div>

    <div>
      <a href="/project_pages/bcr/">Project</a> |
      <a href="https://arxiv.org/abs/2603.15940">Paper</a>
    </div>

  </div>
</div>

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
      Identifies gradient consensus as a key source of adversarial vulnerability, where different transformations still produce aligned attack directions. Proposes stochastic filter ensembles to enforce gradient divergence and improve robustness.
    </div>

    <div>
      <a href="/project_pages/drift/">Project</a> |
      <a href="https://arxiv.org/abs/2509.24359">Paper</a>
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
      Reveals that adversarial patch transferability across quantized models is driven by hidden cross-bit alignment in gradients and feature structure. Introduces a training framework that explicitly disrupts this alignment to prevent transfer.
    </div>

    <div>
      <a href="/project_pages/triqdef/">Project</a> |
      <a href="https://arxiv.org/abs/2508.12132">Paper</a>
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
      Shows that adversarial transferability can be strengthened by preserving spectral and semantic structure across models. Introduces regularization techniques that stabilize these shared components to improve black-box attack effectiveness.
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
          Authors: Nandish Chattopadhyay*, <u><b>Amira Guesmi*</b></u>, Muhammad Abdullah Hanif, Bassem Ouni, Muhammad Shafique (* equal contribution)
        </p>
    </div>

    <div style="font-size:0.9rem; line-height:1.6; margin-bottom:12px; text-align:justify;">
      Frames adversarial patches as structured outliers in feature space rather than random perturbations. Combines outlier detection and dimensionality reduction to localize and neutralize patch-induced distortions.
    </div>

    <div>
      <a href="/project_pages/oddr/">Project</a> |
      <a href="(https://openaccess.thecvf.com/content/ICCV2025/html/Chattopadhyay_ODDR_Outlier_Detection__Dimension_Reduction_Based_Defense_Against_Adversarial_ICCV_2025_paper.html)">Paper</a>
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
    Demonstrates that physically robust adversarial patches require adaptation to real-world transformations such as pose and deformation. Introduces a dynamic patch generation framework that maintains effectiveness under these conditions.
    </div>

    <div>
      <a href="/project_pages/dap/">Project</a> |
      <a href="(https://openaccess.thecvf.com/content/CVPR2024/html/Guesmi_DAP_A_Dynamic_Adversarial_Patch_for_Evading_Person_Detectors_CVPR_2024_paper.html)">Paper</a>
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
    Shows that adversarial patches can manipulate geometric perception at the object level, affecting global depth estimation rather than localized regions. Proposes shape-aware perturbations that alter scene understanding.
    </div>

    <div>
      <a href="/project_pages/ssap/">Project</a> |
      <a href="https://ieeexplore.ieee.org/abstract/document/10802252">Paper</a>
    </div>

  </div>
</div>

---

<!-- DA -->
<div style="display:flex; flex-direction:column; gap:18px; margin-bottom:60px;">

  <!-- Image on top -->
  <div style="max-width:600px;">
    <img src="/images/da_method.png" style="width:100%; border-radius:10px;">
  </div>

  <!-- Text underneath -->
  <div style="max-width:900px;">

    <div style="font-size:0.9rem; font-weight:400; margin-bottom:8px; line-height:1.15;">
      ASPLOS 2021: 
      <a href="/project_pages/defensive_appx/">Defensive approximation: securing cnns using approximate computing

          </a>
        <p style="font-size:0.9em; font-style:italic; color:#555;">
          Authors: <u><b>Amira Guesmi</b></u>, Ihsen Alouani, Khaled N Khasawneh, Mouna Baklouti, Tarek Frikha, Mohamed Abid, Nael Abu-Ghazaleh 
        </p>
    </div>

    <div style="font-size:0.9rem; line-height:1.6; margin-bottom:12px; text-align:justify;">
    Reframes approximate computing from a hardware constraint into a mechanism for disrupting adversarial optimization, where reduced precision and stochasticity weaken the reliability of attack gradients.
    </div>

    <div>
      <a href="/project_pages/defensive_appx/">Project</a> |
      <a href="https://dl.acm.org/doi/abs/10.1145/3445814.3446747">Paper</a>
    </div>

  </div>
</div>

---

## 💼 Experience

*Sep 2022 – Present*: Research Team Lead / Postdoctoral Associate, Engineering Division, New York University Abu Dhabi (NYUAD), UAE  

*Feb 2022 – Aug 2022*: Postdoctoral Researcher, IEMN-DOAE Laboratory, CNRS-8520, Polytechnic University Hauts-de-France, France  

---

## 📖 Education

*Mar 2018 - Oct 2021*: Ph.D. in Computer Systems Engineering, National School of Engineers of Sfax, Tunisia
  
*Sep 2013 - Jun 2016*: Engineer Degree in Computer Science & Electrical Engineering, National School of Engineers of Sfax (ENIS), Tunisia  
 
---

## 🏆 Awards & Honors

- **Outstanding Reviewer Award**, ECCV 2026.
- **Silver Reviewer Award**, ICML 2026.
- **Top Reviewer Award**, NeurIPS 2025.
- **Best Senior Researcher Award**, eBRAIN Lab, NYUAD, 2023.
- **Erasmus+ Scholarship**, France, 2019.
- **DAAD Scholarship**: Advanced Technologies based on IoT (ATIoT), Germany, 2018.
- **DAAD Scholarship**: Young ESEM Program (Embedded Systems for Energy Management), Germany, 2016.

---

## 🧑‍🏫 Academic Service & Community

- **Conference Reviewer**: ICML, ICLR, NeurIPS, ICCV, CVPR, AAAI, ECCV, DAC, IROS, ICIP, IJCNN
- **Journal Reviewer**: IEEE TIFS, IEEE TCSVT, TMLR, TMC, IJCV, TCAD, Access
- **Organizer & Speaker**: Tutorial: *ML Security in Autonomous Systems*, IROS 2024  

---

## 📬 Contact & Links

- **Email**: ag9321@nyu.edu  

I am always open to collaborations on **AI security, adversarial robustness, and trustworthy ML systems**.
