<div class="dpr-home-notice-card">
  <h3 class="dpr-home-notice-title">🚀 Start Here</h3>
  <ul class="dpr-home-notice-list">
    <li><a href="#/tutorial/README">使用教程</a></li>
  </ul>
</div>

## 每次日报
- 最新运行日期：2026-08-25
- 运行时间：2026-08-25 20:27:04 UTC
- 运行状态：成功
- 本次总论文数：16
- 精读区：7
- 速读区：9

### 今日简报（AI）
今日共读16篇论文，精读7篇、速读9篇，重点聚焦注意力机制压缩与视觉Transformer高效化。最值得关注的两项高分工作：注意力在何种条件下可压缩，以及无需标注即可将ViT线性化用于目标检测。建议普通读者优先浏览这两个方向，把握高效模型设计的前沿趋势。
- 详情：[/202608/25/README](/202608/25/README)

### 精读区论文标签
1. [Beyond Sparse Weights: When Is Attention Compressible?](/202608/25/2608.21541v1-beyond-sparse-weights-when-is-attention-compressible)  
   标签：评分：9.0/10、query:la
   evidence：注意力可压缩性分析与免训练KV缓存压缩器，用于高效记忆检索
2. [DiD It in 87 Minutes: A Label-Free Softmax-to-Linear Adaptation of Vision Transformers for Object Detection](/202608/25/2608.22368v1-did-it-in-87-minutes-a-label-free-softmax-to-linear-adaptation-of-vision-transformers-for-object-detection)  
   标签：评分：9.0/10、query:la
   evidence：核心匹配：直接将ViT的Softmax注意力转为线性注意力，是线性注意力需求的核心工作。
3. [Sigmoid Attention as a Better Substrate for Learned KV Cache Eviction](/202608/25/2608.23296v1-sigmoid-attention-as-a-better-substrate-for-learned-kv-cache-eviction)  
   标签：评分：9.0/10、query:la
   evidence：sigmoid注意力作为学习式KV缓存淘汰的更好基底
4. [SSDi8: Accurate and Efficient 8-bit Quantization for State Space Duality](/202608/25/2608.21952v1-ssdi8-accurate-and-efficient-8-bit-quantization-for-state-space-duality)  
   标签：评分：8.0/10、query:la
   evidence：针对Mamba-2结构化状态空间对偶SSD这一现代RNN/线性注意力混合架构提出8比特量化框架
5. [Competitive Memory Readout for Robust Video Object Segmentation: 2nd Place Technical Report for the MOSEv2 Track of the 8th LSVOS Challenge](/202608/25/2608.22064v1-competitive-memory-readout-for-robust-video-object-segmentation-2nd-place-technical-report-for-the-mosev2-track-of-the-8th-lsvos-challenge)  
   标签：评分：8.0/10、query:la
   evidence：提出竞争性记忆读出机制，在注意力记忆检索中显式引入同类上下文，提升视频目标分割的鲁棒性
6. [MegaMem: A Retrieval Solution for Ultra-Large Context Windows](/202608/25/2608.22137v1-megamem-a-retrieval-solution-for-ultra-large-context-windows)  
   标签：评分：8.0/10、query:la
   evidence：超大上下文持久记忆检索，为大语言模型的记忆增强架构
7. [Parametric neural control differentiates top neural network models of primate visual cortex](/202608/25/biorxiv-10-64898-2026-08-16-745063-v1-parametric-neural-control-differentiates-top-neural-network-models-of-primate-visual-cortex)  
   标签：评分：8.0/10、query:comp-neuro
   evidence：视觉皮层计算编码模型与参数化神经控制，属核心计算神经科学

### 速读区论文标签
1. [ProxyFormer: A Dual-Stream Proxy Architecture for Ultra-Long Context and High-Resolution Generation](/202608/25/2608.23463v1-proxyformer-a-dual-stream-proxy-architecture-for-ultra-long-context-and-high-resolution-generation)  
   标签：评分：8.0/10、query:la
   evidence：双流代理架构通过压缩代理状态降低注意力二次复杂度，面向高效序列处理
2. [Dual-Layer Agentic Memory with Fast Write Routing and Slow Consolidation](/202608/25/2608.22215v1-dual-layer-agentic-memory-with-fast-write-routing-and-slow-consolidation)  
   标签：评分：7.0/10、query:la
   evidence：面向LLM智能体的双层层级记忆框架，通过写入路由和参数化整合管理知识生命周期，属于记忆增强网络方向
3. [WnW: Waxing-and-Waning KV Cache for Long-Form Speech LLMs](/202608/25/2608.22704v1-wnw-waxing-and-waning-kv-cache-for-long-form-speech-llms)  
   标签：评分：7.0/10、query:la
   evidence：面向长语音大语言模型的KV缓存高效管理
4. [Working memory impairments in Neurofibromatosis Type 1 are explained by disrupted functional connectivity and network controllability](/202608/25/biorxiv-10-1101-2025-04-10-648210-v4-working-memory-impairments-in-neurofibromatosis-type-1-are-explained-by-disrupted-functional-connectivity-and-network-controllability)  
   标签：评分：7.0/10、query:comp-neuro
   evidence：工作记忆损伤的功能连接与网络可控性分析
5. [The Retriever Should Remember: Experience-Amortized Reranking for Long-Term Agent Memory](/202608/25/2608.22767v1-the-retriever-should-remember-experience-amortized-reranking-for-long-term-agent-memory)  
   标签：评分：6.0/10、query:la
   evidence：将大模型相关性分数作为可复用检索经验存入外部记忆，与带注意力的记忆增强网络方向一致
6. [Distributed range adaptation in human parietal encoding of numbers](/202608/25/biorxiv-10-1101-2025-09-25-675916-v3-distributed-range-adaptation-in-human-parietal-encoding-of-numbers)  
   标签：评分：6.0/10、query:comp-neuro
   evidence：顶叶神经群体编码的自适应fMRI研究，与计算神经科学的表征计算相关。
7. [A unified multiscale modelling framework to explore the brain excitatory-inhibitory balance: application to multiple sclerosis](/202608/25/biorxiv-10-64898-2025-12-03-692031-v2-a-unified-multiscale-modelling-framework-to-explore-the-brain-excitatory-inhibitory-balance-application-to-multiple-sclerosis)  
   标签：评分：6.0/10、query:comp-neuro
   evidence：结合动态因果建模与虚拟大脑的统合多尺度脑建模范式，属于计算神经科学核心主题
8. [Spatially resolved mapping of tau amplification rates via differentiable simulation of prion-like propagation](/202608/25/biorxiv-10-64898-2026-06-02-729568-v2-spatially-resolved-mapping-of-tau-amplification-rates-via-differentiable-simulation-of-prion-like-propagation)  
   标签：评分：6.0/10、query:comp-neuro
   evidence：通过可微分模拟推断tau蛋白扩增速率的神经退行性研究
9. [Within-Subject Optogenetic Model Reveals Spatiotemporal Cortical Reorganization in Artificial Vision](/202608/25/biorxiv-10-64898-2026-08-19-745677-v1-within-subject-optogenetic-model-reveals-spatiotemporal-cortical-reorganization-in-artificial-vision)  
   标签：评分：6.0/10、query:comp-neuro
   evidence：光遗传模型结合CNN解码揭示人工视觉皮层表征重组


<div class="dpr-home-promo-card">
  <h3 class="dpr-home-promo-title">💬 社区与支持</h3>
  <ul class="dpr-home-promo-list">
    <li>欢迎 Star / Fork / Issue / PR</li>
    <li>QQ群：583867967（欢迎交流，已有：1151人）</li>
  </ul>
</div>
