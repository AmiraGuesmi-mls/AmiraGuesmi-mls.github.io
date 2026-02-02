---
title: "DAP: A Dynamic Adversarial Patch for Evading Person Detectors"
collection: portfolio
permalink: /project_pages/dap/
date: 2024-06-01
venue: "CVPR"
paperurl: "https://openaccess.thecvf.com/content/CVPR2024/html/Guesmi_DAP_A_Dynamic_Adversarial_Patch_for_Evading_Person_Detectors_CVPR_2024_paper.html"
codeurl: ""
bibtexurl: ""
authors: "Amira Guesmi, Ruitian Ding, Muhammad Abdullah Hanif, Ihsen Alouani, Muhammad Shafique"
excerpt: "A dynamic adversarial patch that adapts spatially and temporally to effectively evade modern person detection models under realistic conditions."
header:
  teaser: /images/dap_teaser.png
  image: /images/dap_overview.png
  caption: "Overview of the DAP framework."
---

## Links
- **Paper:** [CVPR Open Access]({{ page.paperurl }})
{% if page.codeurl and page.codeurl != "" %}- **Code:** [GitHub]({{ page.codeurl }}){% endif %}
{% if page.bibtexurl and page.bibtexurl != "" %}- **BibTeX:** [Download]({{ page.bibtexurl }}){% endif %}

## Overview
<img src="{{ page.header.image | relative_url }}" alt="DAP Overview" style="max-width:100%; border-radius: 8px;"/>

## Abstract
Patch-based adversarial attacks were proven to compromise the robustness and reliability of computer vision systems.
However, their conspicuous and easily detectable nature challenge their practicality in real-world setting. To address this, recent work has proposed using Generative Adversarial Networks (GANs) to generate naturalistic patches that may not attract human attention. However, such approaches suffer from a limited latent space making it challenging to produce a patch that is efficient, stealthy, and robust to multiple real-world transformations.
This paper introduces a novel approach that produces a Dynamic Adversarial Patch (DAP) designed to overcome these limitations. DAP maintains a naturalistic appearance while optimizing attack efficiency and robustness to real-world transformations.
The approach involves redefining the optimization problem and introducing a novel objective function that incorporates a similarity metric to guide the patch's creation. Unlike GAN-based techniques, the DAP directly modifies pixel values within the patch, providing increased flexibility and adaptability to multiple transformations. Furthermore, most clothing-based physical attacks assume static objects and ignore the possible transformations caused by non-rigid deformation due to changes in a person’s pose. To address this limitation, a `Creases Transformation' (CT) block is introduced, enhancing the patch's resilience to a variety of real-world distortions.
Experimental results demonstrate that the proposed approach outperforms state-of-the-art attacks, achieving a success rate of up to 82.28\% in the digital world when targeting the YOLOv7 detector and 65\% in the physical world when targeting YOLOv3tiny detector deployed in edge-based smart cameras. 

## Key Contributions
- We investigate the limitations of GAN-based approaches when used to generate robust naturalistic adversarial patterns. Our investigation reveals that these techniques struggle to integrate multiple transformations while sustaining optimal performance. We show that these techniques can not incorporate multiple transformations while maintaining high performance due to the limited latent space compared to the high flexibility and the larger space provided by our approach as it relies on directly manipulating the patch pixels.
- We propose a framework (See Figure approach) that generates GAN-free naturalistic patches that can resemble any predefined pattern, while maintaining high attack success rate under multiple transformations (e.g., clothing creases and wrinkles, random noise, brightness and contrast variations, re-scaling, and rotation, etc.). 
- To increase robustness against non-rigid deformations experienced by a printed adversarial patch on a T-shirt and caused by pose changes of a moving person, we develop a Creases Transformation (CT) block that models these non-rigid deformations by compressing the pixels following a randomly selected direction.
- We thoroughly examine the performance/attack success rate of the proposed method in terms of mean average precision (mAP) both with and without transformations, and transferability between detectors.  Our patch achieves an attack success rate of 82.28% in the digital world (INRIA dataset) when targeting the YOLOv7 detector and 65% in the physical world when attacking the YOLOv3tiny detector for edge systems.

## Citation
```bibtex
@inproceedings{guesmi2024dap,
  title     = {DAP: A Dynamic Adversarial Patch for Evading Person Detectors},
  author    = {Guesmi, Amira and Ding, Ruitian and Hanif, Muhammad Abdullah and Alouani, Ihsen and Shafique, Muhammad},
  booktitle = {Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition (CVPR)},
  year      = {2024}
}
