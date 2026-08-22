---
title: Parametric neural control differentiates top neural network models of primate visual cortex
title_zh: 参数化神经控制区分灵长类视觉皮层的顶级神经网络模型
authors: "Prince, J. S., Wang, B., Fel, T., Jagadeesh, A. V., Vaziri, P. A., Alvarez, G. A., Livingstone, M. S., Konkle, T."
date: 2026-08-20
pdf: "https://www.biorxiv.org/content/10.64898/2026.08.16.745063v1.full.pdf"
tags: ["query:comp-neuro"]
score: 6.0
evidence: 用参数化神经控制方法区分视觉皮层计算模型
tldr: 领先的深度神经网络编码模型在预测灵长类视觉皮层响应时精度几乎无差别，但可能并未收敛到相同的脑对齐参数化。本文提出轴向特征强调方法，将模型的编码轴转化为分级刺激扰动，以参数化控制神经活动。在五个猕猴的闭环实验中，尽管自然图像预测性匹配，模型在控制能力上差异显著，对抗训练模型表现更优，但与控制力相关性较弱，控制力更好由输入梯度的空间频率结构预测。该方法为评估神经元与模型表征对齐提供了因果手段。
source: biorxiv
selection_source: fresh_fetch
motivation: 深度神经网络编码模型预测视觉皮层精度相近，但未必共享相同的脑对齐参数化，缺乏因果验证方法。
method: 提出轴向特征强调，将模型编码轴转化为分级刺激扰动，并在猕猴视觉区进行闭环神经控制实验。
result: 模型控制神经活动能力差异显著，对抗训练模型有优势，且控制力由输入梯度空间频率结构预测。
conclusion: 轴对齐特征强调可作为因果手段评估神经元与模型在视觉空间参数化上的对齐程度。
---

## 摘要
领先的深度神经网络编码模型以几乎无法区分的精度预测视觉皮层反应，这引发了强烈的推断：这些模型已经收敛到相同的、与大脑对齐的自然图像空间参数化上。在这里，我们证明情况并非如此。我们引入了轴对齐特征强调，将每个模型的拟合编码轴转换为分级刺激扰动，这些扰动被预测会在自然图像范围内外参数化地控制神经放电。我们从十个领先视觉模型生成了超过27,500个控制器刺激，并在针对早期、中期和高级视觉区域的闭环实验中将其呈现给五只猕猴。尽管自然图像预测性匹配，模型在利用强调刺激控制神经放电的能力上存在显著差异，揭示出大多数模型编码轴未能捕捉对应神经元的精确调谐。两个对抗训练模型表现出持续优势，尽管对抗鲁棒性仅微弱地预测了其他模型中的神经控制。相反，控制更好地由输入梯度的空间频率结构预测：即影响每个编码轴的像素分布。总体而言，这些结果确立了通过轴对齐特征强调进行神经控制作为一种因果方法，用于评估神经元和模型如何参数化视觉世界之间的对齐程度。

## Abstract
Leading deep neural network encoding models predict visual cortical responses with nearly indistinguishable accuracy, raising the strong inference that these models have converged on the same underlying brain-aligned parameterization of natural image space. Here we demonstrate that this is not the case. We introduce axis-aligned feature accentuation, which converts each model's fitted encoding axis into graded stimulus perturbations that are predicted to parametrically control neural firing within and beyond the natural-image range. We generated over 27,500 controller stimuli from ten leading vision models and presented them to five macaques in closed-loop experiments targeting early, mid-, and high-level visual areas. Despite matched natural image predictivity, models diverged strongly in their ability to control neural firing using accentuated stimuli, revealing that most model encoding axes failed to capture the precise tuning of their corresponding neurons. The two adversarially trained models showed a consistent advantage, though adversarial robustness was only weakly predictive of neural control across other models. Instead, control was better predicted by the spatial frequency structure of the input gradient: the distribution of pixels influencing each encoding axis. Overall, these results establish neural control via axis-aligned feature accentuation as a causal method to assess the alignment between how neurons and models parameterize the visual world.