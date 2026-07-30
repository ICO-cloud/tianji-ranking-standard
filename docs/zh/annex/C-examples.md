> **ICO Std 2002:2026 — 中文版 — 附录C 实施案例**

## 附录C 实施案例
## 目的
本附录提供ICO Std 2002在不同排名领域的说明性实施示例。每个示例通过完整的排名生命周期——从指标设计和权重分配到数据采集、评分和发布——展示标准的实际应用。这些示例
> 免责声明
## C.1 示例1：非物质文化遗产排名实施框架
### C.1.1 场景描述
某排名实体拟开发特定国家内非物质文化遗产（ICH）要素的排名，评估其保护状况、社区活力和传承有效性。该排名旨在为政策制定者、文化组织和公众提供有关ICH保护状况的信息，与联合国教科文组织《保护非物质文化遗产公约》（2003年）一致。
适用标准条款
### C.1.2 流程示意图
### C.1.3 指标体系
#### 一级指标（维度）
| ID | Dimension | Weight | Description |
|----|-----------|--------|-------------|
| D1 | 保护状况 | 0.30 | Measures the formal recognition and institutional support for the ICH element |
| D2 | 社区活力 | 0.30 | Measures the active engagement of the bearer community in sustaining the ICH element |
| D3 | 传承有效性 | 0.25 | Measures the effectiveness of inter-generational transmission |
| D4 | 公众认知与影响力 | 0.15 | Measures the broader public awareness and cultural influence of the ICH element |
#### 二级指标（子维度）
| ID | Sub-dimension | Parent | Weight (within parent) | Description |
|----|--------------|--------|----------------------|-------------|
| D1.1 | 注册状态 | D1 | 0.35 | Whether the element is inscribed on national/international ICH lists |
| D1.2 | 保护计划 | D1 | 0.35 | Existence and quality of safeguarding plans |
| D1.3 | 资金支持 | D1 | 0.30 | Level of financial support for safeguarding activities |
| D2.1 | 从业者数量 | D2 | 0.30 | Number of active practitioners/transmitters |
| D2.2 | 社区参与 | D2 | 0.35 | Level of community participation in ICH practices |
| D2.3 | 实践连续性 | D2 | 0.35 | Continuity of practice over time (no significant interruptions) |
| D3.1 | 学徒制 | D3 | 0.35 | Existence and functioning of formal/informal apprenticeship systems |
| D3.2 | 青年参与 | D3 | 0.35 | Proportion of practitioners under 35 years of age |
| D3.3 | 知识记录 | D3 | 0.30 | Completeness of documentation of ICH knowledge and techniques |
| D4.1 | 媒体报道 | D4 | 0.35 | Volume and quality of media coverage |
| D4.2 | 教育整合 | D4 | 0.35 | Integration into formal and informal education |
| D4.3 | 文化旅游影响 | D4 | 0.30 | Contribution to cultural tourism (as a measure of public interest) |
#### 三级指标（具体度量）— 选取示例
| ID | Measure | Parent | Data Source Tier | Measurement Method |
|----|---------|--------|-----------------|-------------------|
| D1.1.1 | National ICH list inscription | D1.1 | Tier 1 | Binary (1 = inscribed, 0 = not) + tier of inscription (national/international) |
| D1.1.2 | UNESCO ICH list inscription | D1.1 | Tier 1 | Binary (1 = inscribed, 0 = not) |
| D1.2.1 | Safeguarding plan existence | D1.2 | Tier 1 | Binary (1 = exists, 0 = not) |
| D1.2.2 | Safeguarding plan quality score | D1.2 | Tier 2 | Expert assessment on 1–5 scale (rubric-based) |
| D2.1.1 | Number of active practitioners | D2.1 | Tier 1 | Count from official registry or survey |
| D2.2.1 | Community participation rate | D2.2 | Tier 2 | Survey-based estimate (% of community members participating) |
| D3.2.1 | Proportion of practitioners under 35 | D3.2 | Tier 1 | Demographic data from registry/survey |
| D4.1.1 | Annual media mentions | D4.1 | Tier 3 | Count from media database search |
### C.1.4 权重分配
权重通过分析层次过程（AHP）确定，由12名ICH专家组成的小组进行（§06.1.2——专家组法）。AHP过程包括：
   每位专家对一级维度进行两两比较；
   使用几何平均聚合个体判断；
   从聚合比较矩阵计算优先权重；
一致性检验（所有专家的一致性比率CR
一级权重结果
对于定性指标（1–5量表专家评估），得分归一化至[0, 1]区间：
说明性评分结果
| Rank | ICH Element | D1 (0.30) | D2 (0.30) | D3 (0.25) | D4 (0.15) | Composite Score |
|------|-------------|-----------|-----------|-----------|-----------|----------------|
| 1 | Traditional Silk Weaving | 0.89 | 0.85 | 0.82 | 0.78 | 0.846 |
| 2 | Dragon Boat Festival | 0.92 | 0.78 | 0.76 | 0.85 | 0.828 |
| 3 | Ceramic Firing Technique | 0.75 | 0.82 | 0.71 | 0.62 | 0.746 |
| 4 | Folk Music Tradition | 0.68 | 0.65 | 0.72 | 0.58 | 0.662 |
| 5 | Traditional Paper-cutting | 0.71 | 0.55 | 0.48 | 0.65 | 0.588 |
稳健性检验
进行了自助重抽样（1000次迭代）。结果：
### C.1.7 发布与审计
排名以**三级透明度**（数据透明，§9.2.3）发布，包括：
   完整方法论文件；
   所有一级和二级指标得分；
   包含三级指标得分的可下载数据文件；
   稳健性分析结果；
   局限性披露（§9.1.4），包括排名衡量保护状况且不应作为资金分配唯一依据的注意事项。
## C.2 示例2：消费品品质排名实施框架
### C.2.1 场景描述
某排名实体拟开发特定消费品类别（如智能手机）的品质排名。该排名基于客观质量度量、用户体验和性价比评估产品。该排名必须应对消费品排名中普遍存在的数据操纵（如虚假评论、刷单）风险。
适用标准条款
### C.2.2 流程示意图
### C.2.3 指标体系
#### 一级指标
| ID | Dimension | Weight | Description |
|----|-----------|--------|-------------|
| P1 | 产品性能 | 0.35 | Objective technical performance measures |
| P2 | 用户体验 | 0.30 | Subjective and objective user experience measures |
| P3 | 性价比 | 0.20 | Quality relative to price |
| P4 | 品牌可靠性 | 0.15 | Brand reputation, after-sales service, warranty |
#### 二级指标——品类特定（智能手机）
| ID | Sub-dimension | Parent | Weight (within parent) | Measurement |
|----|--------------|--------|----------------------|-------------|
| P1.1 | Processor performance | P1 | 0.25 | Benchmark score (Tier 1: lab test) |
| P1.2 | Display quality | P1 | 0.20 | Colour accuracy, brightness, resolution (Tier 1) |
| P1.3 | Camera quality | P1 | 0.25 | DxOMark or equivalent score (Tier 1) |
| P1.4 | Battery life | P1 | 0.20 | Standardised battery test (Tier 1) |
| P1.5 | Build quality | P1 | 0.10 | Durability test score (Tier 1) |
| P2.1 | User satisfaction score | P2 | 0.40 | Verified user survey (Tier 2) |
| P2.2 | Ease of use | P2 | 0.30 | Expert assessment (Tier 2) |
| P2.3 | Software experience | P2 | 0.30 | Expert assessment (Tier 2) |
| P3.1 | Performance-to-price ratio | P3 | 0.60 | Composite score / retail price (Tier 1) |
| P3.2 | Feature completeness | P3 | 0.40 | Feature count vs. category average (Tier 1) |
| P4.1 | Brand reputation index | P4 | 0.40 | Brand evaluation score (Tier 2) |
| P4.2 | After-sales service quality | P4 | 0.35 | Customer service satisfaction survey (Tier 2) |
| P4.3 | Warranty coverage | P4 | 0.25 | Warranty terms and coverage (Tier 1) |
### C.2.4 反刷单机制
消费品排名特别容易受到数据操纵。按照§7.5的规定，适用以下反欺诈措施：
三级数据欺诈检测
对于电商评论数据（三级），适用以下检测算法：
重复检测
文本相同或近于相同的评论被标记并排除。检测阈值：Jaccard相似度
时间聚集检测
   评论量异常激增（如日均率的3个标准差以上）被标记以供人工审查。
账户年龄和活动过滤
   注册不足30天或先前评论不足3条的账户的评论被排除在评分计算之外。
反刷单惩罚
如果发现某产品具有统计上显著比例的虚假评论（由上述欺诈检测算法确定），则适用以下惩罚：
### C.2.5 评分与排名
归一化
应用z-分数标准化：
说明性评分结果
| Rank | Product | P1 (0.35) | P2 (0.30) | P3 (0.20) | P4 (0.15) | Composite | Fraud Penalty Applied |
|------|---------|-----------|-----------|-----------|-----------|-----------|----------------------|
| 1 | Phone Alpha | 0.92 | 0.88 | 0.75 | 0.82 | 0.863 | No |
| 2 | Phone Beta | 0.88 | 0.82 | 0.85 | 0.78 | 0.838 | No |
| 3 | Phone Gamma | 0.85 | 0.595 | 0.72 | 0.75 | 0.718 | Yes (P2.1 adjusted) |
| 4 | Phone Delta | 0.72 | 0.75 | 0.68 | 0.70 | 0.716 | No |
| 5 | Phone Epsilon | 0.68 | 0.70 | 0.62 | 0.65 | 0.667 | No |
### C.2.6 敏感性分析
按照§8.5.3的规定，进行了以下敏感性分析：
权重变异测试
所有一级权重变化±5个百分点。最大排名变化为1位，表明排名对中等权重变异具有稳健性。
方法变异测试
使用几何平均聚合方法重新计算排名。WAM和几何平均排名之间的Spearman ρ为0.94，表明高度一致。
数据扰动测试
向输入数据添加随机噪声（每个指标标准差的±5%）。排名重新计算100次。平均排名稳定性（排名不变的实体比例）为88%。
## C.3 示例3：跨领域综合排名实施框架
### C.3.1 场景描述
某排名实体拟开发跨领域综合排名，从不同领域评估实体的多个维度（如结合经济、环境、文化和基础设施指标的"城市宜居指数"）。主要挑战在于不同领域、不同测量尺度和单位的指标的有意义聚合。
适用标准条款
### C.3.2 流程示意图
### C.3.3 指标体系
#### 一级指标（领域）
| ID | Domain | Weight | Source Module | Description |
|----|--------|--------|--------------|-------------|
| L1 | 经济活力 | 0.25 | SE-04 | Economic output, employment, innovation |
| L2 | 环境质量 | 0.25 | SE-08 | Air quality, green space, GHG emissions |
| L3 | 文化丰富度 | 0.20 | SE-05 | Cultural heritage, creative industries, cultural participation |
| L4 | 基础设施与服务 | 0.30 | SE-04 | Transportation, healthcare, education, housing |
#### 二级和三级指标——选取示例
| ID | Sub-dimension / Measure | Parent | Data Source | Normalisation |
|----|------------------------|--------|------------|---------------|
| L1.1 | GDP per capita | L1 | Tier 1 (National statistics) | Percentile ranking |
| L1.2 | Employment rate | L1 | Tier 1 (Labour statistics) | Percentile ranking |
| L1.3 | Innovation index | L1 | Tier 2 (Composite index) | Percentile ranking |
| L2.1 | Air quality index (AQI) | L2 | Tier 1 (Environmental monitoring) | Inverse percentile (lower AQI = better) |
| L2.2 | Green space per capita | L2 | Tier 1 (Urban planning data) | Percentile ranking |
| L2.3 | GHG emissions per capita | L2 | Tier 1 (ISO 14064 compliant) | Inverse percentile |
| L3.1 | Cultural heritage density | L3 | Tier 1 (Heritage registry) | Percentile ranking |
| L3.2 | Creative industry employment | L3 | Tier 1 (Labour statistics) | Percentile ranking |
| L3.3 | Cultural participation rate | L3 | Tier 2 (Resident survey) | Percentile ranking |
| L4.1 | Public transport coverage | L4 | Tier 1 (Transport authority) | Percentile ranking |
| L4.2 | Healthcare access index | L4 | Tier 2 (Survey + official data) | Percentile ranking |
| L4.3 | Education quality index | L4 | Tier 2 (Survey + official data) | Percentile ranking |
| L4.4 | Housing affordability | L4 | Tier 1 (Real estate data) | Percentile ranking |
### C.3.4 跨领域归一化
不同领域的指标具有不同的测量尺度（如GDP以货币单位计、AQI以指数单位计、就业率以百分比计）。直接比较需要共同的归一化方法。
选择百分位排名归一化（§8.2），因为其对异常值具有稳健性，且能跨不同尺度产生可比得分：
### C.3.5 权重分配
权重通过利益相关方咨询和专家组法的组合确定（§06.1）：
   领域间权重（一级）：通过与200名居民、30名政策制定者和20名投资者的利益相关方咨询确定。最终权重经校准以反映目标受众的共识优先级。
领域内权重（二级和三级）：通过由8名领域专家（每领域2名）组成的AHP确定。
### C.3.6 敏感性分析
跨领域排名对领域权重选择特别敏感。进行了以下多维敏感性分析：
逐项权重变异
每个一级权重独立变化±5和±10个百分点，其余权重按比例调整。任何实体的最大排名变化为：
| Weight Variation | Max Rank Change | Entities with ≥2 Position Change |
|-----------------|-----------------|----------------------------------|
| ±5 pp | 2 positions | 3 of 50 cities |
| ±10 pp | 4 positions | 8 of 50 cities |
多维权重敏感性
使用10
| Statistic | Description |
|-----------|-------------|
| Mean rank | Average rank across all weight combinations |
| Rank standard deviation | Variability of rank across weight combinations |
| 90% rank interval | 5th to 95th percentile of rank distribution |
| Rank stability index | Proportion of weight combinations where rank is within ±3 of published rank |
说明性结果
| City | Published Rank | Mean Rank | Rank SD | 90% Interval | Stability Index |
|------|---------------|-----------|---------|--------------|----------------|
| City A | 1 | 1.2 | 0.5 | [1, 2] | 98% |
| City B | 2 | 2.8 | 1.1 | [1, 5] | 72% |
| City C | 3 | 3.5 | 1.8 | [1, 7] | 55% |
| City D | 4 | 4.2 | 1.5 | [2, 8] | 48% |
| City E | 5 | 4.8 | 1.2 | [2, 7] | 62% |
领域排除测试
依次排除每个领域重新计算排名。此测试识别哪些领域对排名影响最大：
| Excluded Domain | Mean Rank Change | Max Rank Change |
|----------------|-----------------|-----------------|
| L1 (Economic) | 2.8 positions | 8 positions |
| L2 (Environmental) | 2.2 positions | 6 positions |
| L3 (Cultural) | 1.5 positions | 5 positions |
| L4 (Infrastructure) | 3.2 positions | 10 positions |
结果表明基础设施与服务（L4）对排名影响最大，这与其最高权重（0.30）一致。此发现记录在方法论声明中。
### C.3.7 交互式排名工具
按照§06.4（用户可调权重），提供了交互式排名工具，允许用户：
   使用滑块控制调整一级领域权重；
   基于调整后的权重实时重新计算排名；
   将用户调整排名与默认排名实体排名进行比较；
   查看每个实体的敏感性分析结果。
该工具显著展示默认（排名实体）权重与任何用户调整结果，并明确说明用户调整排名非官方排名。
### C.3.8 发布
排名以**四级透明度**（完全可复现，§9.2.4）发布，包括：
   完整方法论文件；
   每个层级所有指标得分；
完整数据集（以CSV格式下载）；
分析代码（用于评分、聚合和敏感性分析的Python脚本）；
   全面的敏感性分析报告；
   含用户可调权重的交互式排名工具；
   局限性披露（§9.1.4），包括排名衡量相对宜居性且不应作为搬迁或投资决策唯一依据的注意事项。
## C.4 跨示例比较
| Aspect | Example 1 (ICH) | Example 2 (Consumer Products) | Example 3 (Cross-Domain) |
|--------|-----------------|------------------------------|--------------------------|
| Domain | Cultural Heritage | Consumer Products | City Livability |
| Extension Module | SE-05 | SE-01 | SE-04 + SE-05 + SE-08 |
| Primary Challenge | Valuing intangible attributes | Anti-fraud / anti-brushing | Cross-domain aggregation |
| Normalisation | Min-max | Z-score + percentile | Percentile ranking |
| Aggregation | WAM | WAM + anti-fraud penalty | WAM |
| Weighting Method | AHP (expert panel) | AHP (expert panel) | Stakeholder consultation + AHP |
| Key Risk | Cultural bias in expert assessment | Data manipulation by ranked entities | Weight sensitivity across domains |
| Transparency Level | Level 3 | Level 2 | Level 4 |
| Anti-Fraud | Not applicable | Tier 3 fraud detection + penalty | Not applicable |
| Sensitivity Analysis | Bootstrap + method variation | Weight variation + method variation + data perturbation | OAT + Monte Carlo + domain exclusion |
| Key Robustness Result | Spearman's ρ = 0.96 (WAM vs. geometric) | Max rank change = 1 position (±5pp weight) | Mean stability index = 67% across entities |
## C.5 关键实施要点
### C.5.1 指标设计
   指标选择必须由排名目的驱动（§05.1），而非数据可用性。在示例1中，指标体系包含需要二级数据采集的定性度量（如保护计划质量），尽管仅使用一级数据会更容易采集。
   领域特定指标应由领域专家验证（§05.1）。在所有三个示例中，领域专家参与了指标选择过程。
### C.5.2 权重分配
权重方法的选择应予以记录和论证（§06.1）。当专家判断可用时，AHP是合适的；当排名目标受众具有多元视角时，利益相关方咨询是适当的。
   权重敏感性分析（§8.5.3）对于不同领域相对重要性可能因利益相关方而异的跨领域排名至关重要。
### C.5.3 数据质量与反欺诈
   三级数据源分类（§7.1）为管理不同来源类型的数据质量提供了实用框架。
   反欺诈机制（§7.5）对于数据操纵为已知风险的消费品排名至关重要。反刷单惩罚机制提供了与检测到的欺诈成比例的威慑。
### C.5.4 透明度与可复现性
   四级透明度体系（§9.2）为逐步改进排名发布透明度提供了实用框架。排名实体应在考虑数据敏感性和目标受众需求的前提下，追求可实现的最高透明度等级。
   用户可调权重（§06.4）对于不同利益相关方可能具有不同优先级的跨领域排名特别有价值。交互式排名工具提供了超越柏林原则消费者选择建议的利益相关方参与机制。
