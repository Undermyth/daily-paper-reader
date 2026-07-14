---
title: "NiCLIP: Neuroimaging contrastive language-image pretraining model for predicting text from brain activation images"
title_zh: NiCLIP：用于从脑激活图像预测文本的神经影像对比语言-图像预训练模型
authors: "Peraza, J. A., Kent, J. D., Nichols, T. E., Poline, J.-B., de la Vega, A., Laird, A. R."
date: 2026-07-11
pdf: "https://www.biorxiv.org/content/10.1101/2025.06.14.659706v4.full.pdf"
tags: ["query:comp-neuro"]
score: 7.0
evidence: 从脑激活预测认知过程，与推理计算机制相关
tldr: 神经影像学中预测认知过程长期存在挑战，现有功能解码方法依赖有限指标而忽略文本语义。本文提出NiCLIP，基于对比语言-图像预训练，利用23000篇论文对齐脑激活与文本。评估表明使用全文优于摘要，能准确预测情感、语言等认知任务，但受噪声个体数据影响。该模型为定量功能解码提供了强大工具，促进假设生成。
source: biorxiv
selection_source: fresh_fetch
figures_json: "[{\"url\": \"assets/figures/biorxiv/biorxiv-10-1101-2025-06-14-659706-v4/fig-001.webp\", \"caption\": \"\", \"page\": 0, \"index\": 1, \"width\": 1825, \"height\": 1810}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-1101-2025-06-14-659706-v4/fig-002.webp\", \"caption\": \"\", \"page\": 0, \"index\": 2, \"width\": 1722, \"height\": 1984}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-1101-2025-06-14-659706-v4/fig-003.webp\", \"caption\": \"\", \"page\": 0, \"index\": 3, \"width\": 1711, \"height\": 1868}, {\"url\": \"assets/figures/biorxiv/biorxiv-10-1101-2025-06-14-659706-v4/fig-004.webp\", \"caption\": \"\", \"page\": 0, \"index\": 4, \"width\": 1803, \"height\": 1594}]"
tables_json: "[{\"url\": \"assets/tables/biorxiv/biorxiv-10-1101-2025-06-14-659706-v4/table-001.webp\", \"caption\": \"\", \"page\": 0, \"index\": 1, \"width\": 1845, \"height\": 726}, {\"url\": \"assets/tables/biorxiv/biorxiv-10-1101-2025-06-14-659706-v4/table-002.webp\", \"caption\": \"\", \"page\": 0, \"index\": 2, \"width\": 1702, \"height\": 1439}]"
motivation: 现有神经影像元分析解码方法仅使用有限指标，无法捕捉文本语义，亟需对齐脑激活与文本的模型。
method: 基于CLIP对比学习框架，利用23000篇神经科学论文训练文本-脑激活关联，采用认知本体和全文本优化。
result: NiCLIP准确预测组级认知任务（如情感、语言），受限于噪声个体数据；领域微调LLM提升有限。
conclusion: NiCLIP是定量功能解码的显著进步，为神经影像研究提供假设生成和科学发现的强大工具。
---

## 摘要
多年来，从脑激活图中预测认知过程一直是神经科学领域的一个未解问题。元分析功能解码方法旨在通过提供与特定脑区相关的行为特征的定量估计来解决这一问题。现有方法在神经影像元分析中面临内在挑战，特别是在整合出版物中的文本信息时，因为它们依赖于无法捕捉文本语义上下文的有限指标。大型语言模型与先进的深度对比学习模型（如CLIP）的结合，用于将文本与图像对齐，已经彻底改变了神经影像元分析，可能为功能解码挑战提供解决方案。在这项工作中，我们提出了NiCLIP，一个对比语言-图像预训练模型，能够从脑激活模式中预测认知任务、概念和领域。我们利用超过23,000篇神经科学文章来训练一个用于文本-脑关联的CLIP模型。对NiCLIP预测的评估表明，使用全文文章而非摘要，以及使用具有精确任务-概念-领域映射的精心策划的认知本体时，性能最佳。此外，领域特定微调的大型语言模型（如BrainGPT模型）显示出与基础大型语言模型在数值上相似的性能。我们的结果表明，NiCLIP能够从人类连接组项目提供的群体级激活图中准确预测多个领域（如情感、语言、运动）的认知任务，并精确描述特定脑区（包括杏仁核、海马体和颞顶联合区）的功能角色。然而，NiCLIP在处理噪声较大的个体级激活图时显示出局限性。NiCLIP代表了神经影像定量功能解码的重大进展，为研究人员提供了用于假设生成和科学发现的强大工具。

## Abstract
Predicting cognitive processes from brain activation maps has remained an open question within the neuroscience community for many years. Meta-analytic functional decoding methods aim to tackle this issue by providing a quantitative estimation of behavioral profiles associated with specific brain regions. Existing methods face intrinsic challenges in neuroimaging meta-analysis, particularly in consolidating textual information from publications, as they rely on limited metrics that do not capture the semantic context of the text. The combination of large language models (LLMs) with advanced deep contrastive learning models (e.g., CLIP) for aligning text with images has revolutionized neuroimaging meta-analysis, potentially offering solutions to functional decoding challenges. In this work, we present NiCLIP, a contrastive language-image pretrained model that predicts cognitive tasks, concepts, and domains from brain activation patterns. We leveraged over 23,000 neuroscientific articles to train a CLIP model for text-to-brain association. Evaluation of NiCLIP predictions revealed that performance is optimized when using full-text articles instead of abstracts, as well as a curated cognitive ontology with precise task-concept-domain mappings. Furthermore, domain-specific fine-tuned LLMs (e.g., BrainGPT models) show numerically similar performance to their base LLM counterparts. Our results indicated that NiCLIP accurately predicts cognitive tasks from group-level activation maps provided by the Human Connectome Project across multiple domains (e.g., emotion, language, motor) and precisely characterizes the functional roles of specific brain regions, including the amygdala, hippocampus, and temporoparietal junction. However, NiCLIP showed limitations with noisy subject-level activation maps. NiCLIP represents a significant advancement in quantitative functional decoding for neuroimaging, offering researchers a powerful tool for hypothesis generation and scientific discovery.