<div class="dpr-home-notice-card">
  <h3 class="dpr-home-notice-title">🚀 Start Here</h3>
  <ul class="dpr-home-notice-list">
    <li><a href="#/tutorial/README">使用教程</a></li>
  </ul>
</div>

## 每次日报
- 最新运行日期：2026-08-17
- 运行时间：2026-08-17 19:35:50 UTC
- 运行状态：成功
- 本次总论文数：5
- 精读区：2
- 速读区：3

### 今日简报（AI）
今日精读5篇论文，聚焦线性注意力可遗忘机制与图序列模型跳点提取两大方向。最值得关注的是《The Query Knows What to Forget》提出第二擦除方向（9.0分），以及《HOPPER》的可学习跳点提取（8.0分）。建议优先研读这两篇，其余三篇涉及推理加速与KV缓存压缩，可作为补充。
- 详情：[/202608/17/README](/202608/17/README)

### 精读区论文标签
1. [The Query Knows What to Forget: A Second Erase Direction for Linear Attention](/202608/17/2608.13668v1-the-query-knows-what-to-forget-a-second-erase-direction-for-linear-attention)  
   标签：评分：9.0/10、query:la
   evidence：为线性注意力引入源自查询的第二擦除方向，减少干扰并提升检索性能
2. [HOPPER: Learnable Hop Extraction for Linearized Graph Sequence Models](/202608/17/2608.09031v1-hopper-learnable-hop-extraction-for-linearized-graph-sequence-models)  
   标签：评分：8.0/10、query:la
   evidence：为线性化图序列模型引入可学习的跳数提取，推进类线性注意力序列架构。

### 速读区论文标签
1. [Reduced Matrix Multiplication: Input-Adaptive Matrix-Product Reduction for LLM Inference](/202608/17/2608.13426v1-reduced-matrix-multiplication-input-adaptive-matrix-product-reduction-for-llm-inference)  
   标签：评分：7.0/10、query:la
   evidence：缩减Transformer矩阵乘法以高效推理，与线性注意力目标一致
2. [Prof-K: Probabilistic One-Pass Filtering for Efficient Top-k Selection](/202608/17/2608.12573v1-prof-k-probabilistic-one-pass-filtering-for-efficient-top-k-selection)  
   标签：评分：6.0/10、query:la
   evidence：高效top-k过滤，可用于注意力剪枝
3. [KV Cache Compression Through the Lens of Transform Coding](/202608/17/2608.14191v1-kv-cache-compression-through-the-lens-of-transform-coding)  
   标签：评分：6.0/10、query:la
   evidence：面向内存高效Transformer推理的注意力感知KV缓存压缩


<div class="dpr-home-promo-card">
  <h3 class="dpr-home-promo-title">💬 社区与支持</h3>
  <ul class="dpr-home-promo-list">
    <li>欢迎 Star / Fork / Issue / PR</li>
    <li>QQ群：583867967（欢迎交流，已有：1151人）</li>
  </ul>
</div>
