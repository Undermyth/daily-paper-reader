<div class="dpr-home-notice-card">
  <h3 class="dpr-home-notice-title">🚀 Start Here</h3>
  <ul class="dpr-home-notice-list">
    <li><a href="#/tutorial/README">使用教程</a></li>
  </ul>
</div>

## 每次日报
- 最新运行日期：2026-07-31
- 运行时间：2026-07-31 21:51:22 UTC
- 运行状态：成功
- 本次总论文数：11
- 精读区：6
- 速读区：5

### 今日简报（AI）
今日共处理11篇论文，精读6篇、速读5篇，核心关注视觉扩散模型与KV缓存优化。  
最值得精读的是9.0分的《Chimera》——探索混合视觉扩散Transformer的Chinchilla缩放；其次是8.0分的投机解码中的功能重建方法。  
建议普通读者优先阅读这两篇高分论文，并可快速浏览KV缓存相关的三篇速读文章以了解最新优化思路。
- 详情：[/202607/31/README](/202607/31/README)

### 精读区论文标签
1. [Chimera: Designing and Chinchilla-Scaling Hybrid Visual Diffusion Transformers](/202607/31/2607.28611v1-chimera-designing-and-chinchilla-scaling-hybrid-visual-diffusion-transformers)  
   标签：评分：9.0/10、query:la
   evidence：结合线性注意力与交错MLA的混合视觉扩散Transformer，实现O(N)长上下文状态追踪
2. [Beyond KV Reconstruction: Functional Reconstruction for MLA Draft Models in Speculative Decoding](/202607/31/2607.27269v1-beyond-kv-reconstruction-functional-reconstruction-for-mla-draft-models-in-speculative-decoding)  
   标签：评分：8.0/10、query:la
   evidence：通过潜在状态压缩与投机解码提升注意力效率
3. [Recall Before You Rank: Similarity-Guided Top-$K$ Reuse for Efficient Long-Context Attention](/202607/31/2607.27692v1-recall-before-you-rank-similarity-guided-top-k-reuse-for-efficient-long-context-attention)  
   标签：评分：8.0/10、query:la
   evidence：通过检索复用与Top-K稀疏注意力提升长上下文序列处理效率
4. [S-CEReBrO: Breaking the Memory Barrier in Continuous EEG Monitoring](/202607/31/2607.27913v1-s-cerebro-breaking-the-memory-barrier-in-continuous-eeg-monitoring)  
   标签：评分：8.0/10、query:la
   evidence：窗口交替注意力机制将KV缓存大小与信号时长解耦，实现持续监测的常量内存
5. [Memory Decoder at Scale: A Pretrained, Parametric Long-Term Memory](/202607/31/2607.27919v1-memory-decoder-at-scale-a-pretrained-parametric-long-term-memory)  
   标签：评分：8.0/10、query:la
   evidence：大规模预训练参数化长期记忆模块，通过索引与检索增强解码器语言模型
6. [Understanding Is Done Early: A Depth Division of Labor in Large Language Models and Its Use for Unbounded-Context Memory](/202607/31/2607.28263v1-understanding-is-done-early-a-depth-division-of-labor-in-large-language-models-and-its-use-for-unbounded-context-memory)  
   标签：评分：8.0/10、query:la
   evidence：利用深度分工实现上下文长度无关的Transformer记忆

### 速读区论文标签
1. [HiKV: Hierarchical Importance-Aware KV Cache with Hardware Acceleration for LLM Decoding](/202607/31/2607.22389v1-hikv-hierarchical-importance-aware-kv-cache-with-hardware-acceleration-for-llm-decoding)  
   标签：评分：7.0/10、query:la
   evidence：层次化重要性的KV缓存压缩，用于大语言模型解码中的高效记忆检索
2. [SemPIC: Learning Semantic Position-Independent KV Caches](/202607/31/2607.28069v1-sempic-learning-semantic-position-independent-kv-caches)  
   标签：评分：7.0/10、query:la
   evidence：学习位置无关的KV缓存以提升注意力记忆复用
3. [ReToken: One Token to Improve Vision-Language Models for Visual Retrieval](/202607/31/2607.28627v1-retoken-one-token-to-improve-vision-language-models-for-visual-retrieval)  
   标签：评分：7.0/10、query:la
   evidence：用检索目标token从KV缓存中选择相关视觉token，提升检索同时降低注意力缓存开销
4. [Gradient-free Task-Conditioned Retrieval for On-Device In-Context Learning](/202607/31/2607.27766v1-gradient-free-task-conditioned-retrieval-for-on-device-in-context-learning)  
   标签：评分：6.0/10、query:la
   evidence：针对端侧上下文学习从本地记忆进行任务条件检索
5. [RRM: Experience-Driven Reflective Retrieval Memory for Long-Horizon Multimodal Reasoning](/202607/31/2607.28156v1-rrm-experience-driven-reflective-retrieval-memory-for-long-horizon-multimodal-reasoning)  
   标签：评分：6.0/10、query:la
   evidence：面向多模态长时程推理的反思式检索记忆框架，结合图记忆与经验记忆


<div class="dpr-home-promo-card">
  <h3 class="dpr-home-promo-title">💬 社区与支持</h3>
  <ul class="dpr-home-promo-list">
    <li>欢迎 Star / Fork / Issue / PR</li>
    <li>QQ群：583867967（欢迎交流，已有：1151人）</li>
  </ul>
</div>
