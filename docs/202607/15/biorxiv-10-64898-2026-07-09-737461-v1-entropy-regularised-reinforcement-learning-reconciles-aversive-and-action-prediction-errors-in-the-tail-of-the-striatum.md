---
title: Entropy regularised reinforcement learning reconciles aversive and action prediction errors in the tail of the striatum
title_zh: 熵正则化强化学习调和纹状体尾部中的厌恶和动作预测误差
authors: "Mahajan, P., Seymour, B."
date: 2026-07-11
pdf: "https://www.biorxiv.org/content/10.64898/2026.07.09.737461v1.full.pdf"
tags: ["query:comp-neuro"]
score: 6.0
evidence: 熵正则化强化学习模型调和尾状核厌恶与动作预测误差，属于计算神经科学主题
tldr: 尾侧纹状体多巴胺信号存在厌恶预测误差与动作预测误差两种对立解释。本文提出熵正则化强化学习模型，使TS多巴胺神经元同时更新厌恶价值和默认策略。威胁信念门控厌恶价值初始化产生TS样活动，默认策略学习生成随习惯形成而衰减的动作预测误差。该模型统一了两种理论，并揭示了TS在潜在威胁下谨慎行为和结果不确定性下稳定学习的规范作用。
source: biorxiv
selection_source: fresh_fetch
figures_json: "[{\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-09-737461-v1/fig-001.webp\", \"caption\": \"\", \"page\": 0, \"index\": 1, \"width\": 1675, \"height\": 659, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-09-737461-v1/fig-002.webp\", \"caption\": \"\", \"page\": 0, \"index\": 2, \"width\": 1687, \"height\": 538, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-09-737461-v1/fig-003.webp\", \"caption\": \"\", \"page\": 0, \"index\": 3, \"width\": 1572, \"height\": 705, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-09-737461-v1/fig-004.webp\", \"caption\": \"\", \"page\": 0, \"index\": 4, \"width\": 1704, \"height\": 1636, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-09-737461-v1/fig-005.webp\", \"caption\": \"\", \"page\": 0, \"index\": 5, \"width\": 1692, \"height\": 1032, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-07-09-737461-v1/fig-006.webp\", \"caption\": \"\", \"page\": 0, \"index\": 6, \"width\": 1695, \"height\": 332, \"label\": \"Figure\"}]"
tables_json: "[{\"url\": \"assets/tables/biorxiv/biorxiv-10-64898-2026-07-09-737461-v1/table-001.webp\", \"caption\": \"\", \"page\": 0, \"index\": 1, \"width\": 1696, \"height\": 975, \"label\": \"Table\"}]"
motivation: 调和尾侧纹状体多巴胺的厌恶与动作预测误差两种理论，揭示其共存机制。
method: 构建熵正则化强化学习模型，使TS多巴胺神经元同时更新厌恶价值和默认策略。
result: 模型再现了支持两种观点的关键响应模式和仿真结果，信号随习惯形成而衰减。
conclusion: 统合模型揭示了TS在谨慎行为和结果不确定性下稳定学习中的规范作用。
---

## 摘要
纹状体尾部（TS）中的多巴胺活动为多巴胺的强化学习理论带来了新的挑战。一些研究表明，投射到TS的多巴胺信号编码厌恶或威胁预测误差，而另一些研究则认为它们编码参与软习惯形成的动作预测误差。在这里，我们表明这些解释不一定相互排斥。我们实例化了一个熵正则化强化学习模型，其中投射到TS的多巴胺神经元同时更新厌恶值和默认策略。在该模型中，威胁信念门控厌恶值初始化，在从潜在威胁的新奇物体撤退时产生类似TS的活动，而默认策略学习产生动作预测误差信号，随着动作变得习惯化而衰减。我们的结果进一步表明为什么这两种信号可能需要共存于我们模型中的时间差分误差中，并定性地重现了先前用于支持这两种观点的研究中的关键反应模式和模拟。除了这种描述性调和之外，我们的模型模拟还强调了纹状体尾部在潜在威胁背景下的谨慎行为以及在结果不确定性面前的稳定学习中的规范性作用。

## Abstract
AO_SCPLOWBSTRACTC_SCPLOWDopamine activity in the tail of the striatum (TS) presents a novel challenge for reinforcement-learning theories of dopamine. Some studies suggest that TS-projecting dopamine signals encode aversive or threat prediction errors, whereas others argue that they encode action prediction errors involved in soft-habit formation. Here, we show that these accounts need not be mutually exclusive. We instantiate an entropy-regularised reinforcement-learning model in which TS-projecting dopamine neurons update both aversive values and the default policy. In this model, threat belief gates aversive value initialisations, producing TS-like activity during retreat from potentially threatening novel objects, while default-policy learning generates action prediction error signals that decline as actions become habitual. Our results further suggest why both of these signals may need to coexist in the temporal difference errors in our model, and qualitatively reproduce key response patterns and simulations from studies previously used to support both views. Beyond this descriptive reconciliation, our model simulations also highlight the normative role of the tail of the striatum in cautious behaviours in the context of potential threats and stable learning in the face of outcome uncertainty.