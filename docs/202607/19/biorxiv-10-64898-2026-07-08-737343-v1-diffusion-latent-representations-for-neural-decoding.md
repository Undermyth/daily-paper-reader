---
title: Diffusion Latent Representations for Neural Decoding
title_zh: 面向神经解码的扩散潜在表示
authors: "Wong, B., Laschowski, B."
date: 2026-07-13
pdf: "https://www.biorxiv.org/content/10.64898/2026.07.08.737343v1.full.pdf"
tags: ["query:comp-neuro"]
score: 6.0
evidence: 扩散潜表示用于神经解码
tldr: "神经解码可视为表示学习问题，中间表示的选择影响性能和学习难度。本文提出一个框架，利用不同扩散时间步的潜在表示作为中间表示进行神经语音解码。实验发现，教师强制词错误率在不同时间步差异显著，最佳可达3.5%。结果表明扩散潜在表示有效但强烈依赖时间步选择，该框架为系统研究中间表示的影响提供了基础。"
source: biorxiv
selection_source: fresh_fetch
figures_json: "[{\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-08-737343-v1/fig-001.webp\", \"caption\": \"\", \"page\": 0, \"index\": 1, \"width\": 1864, \"height\": 1043}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-08-737343-v1/fig-002.webp\", \"caption\": \"\", \"page\": 0, \"index\": 2, \"width\": 1837, \"height\": 1094}]"
tables_json: "[{\"url\": \"assets/tables/biorxiv/biorxiv-10-64898-2026-07-08-737343-v1/table-001.webp\", \"caption\": \"\", \"page\": 0, \"index\": 1, \"width\": 931, \"height\": 193}, {\"url\": \"assets/tables/biorxiv/biorxiv-10-64898-2026-07-08-737343-v1/table-002.webp\", \"caption\": \"\", \"page\": 0, \"index\": 2, \"width\": 929, \"height\": 159}]"
motivation: 研究中间表示选择对神经解码下游学习和重建效果的影响。
method: 提出框架，使用不同扩散时间步的潜在表示作为中间表示进行语音解码。
result: "教师强制词错误率在44.7%、7.5%和3.5%之间变化，时间步选择至关重要。"
conclusion: 扩散潜在表示有效但依赖时间步，框架可系统研究中间表示的影响。
---

## 摘要
神经解码可被视为一个表示学习问题，其中神经活动在下游重建前被映射到中间表示。中间表示的选择影响性能和学习难度。我们开发了一个新框架，用于研究中间表示选择如何影响下游学习和重建。作为概念验证，我们使用从不同扩散时间步提取的扩散潜在表示进行神经语音解码，实例化了该框架。逐分量评估显示，不同扩散时间步的重建性能差异显著，不同潜在模型的教师强迫词错误率分别为44.7%、7.5%和3.5%。这些结果表明扩散潜在表示可作为从神经活动中学习的有效中间表示，但其有效性强烈依赖于所选扩散时间步。更广泛地，我们的框架为系统研究中间表示选择如何影响下游学习和重建提供了基础。

## Abstract
Neural decoding can be viewed as a representation learning problem in which neural activity is mapped into an intermediate representation before downstream reconstruction. The choice of intermediate representation influences both performance and learning difficulty. Here we developed a novel framework for studying how intermediate representation choice influences downstream learning and reconstruction. As a proof-of-concept, we instantiated our framework using diffusion latent representations extracted from different diffusion timesteps for neural speech decoding. Component-wise evaluation showed that reconstruction performance differed substantially across diffusion timesteps, with teacher-forced Word Error Rates of 44.7%, 7.5%, and 3.5% for different latent models. These results demonstrate that diffusion latent representations can serve as effective intermediate representations for learning from neural activity, but that their effectiveness depends strongly on the selected diffusion timestep. More broadly, our framework provides a basis for systematically studying how intermediate representation choice influences downstream learning and reconstruction.