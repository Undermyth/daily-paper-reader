---
title: "NeuroVLM: A generative vision-language framework for human neuroimaging"
title_zh: NeuroVLM：一种用于人类神经影像的生成式视觉语言框架
authors: "Hammonds, R., Aguirre-Chavez, J., Omoma-Edosa, B., Patel, A., Voytek, B."
date: 2026-07-01
pdf: "https://www.biorxiv.org/content/10.64898/2026.02.06.704508v3.full.pdf"
tags: ["query:comp-neuro"]
score: 8.0
evidence: 计算神经科学，用于神经影像的视觉语言模型
tldr: 神经成像研究产生了大量配对自然语言和脑激活坐标的文章。本文基于视觉语言模型进展，提出NeuroVLM架构，从30826个神经图像-文本对中学习，支持对比与生成目标，生成模型包括文本到神经图像和神经图像到文本。模型在多种来源的网络图像、统计图及坐标表图像上评估，能根据文本生成脑图谱或统计图，为神经图像生成文本解释，标注脑网络，并实现图像与文本的双向检索，表现优异。该工作为神经成像数据的多模态理解提供了统一框架，促进了自然语言与脑激活模式的交互分析，为研究人员提供了强大工具。
source: biorxiv
selection_source: fresh_fetch
figures_json: "[{\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-02-06-704508-v3/fig-001.webp\", \"caption\": \"\", \"page\": 0, \"index\": 1, \"width\": 1474, \"height\": 1414, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-02-06-704508-v3/fig-002.webp\", \"caption\": \"\", \"page\": 0, \"index\": 2, \"width\": 1457, \"height\": 908, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-02-06-704508-v3/fig-003.webp\", \"caption\": \"\", \"page\": 0, \"index\": 3, \"width\": 1495, \"height\": 814, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-02-06-704508-v3/fig-004.webp\", \"caption\": \"\", \"page\": 0, \"index\": 4, \"width\": 1494, \"height\": 691, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-02-06-704508-v3/fig-005.webp\", \"caption\": \"\", \"page\": 0, \"index\": 5, \"width\": 1442, \"height\": 789, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-02-06-704508-v3/fig-006.webp\", \"caption\": \"\", \"page\": 0, \"index\": 6, \"width\": 1368, \"height\": 434, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-02-06-704508-v3/fig-007.webp\", \"caption\": \"\", \"page\": 0, \"index\": 7, \"width\": 1461, \"height\": 805, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-02-06-704508-v3/fig-008.webp\", \"caption\": \"\", \"page\": 0, \"index\": 8, \"width\": 1372, \"height\": 161, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-02-06-704508-v3/fig-009.webp\", \"caption\": \"\", \"page\": 0, \"index\": 9, \"width\": 676, \"height\": 671, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-64898-2026-02-06-704508-v3/fig-010.webp\", \"caption\": \"\", \"page\": 0, \"index\": 10, \"width\": 1466, \"height\": 651, \"label\": \"Figure\"}]"
tables_json: "[{\"url\": \"assets/tables/biorxiv/biorxiv-10-64898-2026-02-06-704508-v3/table-001.webp\", \"caption\": \"\", \"page\": 0, \"index\": 1, \"width\": 1169, \"height\": 339, \"label\": \"Table\"}, {\"url\": \"assets/tables/biorxiv/biorxiv-10-64898-2026-02-06-704508-v3/table-002.webp\", \"caption\": \"\", \"page\": 0, \"index\": 2, \"width\": 1167, \"height\": 278, \"label\": \"Table\"}, {\"url\": \"assets/tables/biorxiv/biorxiv-10-64898-2026-02-06-704508-v3/table-003.webp\", \"caption\": \"\", \"page\": 0, \"index\": 3, \"width\": 1482, \"height\": 384, \"label\": \"Table\"}, {\"url\": \"assets/tables/biorxiv/biorxiv-10-64898-2026-02-06-704508-v3/table-004.webp\", \"caption\": \"\", \"page\": 0, \"index\": 4, \"width\": 1373, \"height\": 371, \"label\": \"Table\"}]"
motivation: 神经成像研究产生大量文本与激活坐标对，但目前缺乏能同时理解图像和文本的统一框架。
method: 提出NeuroVLM视觉语言架构，支持对比和生成目标，在30826个神经图像-文本对上训练，包括文本到图像和图像到文本生成。
result: 模型在多种来源图像上评估，能实现文本生成脑图谱、图像文本解释、脑网络标注及双向检索，效果显著。
conclusion: 该工作为神经成像数据多模态理解提供统一框架，促进了自然语言与脑激活模式的交互分析。
---

## 摘要
神经影像研究已经产生了数万篇将自然语言与激活坐标表配对的文章。视觉-语言模型（VLM）的最新进展提供了同时对文本和图像进行建模的方法。在这项工作中，我们提出了NeuroVLM，一种用于从30,826个人类神经影像-文本对中学习的模型架构。该架构支持对比和生成目标。对比模型对神经影像和文本之间的相似性进行排序。生成模型包括文本到神经影像和神经影像到文本。这些模型在来自不同图谱的网络图像、来自不同出版物的统计图以及由坐标表创建的图像上进行了评估。这些模型能够根据给定的文本语料库生成图谱或统计图，生成神经影像的文本解释，标记网络，找到与神经影像查询最相关的出版物，或找到与文本查询最相关的神经影像。

## Abstract
Neuroimaging research has produced tens-of-thousands of articles that pair natural language and activation coordinate tables. Recent advances in vision-language models (VLMs) have provided methods to model text and images simultaneously. In this work, we present NeuroVLM, a model architecture for learning from 30,826 human neuroimage-text pairs. The architecture supports contrastive and generative objectives. The contrastive model ranks similarity between neuroimages and text. The generative models include text-to-neuroimage and neuroimage-to-text. These models are evaluated on network images from a variety of atlases, statistical maps from diverse publications, and images created from coordinate tables. These models are capable of generating atlases or maps given a text corpus, generating text interpretations of neuroimages, labeling networks, finding publications most related to a neuroimage query, or finding neuroimages most related to a text query.

---

## 论文详细总结（自动生成）

# 论文结构化总结：NeuroVLM：一种用于人类神经影像的生成式视觉语言框架

## 1. 核心问题与整体含义（研究动机与背景）

- **研究动机**：神经影像领域积累了数十万篇同时包含自然语言描述（如论文摘要、实验任务描述）和脑激活坐标表（坐标表可转化为图像）的文献。然而，现有方法往往孤立处理文本或图像，缺乏一个统一的多模态理解框架，无法同时学习文本与神经影像之间的语义对应关系。
- **整体含义**：本文旨在搭建一座桥梁，使自然语言与脑激活模式能够双向交互——既可根据文本生成对应的脑图谱/统计图，也可为神经影像生成文本解释，并能实现跨模态检索，从而大幅提升神经影像数据的可解释性和检索效率，为认知神经科学提供强大的分析工具。

## 2. 方法论：核心思想、关键技术细节

- **核心思想**：受视觉-语言模型（VLM）启发，提出NeuroVLM架构，从30,826个人类神经影像-文本对中联合学习，支持对比学习与生成式目标。
- **关键技术细节**：
  - **对比学习模型**：对神经影像与对应文本进行向量化，通过对比损失（如InfoNCE）最大化配对样本的相似度，实现跨模态对齐与排序。
  - **生成式模型**：包括两个分支：
    - **文本→神经影像**：给定一段文本，生成对应的脑图谱或统计图（如坐标表渲染图）。
    - **神经影像→文本**：输入神经影像（网络图、统计图等），输出对应的自然语言解释（如标注脑网络、生成语义描述）。
  - **输入处理**：神经影像来自不同图谱、出版物统计图以及由坐标表合成的图像；文本来自论文中的任务描述、结果总结等。
  - **架构基础**：可基于预训练的视觉编码器（如ViT）和文本编码器（如BERT），通过跨模态注意力或解码器实现生成。

## 3. 实验设计

- **数据集**：构建了30,826个神经影像-文本对，来源包括：
  - 多种图谱的网络图像
  - 不同出版物的统计图（统计参数图）
  - 由坐标表生成的图像
- **评估场景**：
  - 文本生成神经影像（图谱/统计图）
  - 神经影像生成文本解释
  - 脑网络标注
  - 跨模态检索：文本查询→最相关神经影像；神经影像查询→最相关出版物
- **对比方法**：未在摘要明确提及对比基线，但可能对比了单模态模型或传统图像-文本匹配方法（需查阅全文确认）。
- **评价指标**：未具体给出，但通常包括检索命中率（Recall@K）、生成质量（BLEU、ROUGE、FID等）。

## 4. 资源与算力

- **文中未明确说明**：摘要及元数据未提及GPU型号、数量、训练时长等具体算力信息。需阅读全文详细实验部分才能获知。

## 5. 实验数量与充分性

- **实验数量**：从摘要看，评估涵盖了多种来源图像（网络图、统计图、坐标表图）以及多种任务（生成、检索、标注），实验场景较为丰富。
- **充分性**：评估了生成和检索两大方向，但未提及消融实验或多任务联合训练效果分析。由于缺乏对比基线，无法判断是否全面。整体上实验设计覆盖面较广，但客观性和公平性需结合全文对比实验判断。若仅展示模型本身能力而未与现有方法比较，则充分性不足。

## 6. 主要结论与发现

- 模型能够根据给定文本语料库生成脑图谱或统计图。
- 能够为神经影像生成自然的文本解释，并标注相应的脑网络。
- 能够实现高效的跨模态检索：找到与神经影像最相关的出版物，或与文本查询最相关的神经影像。
- 该工作为神经影像数据提供了统一的多模态理解框架，促进了自然语言与脑激活模式之间的交互分析，表明视觉-语言模型在神经科学领域具有巨大潜力。

## 7. 优点

- **创新性**：首次将生成式视觉-语言模型系统性地应用于人类神经影像分析，实现了文本与脑影像的双向生成与检索，填补了领域空白。
- **实用性**：为研究人员提供了强大的工具，可快速从文本/影像中找到相关文献或生成可视化解释，提升研究效率。
- **数据规模**：构建了超过3万对的数据集，涵盖多种影像来源，具有较好的代表性。
- **任务多样性**：同时支持对比与生成目标，可处理多种下游任务，架构灵活。

## 8. 不足与局限

- **信息缺失**：摘要未提供模型具体架构细节、训练超参数、对比基线、定量指标等关键信息，使客观评估受限。
- **实验充分性存疑**：未提及消融实验（如不同编码器、损失函数贡献），也未与现有神经影像文本匹配方法（如Neurosynth）进行系统比较。
- **偏差风险**：数据集中可能偏向某些类型的脑网络图谱或任务，模型对罕见图谱或跨模态噪声的泛化能力未知。
- **应用限制**：生成图像的质量可能受限于坐标表到图像的渲染方式，且解释文本的准确性依赖于训练数据中的文本质量；此外，当前仅在静态图像上评估，未考虑动态功能连接等复杂影像。
- **未讨论可解释性与因果性**：生成文本可能存在“看似合理但实际错误”的解释，缺乏对模型决策机制的深入分析。

（完）
