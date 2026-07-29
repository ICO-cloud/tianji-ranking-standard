# Annex C: Application Examples
## 附录C 实施案例

**ICO Std 2002 — Annex C (Informative)**

---

## Purpose | 目的

This annex provides illustrative examples of applying ICO Std 2002 across different ranking domains. Each example demonstrates the standard's practical application by walking through the complete ranking lifecycle — from indicator design and weighting to data collection, scoring, and publication. These examples are **illustrative only** and do not represent actual ranking results.

本附录提供ICO Std 2002在不同排名领域的说明性实施示例。每个示例通过完整的排名生命周期——从指标设计和权重分配到数据采集、评分和发布——展示标准的实际应用。这些示例**仅供说明之用**，不代表实际排名结果。

> **Disclaimer**: The indicator systems, weights, data, and scores used in these examples are hypothetical and are provided solely for the purpose of illustrating the application of ICO Std 2002. They should not be interpreted as actual rankings or evaluations of any real entity, product, or heritage item.
>
> **免责声明**：本示例中使用的指标体系、权重、数据和得分均为假设性数据，仅用于说明ICO Std 2002的应用。不应将其解读为对任何真实实体、产品或遗产项目的实际排名或评价。

---

## C.1 Example 1: Intangible Cultural Heritage (ICH) Ranking | 示例1：非物质文化遗产排名实施框架

### C.1.1 Scenario Description | 场景描述

A ranking entity wishes to develop a ranking of intangible cultural heritage (ICH) elements within a specific country, evaluating their safeguarding status, community vitality, and transmission effectiveness. The ranking is intended to inform policy-makers, cultural organisations, and the public about the state of ICH safeguarding, consistent with the UNESCO Convention for the Safeguarding of the Intangible Cultural Heritage (2003).

某排名实体拟开发特定国家内非物质文化遗产（ICH）要素的排名，评估其保护状况、社区活力和传承有效性。该排名旨在为政策制定者、文化组织和公众提供有关ICH保护状况的信息，与联合国教科文组织《保护非物质文化遗产公约》（2003年）一致。

**Applicable standard provisions** | **适用标准条款**: ICO Std 2002 core layer (§04–§11) and SE-05 (Cultural Heritage) extension module.

### C.1.2 Process Flow Diagram | 流程示意图

```
┌─────────────────────────────────────────────────────────────────┐
│  STEP 1: Purpose & Scope Definition (§04, §01)                  │
│  目的与范围界定                                                   │
│  - Define: ICH safeguarding assessment                          │
│  - Target: Policy-makers, cultural organisations, public       │
│  - Domain: SE-05 (Cultural Heritage)                            │
└───────────────────────────┬─────────────────────────────────────┘
                            ▼
┌─────────────────────────────────────────────────────────────────┐
│  STEP 2: Indicator System Design (§05)                           │
│  指标体系设计                                                     │
│  - Level 1: 4 dimensions                                        │
│  - Level 2: 12 sub-dimensions                                   │
│  - Level 3: 36 specific measures                                │
└───────────────────────────┬─────────────────────────────────────┘
                            ▼
┌─────────────────────────────────────────────────────────────────┐
│  STEP 3: Weight Assignment (§06)                                 │
│  权重分配                                                        │
│  - AHP-based expert weighting                                    │
│  - Sensitivity analysis of weight variations                    │
└───────────────────────────┬─────────────────────────────────────┘
                            ▼
┌─────────────────────────────────────────────────────────────────┐
│  STEP 4: Data Collection (§07)                                   │
│  数据采集                                                        │
│  - Tier 1: Official ICH registries, government statistics       │
│  - Tier 2: Expert surveys, community interviews                 │
│  - Tier 3: Publicly available media reports                     │
└───────────────────────────┬─────────────────────────────────────┘
                            ▼
┌─────────────────────────────────────────────────────────────────┐
│  STEP 5: Scoring & Ranking (§08)                                 │
│  评分与排名                                                      │
│  - Normalisation: Min-max method                                │
│  - Aggregation: Weighted arithmetic mean (WAM)                  │
│  - Robustness: Bootstrap resampling (1000 iterations)           │
└───────────────────────────┬─────────────────────────────────────┘
                            ▼
┌─────────────────────────────────────────────────────────────────┐
│  STEP 6: Publication & Audit (§09, §10)                          │
│  发布与审计                                                      │
│  - Transparency Level 3 (Data Transparency)                     │
│  - Internal audit + external peer review                        │
└─────────────────────────────────────────────────────────────────┘
```

### C.1.3 Indicator System | 指标体系

#### Level 1 Indicators (Dimensions) | 一级指标（维度）

| ID | Dimension | Weight | Description |
|----|-----------|--------|-------------|
| D1 | Safeguarding Status 保护状况 | 0.30 | Measures the formal recognition and institutional support for the ICH element |
| D2 | Community Vitality 社区活力 | 0.30 | Measures the active engagement of the bearer community in sustaining the ICH element |
| D3 | Transmission Effectiveness 传承有效性 | 0.25 | Measures the effectiveness of inter-generational transmission |
| D4 | Public Awareness & Influence 公众认知与影响力 | 0.15 | Measures the broader public awareness and cultural influence of the ICH element |

#### Level 2 Indicators (Sub-dimensions) | 二级指标（子维度）

| ID | Sub-dimension | Parent | Weight (within parent) | Description |
|----|--------------|--------|----------------------|-------------|
| D1.1 | Registry status 注册状态 | D1 | 0.35 | Whether the element is inscribed on national/international ICH lists |
| D1.2 | Safeguarding plan 保护计划 | D1 | 0.35 | Existence and quality of safeguarding plans |
| D1.3 | Funding support 资金支持 | D1 | 0.30 | Level of financial support for safeguarding activities |
| D2.1 | Practitioner count 从业者数量 | D2 | 0.30 | Number of active practitioners/transmitters |
| D2.2 | Community engagement 社区参与 | D2 | 0.35 | Level of community participation in ICH practices |
| D2.3 | Practice continuity 实践连续性 | D2 | 0.35 | Continuity of practice over time (no significant interruptions) |
| D3.1 | Apprenticeship system 学徒制 | D3 | 0.35 | Existence and functioning of formal/informal apprenticeship systems |
| D3.2 | Youth involvement 青年参与 | D3 | 0.35 | Proportion of practitioners under 35 years of age |
| D3.3 | Knowledge documentation 知识记录 | D3 | 0.30 | Completeness of documentation of ICH knowledge and techniques |
| D4.1 | Media coverage 媒体报道 | D4 | 0.35 | Volume and quality of media coverage |
| D4.2 | Educational integration 教育整合 | D4 | 0.35 | Integration into formal and informal education |
| D4.3 | Cultural tourism impact 文化旅游影响 | D4 | 0.30 | Contribution to cultural tourism (as a measure of public interest) |

#### Level 3 Indicators (Specific Measures) — Selected Examples | 三级指标（具体度量）— 选取示例

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

### C.1.4 Weight Assignment | 权重分配

Weights were determined using the Analytic Hierarchy Process (AHP) with a panel of 12 ICH experts (§06.1.2 — Expert Panel Method). The AHP process involved:

权重通过分析层次过程（AHP）确定，由12名ICH专家组成的小组进行（§06.1.2——专家组法）。AHP过程包括：

a) pairwise comparison of Level 1 dimensions by each expert;
   每位专家对一级维度进行两两比较；

b) aggregation of individual judgments using the geometric mean;
   使用几何平均聚合个体判断；

c) calculation of priority weights from the aggregate comparison matrix;
   从聚合比较矩阵计算优先权重；

d) consistency check (consistency ratio CR < 0.10 for all experts).
   一致性检验（所有专家的一致性比率CR < 0.10）。

**Resulting Level 1 Weights** | **一级权重结果**:

$$w_{D1} = 0.30, \quad w_{D2} = 0.30, \quad w_{D3} = 0.25, \quad w_{D4} = 0.15$$

### C.1.5 Data Collection | 数据采集

Data collection followed the three-tier classification system (§7.1):

数据采集遵循三级分类体系（§7.1）：

| Data Source Tier | Proportion of Data Points | Examples |
|-----------------|--------------------------|----------|
| Tier 1 (Official/Audited) | 65% | National ICH registry, UNESCO lists, government funding records |
| Tier 2 (Survey/Expert) | 30% | Expert assessment of safeguarding plan quality, community surveys |
| Tier 3 (Unverified/Public) | 5% | Media database searches, public web sources |

**Data quality metrics** | **数据质量度量** (§7.3):

- Accuracy rate: 94% (Tier 1 data verified against original sources)
- Completeness rate: 87% (13% of data points missing, handled by §7.4.1 methods)
- Timeliness index: 91% (data within the declared reference period)

### C.1.6 Scoring and Ranking | 评分与排名

**Normalisation** | **归一化** (§8.2):

Min-max normalisation was applied to all quantitative indicators:

所有定量指标均采用最小-最大归一化：

$$s_{ij} = \frac{x_{ij} - \min_k x_{kj}}{\max_k x_{kj} - \min_k x_{kj}}$$

For qualitative indicators (expert assessments on 1–5 scale), scores were normalised to the [0, 1] interval:

对于定性指标（1–5量表专家评估），得分归一化至[0, 1]区间：

$$s_{ij} = \frac{x_{ij} - 1}{5 - 1}$$

**Aggregation** | **聚合** (§8.3.1):

The weighted arithmetic mean (WAM) was used for aggregation:

使用加权算术平均（WAM）进行聚合：

$$C_i = \sum_{j=1}^{n} w_j \cdot s_{ij}$$

**Illustrative Scoring Results** | **说明性评分结果** (hypothetical data for 5 ICH elements):

| Rank | ICH Element | D1 (0.30) | D2 (0.30) | D3 (0.25) | D4 (0.15) | Composite Score |
|------|-------------|-----------|-----------|-----------|-----------|----------------|
| 1 | Traditional Silk Weaving | 0.89 | 0.85 | 0.82 | 0.78 | 0.846 |
| 2 | Dragon Boat Festival | 0.92 | 0.78 | 0.76 | 0.85 | 0.828 |
| 3 | Ceramic Firing Technique | 0.75 | 0.82 | 0.71 | 0.62 | 0.746 |
| 4 | Folk Music Tradition | 0.68 | 0.65 | 0.72 | 0.58 | 0.662 |
| 5 | Traditional Paper-cutting | 0.71 | 0.55 | 0.48 | 0.65 | 0.588 |

**Robustness Check** | **稳健性检验** (§8.5.3):

Bootstrap resampling (1,000 iterations) was conducted. Results:

进行了自助重抽样（1000次迭代）。结果：

- Mean rank standard deviation across bootstrap samples: 0.3 positions
- Proportion of elements with rank within ±1 of published rank: 92%
- Geometric mean aggregation (alternative method) correlation with WAM: Spearman's ρ = 0.96

### C.1.7 Publication and Audit | 发布与审计

The ranking was published at **Transparency Level 3** (Data Transparency, §9.2.3), including:

排名以**三级透明度**（数据透明，§9.2.3）发布，包括：

a) full methodology documentation;
   完整方法论文件；

b) all Level 1 and Level 2 indicator scores;
   所有一级和二级指标得分；

c) downloadable data files with Level 3 indicator scores;
   包含三级指标得分的可下载数据文件；

d) robustness analysis results;
   稳健性分析结果；

e) limitations disclosure (§9.1.4), including the caveat that the ranking measures safeguarding status and should not be used as the sole basis for funding allocation.
   局限性披露（§9.1.4），包括排名衡量保护状况且不应作为资金分配唯一依据的注意事项。

---

## C.2 Example 2: Consumer Product Quality Ranking | 示例2：消费品品质排名实施框架

### C.2.1 Scenario Description | 场景描述

A ranking entity wishes to develop a quality ranking for a specific consumer product category (e.g., smartphones). The ranking evaluates products based on objective quality measures, user experience, and value for money. The ranking must address the significant risk of data manipulation (e.g., fake reviews,刷单) that is prevalent in consumer product rankings.

某排名实体拟开发特定消费品类别（如智能手机）的品质排名。该排名基于客观质量度量、用户体验和性价比评估产品。该排名必须应对消费品排名中普遍存在的数据操纵（如虚假评论、刷单）风险。

**Applicable standard provisions** | **适用标准条款**: ICO Std 2002 core layer (§04–§11) and SE-01 (Products) extension module.

### C.2.2 Process Flow Diagram | 流程示意图

```
┌─────────────────────────────────────────────────────────────────┐
│  STEP 1: Purpose & Scope Definition (§04, §01)                  │
│  目的与范围界定                                                   │
│  - Define: Consumer product quality assessment                  │
│  - Target: Consumers, manufacturers, regulators                │
│  - Domain: SE-01 (Products)                                     │
└───────────────────────────┬─────────────────────────────────────┘
                            ▼
┌─────────────────────────────────────────────────────────────────┐
│  STEP 2: Category-Differentiated Indicator Design (§05)          │
│  品类差异化指标设计                                                │
│  - Core indicators (common across categories)                   │
│  - Category-specific indicators (unique to product type)        │
│  - Anti-fraud indicators (§7.5)                                 │
└───────────────────────────┬─────────────────────────────────────┘
                            ▼
┌─────────────────────────────────────────────────────────────────┐
│  STEP 3: Weight Assignment with Category Adjustment (§06)        │
│  品类调整权重分配                                                  │
│  - Base weights from AHP                                        │
│  - Category-specific adjustments (documented)                   │
└───────────────────────────┬─────────────────────────────────────┘
                            ▼
┌─────────────────────────────────────────────────────────────────┐
│  STEP 4: Data Collection with Anti-Fraud Measures (§07, §7.5)    │
│  含反欺诈措施的数据采集                                            │
│  - Tier 1: Laboratory test results, certification data          │
│  - Tier 2: Verified user surveys, expert assessments            │
│  - Tier 3: E-commerce reviews (with fraud detection)            │
│  - Anti-fraud: Bot detection, duplicate filtering, outlier flag │
└───────────────────────────┬─────────────────────────────────────┘
                            ▼
┌─────────────────────────────────────────────────────────────────┐
│  STEP 5: Scoring, Ranking & Anti-Brushing Adjustment (§08)       │
│  评分、排名与反刷单调整                                            │
│  - Normalisation: Z-score standardisation                       │
│  - Aggregation: WAM with anti-fraud penalty                     │
│  - Robustness: Method variation + data perturbation             │
└───────────────────────────┬─────────────────────────────────────┘
                            ▼
┌─────────────────────────────────────────────────────────────────┐
│  STEP 6: Publication & Audit (§09, §10)                          │
│  发布与审计                                                      │
│  - Transparency Level 2 (Methodology Transparency)              │
│  - Anti-fraud audit trail                                       │
└─────────────────────────────────────────────────────────────────┘
```

### C.2.3 Indicator System | 指标体系

#### Level 1 Indicators | 一级指标

| ID | Dimension | Weight | Description |
|----|-----------|--------|-------------|
| P1 | Product Performance 产品性能 | 0.35 | Objective technical performance measures |
| P2 | User Experience 用户体验 | 0.30 | Subjective and objective user experience measures |
| P3 | Value for Money 性价比 | 0.20 | Quality relative to price |
| P4 | Brand Reliability 品牌可靠性 | 0.15 | Brand reputation, after-sales service, warranty |

#### Level 2 Indicators — Category-Specific (Smartphones) | 二级指标——品类特定（智能手机）

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

### C.2.4 Anti-Fraud Mechanisms | 反刷单机制

Consumer product rankings are particularly vulnerable to data manipulation. The following anti-fraud measures are applied in accordance with §7.5:

消费品排名特别容易受到数据操纵。按照§7.5的规定，适用以下反欺诈措施：

**a) Tier 3 Data Fraud Detection** | **三级数据欺诈检测**

For e-commerce review data (Tier 3), the following detection algorithms are applied:

对于电商评论数据（三级），适用以下检测算法：

1. **Duplicate detection** | **重复检测**: Reviews with identical or near-identical text are flagged and excluded. Detection threshold: Jaccard similarity > 0.85.
   文本相同或近于相同的评论被标记并排除。检测阈值：Jaccard相似度 > 0.85。

2. **Temporal clustering detection** | **时间聚集检测**: Unusual spikes in review volume (e.g., >3 standard deviations above the mean daily rate) are flagged for manual review.
   评论量异常激增（如日均率的3个标准差以上）被标记以供人工审查。

3. **Account age and activity filter** | **账户年龄和活动过滤**: Reviews from accounts with <30 days of registration or <3 prior reviews are excluded from the scoring calculation.
   注册不足30天或先前评论不足3条的账户的评论被排除在评分计算之外。

**b) Anti-Brushing Penalty** | **反刷单惩罚**

If a product is found to have a statistically significant proportion of fraudulent reviews (as determined by the fraud detection algorithms above), the following penalty is applied:

如果发现某产品具有统计上显著比例的虚假评论（由上述欺诈检测算法确定），则适用以下惩罚：

$$s_{ij}^{\text{adjusted}} = s_{ij} \times (1 - \lambda \cdot p_{\text{fraud}})$$

where $p_{\text{fraud}}$ is the estimated proportion of fraudulent reviews and $\lambda$ is a penalty coefficient (default: $\lambda = 2.0$, meaning the penalty is double the fraud proportion). This ensures that the cost of fraud detection exceeds any potential benefit from manipulation.

其中 $p_{\text{fraud}}$ 为估计的虚假评论比例，$\lambda$ 为惩罚系数（默认：$\lambda = 2.0$，即惩罚为欺诈比例的两倍）。这确保欺诈检测的成本超过操纵的任何潜在收益。

**Illustrative Example** | **说明性示例**:

Product A has a User Satisfaction Score (P2.1) of 0.85 based on 1,000 reviews. Fraud detection identifies 150 reviews as potentially fraudulent ($p_{\text{fraud}} = 0.15$). The adjusted score is:

产品A基于1000条评论的用户满意度得分（P2.1）为0.85。欺诈检测识别出150条可能虚假的评论（$p_{\text{fraud}} = 0.15$）。调整后得分为：

$$s_{A,P2.1}^{\text{adjusted}} = 0.85 \times (1 - 2.0 \times 0.15) = 0.85 \times 0.70 = 0.595$$

### C.2.5 Scoring and Ranking | 评分与排名

**Normalisation** | **归一化** (§8.2):

Z-score standardisation was applied:

应用z-分数标准化：

$$s_{ij} = \frac{x_{ij} - \mu_j}{\sigma_j}$$

followed by rescaling to [0, 1] using the percentile method to ensure comparability.

随后使用百分位方法重新缩放至[0, 1]以确保可比性。

**Aggregation** | **聚合** (§8.3.1):

WAM with anti-fraud penalty adjustments:

含反欺诈惩罚调整的WAM：

$$C_i = \sum_{j=1}^{n} w_j \cdot s_{ij}^{\text{adjusted}}$$

**Illustrative Scoring Results** | **说明性评分结果** (hypothetical data for 5 smartphones):

| Rank | Product | P1 (0.35) | P2 (0.30) | P3 (0.20) | P4 (0.15) | Composite | Fraud Penalty Applied |
|------|---------|-----------|-----------|-----------|-----------|-----------|----------------------|
| 1 | Phone Alpha | 0.92 | 0.88 | 0.75 | 0.82 | 0.863 | No |
| 2 | Phone Beta | 0.88 | 0.82 | 0.85 | 0.78 | 0.838 | No |
| 3 | Phone Gamma | 0.85 | 0.595 | 0.72 | 0.75 | 0.718 | Yes (P2.1 adjusted) |
| 4 | Phone Delta | 0.72 | 0.75 | 0.68 | 0.70 | 0.716 | No |
| 5 | Phone Epsilon | 0.68 | 0.70 | 0.62 | 0.65 | 0.667 | No |

> **Note**: Phone Gamma's lower User Experience score (P2 = 0.595) reflects the anti-brushing penalty applied to its user satisfaction data. Without the penalty, its P2 score would have been 0.85, and it would have ranked 3rd or higher. The anti-fraud adjustment is documented in the methodology statement and the fraud detection audit trail.
>
> **注**：Phone Gamma较低的用户体验得分（P2 = 0.595）反映了对其用户满意度数据应用的反刷单惩罚。若无惩罚，其P2得分为0.85，排名将第3或更高。反欺诈调整在方法论声明和欺诈检测审计追踪中记录。

### C.2.6 Sensitivity Analysis | 敏感性分析

The following sensitivity analyses were conducted in accordance with §8.5.3:

按照§8.5.3的规定，进行了以下敏感性分析：

**a) Weight variation test** | **权重变异测试**:

All Level 1 weights were varied by ±5 percentage points. The maximum rank change was 1 position, indicating that the ranking is robust to moderate weight variations.

所有一级权重变化±5个百分点。最大排名变化为1位，表明排名对中等权重变异具有稳健性。

**b) Method variation test** | **方法变异测试**:

The ranking was recomputed using the geometric mean aggregation method. The Spearman's ρ between WAM and geometric mean rankings was 0.94, indicating high consistency.

使用几何平均聚合方法重新计算排名。WAM和几何平均排名之间的Spearman ρ为0.94，表明高度一致。

**c) Data perturbation test** | **数据扰动测试**:

Random noise (±5% of the standard deviation of each indicator) was added to the input data. The ranking was recomputed 100 times. The mean rank stability (proportion of elements with unchanged rank) was 88%.

向输入数据添加随机噪声（每个指标标准差的±5%）。排名重新计算100次。平均排名稳定性（排名不变的实体比例）为88%。

---

## C.3 Example 3: Cross-Domain Comprehensive Ranking | 示例3：跨领域综合排名实施框架

### C.3.1 Scenario Description | 场景描述

A ranking entity wishes to develop a comprehensive ranking that evaluates entities across multiple dimensions from different domains (e.g., a "City Livability Index" that combines economic, environmental, cultural, and infrastructural indicators). The primary challenge is the meaningful aggregation of indicators from different domains with different measurement scales and units.

某排名实体拟开发跨领域综合排名，从不同领域评估实体的多个维度（如结合经济、环境、文化和基础设施指标的"城市宜居指数"）。主要挑战在于不同领域、不同测量尺度和单位的指标的有意义聚合。

**Applicable standard provisions** | **适用标准条款**: ICO Std 2002 core layer (§04–§11), with cross-references to SE-04 (Cities), SE-08 (Sustainability), and SE-05 (Cultural Heritage).

### C.3.2 Process Flow Diagram | 流程示意图

```
┌─────────────────────────────────────────────────────────────────┐
│  STEP 1: Purpose & Scope Definition (§04, §01)                  │
│  目的与范围界定                                                   │
│  - Define: City livability assessment                           │
│  - Target: Residents, policy-makers, investors                 │
│  - Cross-domain: SE-04 + SE-08 + SE-05                         │
└───────────────────────────┬─────────────────────────────────────┘
                            ▼
┌─────────────────────────────────────────────────────────────────┐
│  STEP 2: Multi-Domain Indicator Design (§05)                     │
│  多领域指标设计                                                   │
│  - Domain-specific indicators (each domain validated)           │
│  - Cross-domain integration rules                               │
│  - Normalisation method selection for cross-domain comparison   │
└───────────────────────────┬─────────────────────────────────────┘
                            ▼
┌─────────────────────────────────────────────────────────────────┐
│  STEP 3: Cross-Domain Weight Assignment (§06)                    │
│  跨领域权重分配                                                   │
│  - Stakeholder consultation for inter-domain weights            │
│  - AHP for intra-domain weights                                │
│  - Sensitivity analysis across domain weight variations         │
└───────────────────────────┬─────────────────────────────────────┘
                            ▼
┌─────────────────────────────────────────────────────────────────┐
│  STEP 4: Data Collection (§07)                                   │
│  数据采集                                                        │
│  - Tier 1: Official statistics, government databases            │
│  - Tier 2: Resident surveys, expert assessments                │
│  - Tier 3: Social media, public web sources                    │
│  - Cross-domain data harmonisation                              │
└───────────────────────────┬─────────────────────────────────────┘
                            ▼
┌─────────────────────────────────────────────────────────────────┐
│  STEP 5: Scoring, Ranking & Sensitivity Analysis (§08)           │
│  评分、排名与敏感性分析                                            │
│  - Normalisation: Percentile ranking (cross-domain comparable)  │
│  - Aggregation: WAM with domain interaction effects             │
│  - Sensitivity: Multi-dimensional weight sensitivity analysis   │
│  - Robustness: Bootstrap + method variation + domain exclusion  │
└───────────────────────────┬─────────────────────────────────────┘
                            ▼
┌─────────────────────────────────────────────────────────────────┐
│  STEP 6: Publication & Audit (§09, §10)                          │
│  发布与审计                                                      │
│  - Transparency Level 4 (Full Reproducibility)                 │
│  - Interactive ranking tool (§06.4)                             │
│  - Comprehensive sensitivity analysis report                    │
└─────────────────────────────────────────────────────────────────┘
```

### C.3.3 Indicator System | 指标体系

#### Level 1 Indicators (Domains) | 一级指标（领域）

| ID | Domain | Weight | Source Module | Description |
|----|--------|--------|--------------|-------------|
| L1 | Economic Vitality 经济活力 | 0.25 | SE-04 | Economic output, employment, innovation |
| L2 | Environmental Quality 环境质量 | 0.25 | SE-08 | Air quality, green space, GHG emissions |
| L3 | Cultural Richness 文化丰富度 | 0.20 | SE-05 | Cultural heritage, creative industries, cultural participation |
| L4 | Infrastructure & Services 基础设施与服务 | 0.30 | SE-04 | Transportation, healthcare, education, housing |

#### Level 2 and Level 3 Indicators — Selected Examples | 二级和三级指标——选取示例

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

### C.3.4 Cross-Domain Normalisation | 跨领域归一化

**Challenge** | **挑战**: Indicators from different domains have different measurement scales (e.g., GDP in currency units, AQI in index units, employment rates in percentages). Direct comparison requires a common normalisation method.

不同领域的指标具有不同的测量尺度（如GDP以货币单位计、AQI以指数单位计、就业率以百分比计）。直接比较需要共同的归一化方法。

**Method** | **方法**: Percentile ranking normalisation (§8.2) was selected for its robustness to outliers and its ability to produce comparable scores across different scales:

选择百分位排名归一化（§8.2），因为其对异常值具有稳健性，且能跨不同尺度产生可比得分：

$$s_{ij} = \frac{R_{ij} - 1}{N - 1}$$

where $R_{ij}$ is the rank of entity $i$ on indicator $j$ and $N$ is the total number of entities.

其中 $R_{ij}$ 为实体 $i$ 在指标 $j$ 上的排名，$N$ 为实体总数。

For indicators where lower values are better (e.g., AQI, GHG emissions), inverse ranking is applied:

对于较低值更好的指标（如AQI、GHG排放），应用逆排名：

$$s_{ij} = 1 - \frac{R_{ij} - 1}{N - 1}$$

### C.3.5 Weight Assignment | 权重分配

Weights were determined through a combination of stakeholder consultation and expert panel methods (§06.1):

权重通过利益相关方咨询和专家组法的组合确定（§06.1）：

a) **Inter-domain weights** (Level 1): Determined through stakeholder consultation with 200 residents, 30 policy-makers, and 20 investors. The final weights were calibrated to reflect the consensus priorities of the target audience.
   领域间权重（一级）：通过与200名居民、30名政策制定者和20名投资者的利益相关方咨询确定。最终权重经校准以反映目标受众的共识优先级。

b) **Intra-domain weights** (Level 2 and Level 3): Determined through AHP with a panel of 8 domain experts (2 per domain).
   领域内权重（二级和三级）：通过由8名领域专家（每领域2名）组成的AHP确定。

### C.3.6 Sensitivity Analysis | 敏感性分析

Cross-domain rankings are particularly sensitive to the choice of domain weights. The following multi-dimensional sensitivity analysis was conducted:

跨领域排名对领域权重选择特别敏感。进行了以下多维敏感性分析：

**a) One-at-a-time (OAT) weight variation** | **逐项权重变异**:

Each Level 1 weight was independently varied by ±5 and ±10 percentage points, with the remaining weights adjusted proportionally. The maximum rank change for any entity was:

每个一级权重独立变化±5和±10个百分点，其余权重按比例调整。任何实体的最大排名变化为：

| Weight Variation | Max Rank Change | Entities with ≥2 Position Change |
|-----------------|-----------------|----------------------------------|
| ±5 pp | 2 positions | 3 of 50 cities |
| ±10 pp | 4 positions | 8 of 50 cities |

**b) Multi-dimensional weight sensitivity** | **多维权重敏感性**:

A Monte Carlo simulation was conducted with 10,000 random weight combinations (drawn from a Dirichlet distribution with the mean equal to the published weights). For each entity, the following statistics were computed:

使用10,000个随机权重组合（从均值等于发布权重的Dirichlet分布中抽取）进行蒙特卡洛模拟。对每个实体计算以下统计量：

| Statistic | Description |
|-----------|-------------|
| Mean rank | Average rank across all weight combinations |
| Rank standard deviation | Variability of rank across weight combinations |
| 90% rank interval | 5th to 95th percentile of rank distribution |
| Rank stability index | Proportion of weight combinations where rank is within ±3 of published rank |

**Illustrative Results** | **说明性结果** (for 5 hypothetical cities):

| City | Published Rank | Mean Rank | Rank SD | 90% Interval | Stability Index |
|------|---------------|-----------|---------|--------------|----------------|
| City A | 1 | 1.2 | 0.5 | [1, 2] | 98% |
| City B | 2 | 2.8 | 1.1 | [1, 5] | 72% |
| City C | 3 | 3.5 | 1.8 | [1, 7] | 55% |
| City D | 4 | 4.2 | 1.5 | [2, 8] | 48% |
| City E | 5 | 4.8 | 1.2 | [2, 7] | 62% |

> **Note**: City B's relatively low stability index (72%) indicates that its rank is sensitive to the choice of domain weights. This is because City B excels in Economic Vitality (L1) but is weaker in Environmental Quality (L2), and the relative importance of these domains significantly affects its ranking. This sensitivity is disclosed in the limitations section (§9.1.4).
>
> **注**：City B相对较低的稳定性指数（72%）表明其排名对领域权重选择敏感。这是因为City B在经济活力（L1）方面表现优异，但在环境质量（L2）方面较弱，这些领域的相对重要性显著影响其排名。此敏感性在局限性部分（§9.1.4）中披露。

**c) Domain exclusion test** | **领域排除测试**:

The ranking was recomputed with each domain excluded in turn. This test identifies which domains have the greatest influence on the ranking:

依次排除每个领域重新计算排名。此测试识别哪些领域对排名影响最大：

| Excluded Domain | Mean Rank Change | Max Rank Change |
|----------------|-----------------|-----------------|
| L1 (Economic) | 2.8 positions | 8 positions |
| L2 (Environmental) | 2.2 positions | 6 positions |
| L3 (Cultural) | 1.5 positions | 5 positions |
| L4 (Infrastructure) | 3.2 positions | 10 positions |

The results indicate that Infrastructure & Services (L4) has the greatest influence on the ranking, which is consistent with its highest weight (0.30). This finding is documented in the methodology statement.

结果表明基础设施与服务（L4）对排名影响最大，这与其最高权重（0.30）一致。此发现记录在方法论声明中。

### C.3.7 Interactive Ranking Tool | 交互式排名工具

In accordance with §06.4 (User-Adjustable Weights), an interactive ranking tool was provided that allows users to:

按照§06.4（用户可调权重），提供了交互式排名工具，允许用户：

a) adjust the Level 1 domain weights using slider controls;
   使用滑块控制调整一级领域权重；

b) recompute the ranking in real time based on the adjusted weights;
   基于调整后的权重实时重新计算排名；

c) compare the user-adjusted ranking with the default ranking entity ranking;
   将用户调整排名与默认排名实体排名进行比较；

d) view the sensitivity analysis results for each entity.
   查看每个实体的敏感性分析结果。

The tool prominently displays the default (ranking entity) weights alongside any user-adjusted results, with a clear notice that user-adjusted rankings are not the official ranking.

该工具显著展示默认（排名实体）权重与任何用户调整结果，并明确说明用户调整排名非官方排名。

### C.3.8 Publication | 发布

The ranking was published at **Transparency Level 4** (Full Reproducibility, §9.2.4), including:

排名以**四级透明度**（完全可复现，§9.2.4）发布，包括：

a) complete methodology documentation;
   完整方法论文件；

b) all indicator scores at every hierarchical level;
   每个层级所有指标得分；

c) complete dataset (downloadable in CSV format);
   完整数据集（以CSV格式下载）；

d) analysis code (Python scripts for scoring, aggregation, and sensitivity analysis);
   分析代码（用于评分、聚合和敏感性分析的Python脚本）；

e) comprehensive sensitivity analysis report;
   全面的敏感性分析报告；

f) interactive ranking tool with user-adjustable weights;
   含用户可调权重的交互式排名工具；

g) limitations disclosure (§9.1.4), including the caveat that the ranking measures relative livability and should not be used as the sole basis for relocation or investment decisions.
   局限性披露（§9.1.4），包括排名衡量相对宜居性且不应作为搬迁或投资决策唯一依据的注意事项。

---

## C.4 Cross-Example Comparison | 跨示例比较

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

---

## C.5 Key Implementation Lessons | 关键实施要点

### C.5.1 Indicator Design | 指标设计

a) Indicator selection must be driven by the ranking purpose (§05.1), not by data availability. In Example 1, the indicator system includes qualitative measures (e.g., safeguarding plan quality) that require Tier 2 data collection, even though Tier 1 data alone would have been easier to collect.
   指标选择必须由排名目的驱动（§05.1），而非数据可用性。在示例1中，指标体系包含需要二级数据采集的定性度量（如保护计划质量），尽管仅使用一级数据会更容易采集。

b) Domain-specific indicators should be validated by domain experts (§05.1). In all three examples, domain experts were involved in the indicator selection process.
   领域特定指标应由领域专家验证（§05.1）。在所有三个示例中，领域专家参与了指标选择过程。

### C.5.2 Weight Assignment | 权重分配

a) The choice of weighting method should be documented and justified (§06.1). AHP is suitable when expert judgment is available; stakeholder consultation is appropriate when the ranking target audience has diverse perspectives.
   权重方法的选择应予以记录和论证（§06.1）。当专家判断可用时，AHP是合适的；当排名目标受众具有多元视角时，利益相关方咨询是适当的。

b) Weight sensitivity analysis (§8.5.3) is essential for cross-domain rankings where the relative importance of different domains may vary across stakeholders.
   权重敏感性分析（§8.5.3）对于不同领域相对重要性可能因利益相关方而异的跨领域排名至关重要。

### C.5.3 Data Quality and Anti-Fraud | 数据质量与反欺诈

a) The three-tier data source classification (§7.1) provides a practical framework for managing data quality across different source types.
   三级数据源分类（§7.1）为管理不同来源类型的数据质量提供了实用框架。

b) Anti-fraud mechanisms (§7.5) are essential for consumer product rankings where data manipulation is a known risk. The anti-brushing penalty mechanism provides a deterrent that is proportional to the detected fraud.
   反欺诈机制（§7.5）对于数据操纵为已知风险的消费品排名至关重要。反刷单惩罚机制提供了与检测到的欺诈成比例的威慑。

### C.5.4 Transparency and Reproducibility | 透明度与可复现性

a) The four-level transparency system (§9.2) provides a practical framework for progressively improving the transparency of ranking publications. Ranking entities should aim for the highest achievable transparency level, given the sensitivity of the data and the needs of the target audience.
   四级透明度体系（§9.2）为逐步改进排名发布透明度提供了实用框架。排名实体应在考虑数据敏感性和目标受众需求的前提下，追求可实现的最高透明度等级。

b) User-adjustable weights (§06.4) are particularly valuable for cross-domain rankings where different stakeholders may have different priorities. The interactive ranking tool provides a mechanism for stakeholder engagement that goes beyond the Berlin Principles' recommendation of consumer choice.
   用户可调权重（§06.4）对于不同利益相关方可能具有不同优先级的跨领域排名特别有价值。交互式排名工具提供了超越柏林原则消费者选择建议的利益相关方参与机制。

---

> **Note**: This annex is informative and part of ICO Std 2002 (Tianji Ranking Methodology Standard). The examples are illustrative only and do not represent actual rankings. All data, scores, and entity names are hypothetical.
>
> **注**：本附录为资料性附录，属于ICO Std 2002（天机排名方法论标准）。本示例仅供说明之用，不代表实际排名。所有数据、得分和实体名称均为假设性数据。
