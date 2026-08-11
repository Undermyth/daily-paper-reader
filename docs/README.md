<div class="dpr-home-notice-card">
  <h3 class="dpr-home-notice-title">🚀 Start Here</h3>
  <ul class="dpr-home-notice-list">
    <li><a href="#/tutorial/README">使用教程</a></li>
  </ul>
</div>

## 每次日报
- 最新运行日期：2026-08-11
- 运行时间：2026-08-11 20:18:52 UTC
- 运行状态：成功
- 本次总论文数：15
- 精读区：5
- 速读区：10

### 今日简报（AI）
今日精读5篇、速读10篇，共处理15篇论文，重点关注高效视觉Transformer与AI代理内存系统。最值得看的是《HSMLA》与《SuperLocalMemory 4.0》，均获9.0分高分，前者优化注意力效率，后者定义代理内存操作系统。建议下一步优先阅读这两篇全文，并留意低分速读中关于连续工作记忆与边缘动作识别的潜在方向。
- 详情：[/202608/11/README](/202608/11/README)

### 精读区论文标签
1. [HSMLA: Hierarchical Softmax Multi-scale Linear Attention for Efficient Vision Transformers](/202608/11/2608.07616v1-hsmla-hierarchical-softmax-multi-scale-linear-attention-for-efficient-vision-transformers)  
   标签：评分：9.0/10、query:la
   evidence：面向高效视觉Transformer的直接线性注意力方法
2. [SuperLocalMemory 4.0: The Governed Memory Operating System for AI Agents](/202608/11/2608.08253v1-superlocalmemory-40-the-governed-memory-operating-system-for-ai-agents)  
   标签：评分：9.0/10、query:la
   evidence：在AI代理的受治理记忆操作系统中集成Hopfield联想检索
3. [Linearized 2-Simplicial Attention](/202608/11/2608.09307v1-linearized-2-simplicial-attention)  
   标签：评分：9.0/10、query:la
   evidence：线性化注意力，固定大小状态与线性成本，无Softmax注意力
4. [MixFormer: Linear Transformer with Mixture of Memory Experts](/202608/11/2608.09468v1-mixformer-linear-transformer-with-mixture-of-memory-experts)  
   标签：评分：9.0/10、query:la
   evidence：混合记忆专家的线性Transformer及时间感知线性注意力
5. [AraSSM: A bidirectional state-space encoder for Arabic masked language modeling](/202608/11/2608.08256v1-arassm-a-bidirectional-state-space-encoder-for-arabic-masked-language-modeling)  
   标签：评分：8.0/10、query:la
   evidence：双向Mamba状态空间编码器以线性时间建模替代二次自注意力

### 速读区论文标签
1. [Divisive Normalization Shapes Low-Rank Slow Manifolds for Continuous Working Memory](/202608/11/2608.01947v1-divisive-normalization-shapes-low-rank-slow-manifolds-for-continuous-working-memory)  
   标签：评分：7.0/10、query:comp-neuro
   evidence：工作记忆的递归神经动力学计算建模
2. [CoDAT: Collaborative Dual-Attention Transformer with Low-Cost Temporal Modeling for Efficient Edge Action Recognition](/202608/11/2608.06691v1-codat-collaborative-dual-attention-transformer-with-low-cost-temporal-modeling-for-efficient-edge-action-recognition)  
   标签：评分：7.0/10、query:la
   evidence：面向边缘识别的轻量双分支注意力，属高效注意力机制
3. [CoinRAG: Contextualized Information Nugget KV Cache Reuse for Long-Context RAG](/202608/11/2608.07458v1-coinrag-contextualized-information-nugget-kv-cache-reuse-for-long-context-rag)  
   标签：评分：7.0/10、query:la
   evidence：面向长上下文 RAG 的细粒度 KV 缓存复用
4. [Keep It Simple: Multi-Key Episodic Memory Retrieval for Ultra-Long Video Understanding](/202608/11/2608.07663v1-keep-it-simple-multi-key-episodic-memory-retrieval-for-ultra-long-video-understanding)  
   标签：评分：7.0/10、query:la
   evidence：超长序列的多键情节记忆检索
5. [VLZip: Unified Visual and Textual Compression for Interleaved Long-Context Modeling](/202608/11/2608.08630v1-vlzip-unified-visual-and-textual-compression-for-interleaved-long-context-modeling)  
   标签：评分：7.0/10、query:la
   evidence：统一压缩以降低长序列二次注意力开销
6. [DistillCache: KL-Guided Adaptive KV-Cache Eviction for Memory-Efficient LLM Inference](/202608/11/2608.08878v1-distillcache-kl-guided-adaptive-kv-cache-eviction-for-memory-efficient-llm-inference)  
   标签：评分：7.0/10、query:la
   evidence：面向高效 LLM 推理的强化学习 KV 缓存驱逐
7. [Learning to Predict Middle-Layer Attention in MLLMs for Visual Token Prunin](/202608/11/2608.06411v1-learning-to-predict-middle-layer-attention-in-mllms-for-visual-token-prunin)  
   标签：评分：6.0/10、query:la
   evidence：通过预测中间层注意力来剪枝视觉token，提升多模态大模型的视觉序列处理效率，符合高效注意力主题
8. [OasisKV: Scaling In-Decode KV Cache Beyond HBM with Lookahead Sparse Prefetching](/202608/11/2608.08097v1-oasiskv-scaling-in-decode-kv-cache-beyond-hbm-with-lookahead-sparse-prefetching)  
   标签：评分：6.0/10、query:la
   evidence：面向注意力内存的高效KV缓存管理
9. [Don't Scroll Back: Missing-Evidence Memory for Streaming Dialogue Summarization](/202608/11/2608.09043v1-dont-scroll-back-missing-evidence-memory-for-streaming-dialogue-summarization)  
   标签：评分：6.0/10、query:la
   evidence：面向流式摘要的记忆框架，在固定预算下选择性检索无限历史，属于记忆增强型注意力方法
10. [Omni2LoRA: Coherence-Preserving Parametric Memory for Efficient Omni Language Models](/202608/11/2608.09227v1-omni2lora-coherence-preserving-parametric-memory-for-efficient-omni-language-models)  
   标签：评分：6.0/10、query:la
   evidence：通过LoRA压缩实现保相干的参数记忆


<div class="dpr-home-promo-card">
  <h3 class="dpr-home-promo-title">💬 社区与支持</h3>
  <ul class="dpr-home-promo-list">
    <li>欢迎 Star / Fork / Issue / PR</li>
    <li>QQ群：583867967（欢迎交流，已有：1151人）</li>
  </ul>
</div>
