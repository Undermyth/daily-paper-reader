<div class="dpr-home-notice-card">
  <h3 class="dpr-home-notice-title">🚀 Start Here</h3>
  <ul class="dpr-home-notice-list">
    <li><a href="#/tutorial/README">使用教程</a></li>
  </ul>
</div>

## 每次日报
- 最新运行日期：2026-08-05
- 运行时间：2026-08-05 21:20:09 UTC
- 运行状态：成功
- 本次总论文数：15
- 精读区：7
- 速读区：8

### 今日简报（AI）
今日精读2篇高分论文，聚焦长上下文记忆与KV检索，另速读5篇涉及推理效率、3.6M超长上下文推理及状态空间模型。  
最值得关注的是长上下文高效记忆机制：Maglev的滑动循环记忆与SAKI的低秩键索引，均获9.0分，前者优化计算效率，后者提升KV检索性能。  
建议读者优先精读这两篇，并关注PI-Mem的并行迭代记忆方案，以理解当前超长上下文推理的前沿趋势。
- 详情：[/202608/05/README](/202608/05/README)

### 精读区论文标签
1. [Maglev: Sliding Recurrent Memory](/202608/05/2608.02870v1-maglev-sliding-recurrent-memory)  
   标签：评分：9.0/10、query:la
   evidence：带固定滑动循环记忆的循环Transformer，贴合现代RNN与线性注意力
2. [SAKI: Score-Aware Low-Rank Key Indexing for Long-Context KV Retrieval](/202608/05/2608.03228v1-saki-score-aware-low-rank-key-indexing-for-long-context-kv-retrieval)  
   标签：评分：9.0/10、query:la
   evidence：分数感知的低秩键索引直接保留注意力分数，用于长上下文KV检索
3. [Opt.Gear Technical Report](/202608/05/2608.01034v1-optgear-technical-report)  
   标签：评分：8.0/10、query:la
   evidence：卷积门控混合器与局部-全局注意力结合，降低KV缓存开销，提升长上下文推理效率
4. [CoEvo-Mem: Co-Evolving Retrieval Policy and Memory Bank for LLM Agents](/202608/05/2608.01739v1-coevo-mem-co-evolving-retrieval-policy-and-memory-bank-for-llm-agents)  
   标签：评分：8.0/10、query:la
   evidence：为LLM智能体协同演化检索策略与记忆库，属于带注意力的记忆增强网络。
5. [Divisive Normalization Shapes Low-Rank Slow Manifolds for Continuous Working Memory](/202608/05/2608.01947v1-divisive-normalization-shapes-low-rank-slow-manifolds-for-continuous-working-memory)  
   标签：评分：8.0/10、query:comp-neuro
   evidence：将皮层广泛存在的除法归一化计算应用于连续工作记忆的动力学建模
6. [Messages, Not Tokens: Grounded Coresets for Faithful VLM Compression](/202608/05/2608.02134v1-messages-not-tokens-grounded-coresets-for-faithful-vlm-compression)  
   标签：评分：8.0/10、query:la
   evidence：基于核心集的视觉token压缩以实现忠实KV缓存缩减
7. [Designing a Good Virtual Node: Addressable and Cardinality-Preserving Global Memory for Message Passing Architectures](/202608/05/2608.02709v1-designing-a-good-virtual-node-addressable-and-cardinality-preserving-global-memory-for-message-passing-architectures)  
   标签：评分：8.0/10、query:la
   evidence：使用可寻址交叉注意力记忆槽替代自注意力，提供保基数的全局通信

### 速读区论文标签
1. [ATFlash: Per-RoPE-Wavelength Attention Windows for Compute/Memory-Efficient LLM Inference](/202608/05/2608.02947v1-atflash-per-rope-wavelength-attention-windows-for-computememory-efficient-llm-inference)  
   标签：评分：8.0/10、query:la
   evidence：基于RoPE波长的注意力窗口降低大模型推理的计算与内存
2. [PI-Mem: Pushing Long-Context Reasoning to 3.6M Tokens with Parallel-Iterative Memory](/202608/05/2608.03048v1-pi-mem-pushing-long-context-reasoning-to-36m-tokens-with-parallel-iterative-memory)  
   标签：评分：8.0/10、query:la
   evidence：并行迭代记忆机制增强长上下文推理，属于记忆增强神经网络方法
3. [State Propagation Also Satisfies: A Complex-Valued State-Space Model for Deterministic State Tracking](/202608/05/2608.03425v1-state-propagation-also-satisfies-a-complex-valued-state-space-model-for-deterministic-state-tracking)  
   标签：评分：8.0/10、query:la
   evidence：用于确定性状态跟踪的复值状态空间循环模型，无需注意力
4. [SMM Transformer: Leveraging Spiking Neural Networks for Multimodal Tasks](/202608/05/2608.01622v1-smm-transformer-leveraging-spiking-neural-networks-for-multimodal-tasks)  
   标签：评分：7.0/10、query:la
   evidence：脉冲驱动的token混合替代稠密softmax注意力
5. [SPADE: An Input-Adaptive Sparse Attention Engine for Fast Video Diffusion Models Inference](/202608/05/2608.03335v1-spade-an-input-adaptive-sparse-attention-engine-for-fast-video-diffusion-models-inference)  
   标签：评分：7.0/10、query:la
   evidence：用于快速推理的输入自适应稀疏注意力引擎
6. [Gram-Space: Structure-Preserving Codebook Compression for Memory-Efficient Neuro-Symbolic AI](/202608/05/2608.01528v1-gram-space-structure-preserving-codebook-compression-for-memory-efficient-neuro-symbolic-ai)  
   标签：评分：6.0/10、query:la
   evidence：向量符号架构即联想记忆，并保持注意力分数计算
7. [Token Radius Attention for Efficient Video Generation](/202608/05/2608.02504v1-token-radius-attention-for-efficient-video-generation)  
   标签：评分：6.0/10、query:la
   evidence：面向高效视频生成的查询自适应令牌半径注意力；属于高效注意力但与记忆检索关联较弱
8. [Heterogeneous LLM Serving with General-Purpose Processing-Near-Memory for Retrieval-Based Sparse Attention](/202608/05/2608.03555v1-heterogeneous-llm-serving-with-general-purpose-processing-near-memory-for-retrieval-based-sparse-attention)  
   标签：评分：6.0/10、query:la
   evidence：基于检索的稀疏注意力与KV缓存的存内处理加速器


<div class="dpr-home-promo-card">
  <h3 class="dpr-home-promo-title">💬 社区与支持</h3>
  <ul class="dpr-home-promo-list">
    <li>欢迎 Star / Fork / Issue / PR</li>
    <li>QQ群：583867967（欢迎交流，已有：1151人）</li>
  </ul>
</div>
