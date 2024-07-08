---
title: "Defending with Errors: Approximate Computing for Robustness of Deep Neural Networks"
collection: publications
permalink: /publications/ERRORS
venue: "ArXiv"
date: 2022-11-02
citation: '<b>Amira Guesmi</b>, Ihsen Alouani, Khaled N. Khasawneh, Mouna Baklouti, Tarek Frikha, Mohamed Abid, Nael Abu-Ghazaleh'
---
[[PDF]]([(https://arxiv.org/abs/2211.01182)])


## Abstract
Machine-learning architectures, such as Convolutional Neural Networks (CNNs) are vulnerable to adversarial attacks: inputs crafted carefully to force the system output to a wrong label. Since machine-learning is being deployed in safety-critical and security-sensitive domains, such attacks may have catastrophic security and safety consequences. In this paper, we propose for the first time to use hardware-supported approximate computing to improve the robustness of machine-learning classifiers. We show that successful adversarial attacks against the exact classifier have poor transferability to the approximate implementation. Surprisingly, the robustness advantages also apply to white-box attacks where the attacker has unrestricted access to the approximate classifier implementation: in this case, we show that substantially higher levels of adversarial noise are needed to produce adversarial examples. Furthermore, our approximate computing model maintains the same level in terms of classification accuracy, does not require retraining, and reduces resource utilization and energy consumption of the CNN. We conducted extensive experiments on a set of strong adversarial attacks; We empirically show that the proposed implementation increases the robustness of a LeNet-5, Alexnet and VGG-11 CNNs considerably with up to 50% by-product saving in energy consumption due to the simpler nature of the approximate logic.
