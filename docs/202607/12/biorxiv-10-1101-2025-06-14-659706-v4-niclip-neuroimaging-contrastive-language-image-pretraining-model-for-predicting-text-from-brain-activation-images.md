---
title: "NiCLIP: Neuroimaging contrastive language-image pretraining model for predicting text from brain activation images"
title_zh: NiCLIP：用于从脑激活图像预测文本的神经影像对比语言-图像预训练模型
authors: "Peraza, J. A., Kent, J. D., Nichols, T. E., Poline, J.-B., de la Vega, A., Laird, A. R."
date: 2026-07-11
pdf: "https://www.biorxiv.org/content/10.1101/2025.06.14.659706v4.full.pdf"
tags: ["query:comp-neuro"]
score: 7.0
evidence: 对比学习用于从脑激活预测认知过程
tldr: 神经科学中从脑激活图预测认知过程长期存在挑战。现有元分析功能解码依赖有限指标，未捕捉语义。本文提出NiCLIP，利用2.3万篇论文训练的对比语言-图像模型，将文本与脑激活对齐。实验表明全文和精确认知本体最优；能准确预测群体级任务和多脑区功能，但个体级噪声图效果有限。NiCLIP推动了定量功能解码的发展。
source: biorxiv
selection_source: fresh_fetch
figures_json: "[{\"url\": \"assets/figures/biorxiv/biorxiv-10-1101-2025-06-14-659706-v4/fig-001.webp\", \"caption\": \"\", \"page\": 0, \"index\": 1, \"width\": 1825, \"height\": 1810, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-1101-2025-06-14-659706-v4/fig-002.webp\", \"caption\": \"\", \"page\": 0, \"index\": 2, \"width\": 1722, \"height\": 1984, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-1101-2025-06-14-659706-v4/fig-003.webp\", \"caption\": \"\", \"page\": 0, \"index\": 3, \"width\": 1711, \"height\": 1868, \"label\": \"Figure\"}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-1101-2025-06-14-659706-v4/fig-004.webp\", \"caption\": \"\", \"page\": 0, \"index\": 4, \"width\": 1803, \"height\": 1594, \"label\": \"Figure\"}]"
tables_json: "[{\"url\": \"assets/tables/biorxiv/biorxiv-10-1101-2025-06-14-659706-v4/table-001.webp\", \"caption\": \"\", \"page\": 0, \"index\": 1, \"width\": 1845, \"height\": 726, \"label\": \"Table\"}, {\"url\": \"assets/tables/biorxiv/biorxiv-10-1101-2025-06-14-659706-v4/table-002.webp\", \"caption\": \"\", \"page\": 0, \"index\": 2, \"width\": 1702, \"height\": 1439, \"label\": \"Table\"}]"
motivation: 现有脑激活功能解码方法缺乏语义理解，需要更准确的文本-脑关联模型。
method: 基于CLIP架构，使用2.3万篇神经科学文章训练文本-脑激活对比学习模型NiCLIP。
result: 全文优于摘要；精确认知本体提升性能；NiCLIP准确预测HCP群体级任务及特定脑区功能。
conclusion: NiCLIP为神经影像定量功能解码提供了有效工具，支持假设生成与科学发现。
---

## 摘要
从脑激活图预测认知过程多年来一直是神经科学领域的一个未解问题。元分析功能解码方法旨在通过提供与特定脑区相关的行为特征的定量估计来解决这个问题。现有方法在神经影像元分析中面临内在挑战，特别是在整合出版物中的文本信息方面，因为它们依赖于有限的指标，无法捕捉文本的语义背景。将大语言模型（LLM）与先进的深度对比学习模型（如CLIP）相结合以对齐文本和图像，已经彻底改变了神经影像元分析，可能为功能解码挑战提供解决方案。在这项工作中，我们提出了NiCLIP，一个对比语言-图像预训练模型，能够从脑激活模式预测认知任务、概念和领域。我们利用超过23,000篇神经科学文章来训练一个用于文本-脑关联的CLIP模型。对NiCLIP预测的评估显示，使用全文文章而非摘要时性能最优，同时使用具有精确任务-概念-领域映射的策划认知本体也能优化性能。此外，特定领域的微调LLM（如BrainGPT模型）在数值上表现出与基础LLM相似的性能。我们的结果表明，NiCLIP能从人类连接组项目提供的群体级激活图准确预测跨多个领域（如情感、语言、运动）的认知任务，并精确刻画特定脑区（包括杏仁核、海马体和颞顶联合区）的功能角色。然而，NiCLIP在处理噪声较大的个体级激活图时表现出局限性。NiCLIP代表了神经影像定量功能解码的一项重大进展，为研究人员提供了用于假设生成和科学发现的强大工具。

## Abstract
Predicting cognitive processes from brain activation maps has remained an open question within the neuroscience community for many years. Meta-analytic functional decoding methods aim to tackle this issue by providing a quantitative estimation of behavioral profiles associated with specific brain regions. Existing methods face intrinsic challenges in neuroimaging meta-analysis, particularly in consolidating textual information from publications, as they rely on limited metrics that do not capture the semantic context of the text. The combination of large language models (LLMs) with advanced deep contrastive learning models (e.g., CLIP) for aligning text with images has revolutionized neuroimaging meta-analysis, potentially offering solutions to functional decoding challenges. In this work, we present NiCLIP, a contrastive language-image pretrained model that predicts cognitive tasks, concepts, and domains from brain activation patterns. We leveraged over 23,000 neuroscientific articles to train a CLIP model for text-to-brain association. Evaluation of NiCLIP predictions revealed that performance is optimized when using full-text articles instead of abstracts, as well as a curated cognitive ontology with precise task-concept-domain mappings. Furthermore, domain-specific fine-tuned LLMs (e.g., BrainGPT models) show numerically similar performance to their base LLM counterparts. Our results indicated that NiCLIP accurately predicts cognitive tasks from group-level activation maps provided by the Human Connectome Project across multiple domains (e.g., emotion, language, motor) and precisely characterizes the functional roles of specific brain regions, including the amygdala, hippocampus, and temporoparietal junction. However, NiCLIP showed limitations with noisy subject-level activation maps. NiCLIP represents a significant advancement in quantitative functional decoding for neuroimaging, offering researchers a powerful tool for hypothesis generation and scientific discovery.