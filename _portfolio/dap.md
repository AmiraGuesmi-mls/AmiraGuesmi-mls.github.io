---
title: "DAP: A Dynamic Adversarial Patch for Evading Person Detectors"
collection: portfolio
permalink: /project_pages/dap/
date: 2024-06-01
venue: "CVPR 2024"
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
Adversarial patch attacks have shown strong potential in evading object detectors; however, existing approaches rely on static patterns that fail to generalize across poses, scales, and environmental changes.  
This paper introduces **DAP**, a **dynamic adversarial patch** that adapts its appearance based on spatial transformations and temporal variations, enabling robust evasion of state-of-the-art person detectors under realistic conditions. Extensive evaluations demonstrate that DAP significantly outperforms static patch baselines across diverse detection models, viewpoints, and deployment scenarios.

## Key Contributions
- Proposes **DAP**, the first dynamic adversarial patch designed for person detection evasion.
- Introduces adaptive spatial and temporal transformations to improve robustness across poses and scales.
- Demonstrates strong attack success against modern person detectors in realistic evaluation settings.

## Citation
```bibtex
@inproceedings{guesmi2024dap,
  title     = {DAP: A Dynamic Adversarial Patch for Evading Person Detectors},
  author    = {Guesmi, Amira and Ding, Ruitian and Hanif, Muhammad Abdullah and Alouani, Ihsen and Shafique, Muhammad},
  booktitle = {Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition (CVPR)},
  year      = {2024}
}
