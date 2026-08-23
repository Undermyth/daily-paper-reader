---
title: Parametric neural control differentiates top neural network models of primate visual cortex
title_zh: 参数化神经控制区分灵长类视觉皮层顶级神经网络模型
authors: "Prince, J. S., Wang, B., Fel, T., Jagadeesh, A. V., Vaziri, P. A., Alvarez, G. A., Livingstone, M. S., Konkle, T."
date: 2026-08-20
pdf: "https://www.biorxiv.org/content/10.64898/2026.08.16.745063v1.full.pdf"
tags: ["query:comp-neuro"]
score: 7.0
evidence: 利用深度神经网络编码模型和闭环神经控制的计算神经科学研究
tldr: "深度神经网络编码模型在自然图像预测上表现近乎相同，但未必共享大脑一致的图像参数化。本文提出轴对齐特征强调，将模型编码轴转为可参数化控制神经放电的刺激扰动，并在五只猕猴多个视觉皮层区域进行闭环实验。基于超过27,500个控制器刺激，发现模型间控制能力差异显著，多数模型未捕获精确调谐；对抗训练模型略具优势，而输入梯度空间频率结构更能预测控制效果。该工作将神经控制确立为评估模型与大脑对齐的因果方法。"
source: biorxiv
selection_source: fresh_fetch
motivation: 深度模型预测猕猴视觉反应精度相当，但潜在编码机制是否真正对齐大脑尚不明朗，亟需因果性手段加以区分。
method: "提出轴对齐特征强调，将编码轴转换为递增刺激扰动，生成27,500余控制器刺激，并针对五只猕猴的早、中、高层视觉区开展闭环验证。"
result: 模型间神经控制能力差异显著，多数模型未能捕捉精细调谐；对抗训练模型较优，但输入梯度空间频率结构对控制效果的预测力更强。
conclusion: 轴对齐特征强调可作为因果工具，用于甄别模型与视觉皮层参数化的一致性，为模型评估提供新范式。
---

## 摘要
领先的深度神经网络编码模型预测视觉皮层反应的准确度几乎无法区分，这强有力地推断这些模型已经收敛到相同的、与大脑对齐的自然图像空间参数化。在此我们证明情况并非如此。我们引入了轴对齐特征强调，将每个模型的拟合编码轴转换为渐进的刺激扰动，这些扰动预计能够在自然图像范围内外参数化地控制神经放电。我们从十个领先视觉模型生成了超过27,500个控制器刺激，并在针对早期、中期和高级视觉区域的闭环实验中展示给五只猕猴。尽管自然图像预测性匹配，模型在使用强调刺激控制神经放电的能力上差异显著，揭示出大多数模型编码轴未能捕捉其对应神经元的精确调谐。两个对抗训练模型表现出持续的优势，尽管对抗鲁棒性在其他模型中仅对神经控制有弱预测性。相反，控制更好地由输入梯度的空间频率结构预测：影响每个编码轴的像素分布。总体而言，这些结果确立了通过轴对齐特征强调的神经控制作为一种因果方法，用于评估神经元和模型如何参数化视觉世界之间的对齐。

## Abstract
Leading deep neural network encoding models predict visual cortical responses with nearly indistinguishable accuracy, raising the strong inference that these models have converged on the same underlying brain-aligned parameterization of natural image space. Here we demonstrate that this is not the case. We introduce axis-aligned feature accentuation, which converts each model's fitted encoding axis into graded stimulus perturbations that are predicted to parametrically control neural firing within and beyond the natural-image range. We generated over 27,500 controller stimuli from ten leading vision models and presented them to five macaques in closed-loop experiments targeting early, mid-, and high-level visual areas. Despite matched natural image predictivity, models diverged strongly in their ability to control neural firing using accentuated stimuli, revealing that most model encoding axes failed to capture the precise tuning of their corresponding neurons. The two adversarially trained models showed a consistent advantage, though adversarial robustness was only weakly predictive of neural control across other models. Instead, control was better predicted by the spatial frequency structure of the input gradient: the distribution of pixels influencing each encoding axis. Overall, these results establish neural control via axis-aligned feature accentuation as a causal method to assess the alignment between how neurons and models parameterize the visual world.