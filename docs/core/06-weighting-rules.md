# Chapter 6: Weighting Rules | 第6章 权重分配规则

**ICO Std 2002:2026 — Chapter 6**

---

This chapter specifies the methods, procedures, and requirements for assigning weights to indicators in a ranking system. It establishes rules for weight determination, sensitivity analysis, disclosure, prohibited practices, and cross-domain weight coordination.

本章规定了排名系统中指标权重分配的方法、程序和要求。它确立了权重确定、敏感性分析、披露、禁止行为和跨领域权重协调的规则。

---

## 6.1 Weight Assignment Methods | 权重分配方法论

The ranking entity shall select a weight assignment method from those specified in 6.1.1 through 6.1.4, or a combination thereof, and shall document the rationale for the selection (see 6.2.1).

排名实体应从6.1.1至6.1.4规定的方法中选择权重分配方法或其组合，并应记录选择的理由（见6.2.1）。

### 6.1.1 Equal Weighting | 等权法

Equal weighting assigns the same weight to all indicators at a given hierarchical level.

等权法对给定层级的所有指标赋予相同权重。

For *n* indicators at level *k*, the weight of indicator *i* is:

对于层级 *k* 的 *n* 个指标，指标 *i* 的权重为：

$$w_i^{(k)} = \frac{1}{n}, \quad i = 1, 2, \ldots, n; \quad \sum_{i=1}^{n} w_i^{(k)} = 1$$

**Applicability** | **适用场景**:

a) Where no defensible theoretical or empirical basis exists for differential weighting.

当不存在差异赋权的可辩护理论或实证依据时。

b) As a baseline for sensitivity analysis (see 6.3).

作为敏感性分析的基线（见6.3）。

c) For ranking systems with a small number of indicators (typically *n* ≤ 5) where the indicators represent equally important dimensions.

对于指标数量较少（通常 *n* ≤ 5）且指标代表同等重要维度的排名系统。

**Limitations** | **局限性**:

a) Equal weighting implicitly assumes that all indicators contribute equally to the ranking purpose, which is rarely the case in practice.

等权法隐含假设所有指标对排名目的的贡献相同，这在实践中很少成立。

b) Equal weighting does not account for differences in indicator reliability or variance.

等权法不考虑指标可靠性或方差的差异。

c) When indicators have different numbers of sub-indicators, equal weighting at the dimension level may introduce indirect weighting bias at the sub-indicator level.

当指标具有不同数量的子指标时，维度层的等权法可能在子指标层引入间接赋权偏差。

### 6.1.2 Expert-Based Weighting | 专家赋权法

Expert-based weighting methods derive weights from the informed judgement of domain experts. The following methods are recognised:

专家赋权法从领域专家的知情判断中导出权重。认可以下方法：

#### 6.1.2.1 Delphi Method | 德尔菲法

The Delphi method derives weights through iterative, anonymous expert consultation with controlled feedback. The requirements specified in 5.4.2 shall apply, with the following additional requirements:

德尔菲法通过迭代的、匿名的、有控制反馈的专家咨询导出权重。5.4.2规定的要求应适用，另加以下要求：

a) The expert panel shall include at least seven members for weight determination.

专家小组应包括至少七名成员用于权重确定。

b) At least three rounds of consultation shall be conducted.

应进行至少三轮咨询。

c) The final weights shall be calculated as the median of the experts' final-round estimates.

最终权重应计算为专家最后一轮估计的中位数。

d) The dispersion of expert judgements (interquartile range) shall be reported.

应报告专家判断的离散度（四分位距）。

#### 6.1.2.2 Analytic Hierarchy Process (AHP) | 层次分析法

The AHP derives weights from pairwise comparisons of indicator importance. The requirements specified in 5.4.3 shall apply, with the following additional requirements:

AHP从指标重要性的配对比较中导出权重。5.4.3规定的要求应适用，另加以下要求：

a) The pairwise comparison scale shall follow the Saaty 1–9 scale.

配对比较量表应遵循Saaty 1–9量表。

b) The consistency ratio (CR) shall be calculated for each comparison matrix. A matrix with CR > 0.10 shall be revised.

应计算每个比较矩阵的一致性比率（CR）。CR > 0.10的矩阵应予以修订。

c) When multiple experts participate, individual priority vectors shall be aggregated using the geometric mean method.

当多名专家参与时，应使用几何平均法聚合个体优先向量。

### 6.1.3 Data-Driven Weighting | 数据驱动法

Data-driven weighting methods derive weights from the statistical properties of the data. The following methods are recognised:

数据驱动赋权法从数据的统计特性中导出权重。认可以下方法：

#### 6.1.3.1 Principal Component Analysis (PCA) | 主成分分析

PCA-derived weights are obtained from the factor loadings of the first principal component or from the proportion of variance explained by each indicator. The requirements specified in 5.4.4 shall apply.

PCA导出的权重从第一主成分的因子载荷或每个指标解释的方差比例获得。5.4.4规定的要求应适用。

#### 6.1.3.2 Factor Analysis | 因子分析

Factor analysis may be used to derive weights from the factor structure of the indicator data. When factor analysis is used for weighting:

因子分析可用于从指标数据的因子结构导出权重。当因子分析用于赋权时：

a) The factor extraction method (e.g., maximum likelihood, principal axis factoring) shall be documented.

应记录因子提取方法（如最大似然法、主轴因子法）。

b) The factor rotation method (if any) shall be documented.

应记录因子旋转方法（如有）。

c) Factor scores shall be used to derive weights only after confirming the theoretical meaningfulness of the factor structure.

只有在确认因子结构的理论意义之后，因子得分才应用于导出权重。

#### 6.1.3.3 Entropy Method | 熵权法

The entropy method derives weights from the information entropy of each indicator, assigning higher weights to indicators with greater variation. The entropy weight for indicator *j* is calculated as:

熵权法从每个指标的信息熵导出权重，对变异程度更大的指标赋予更高权重。指标 *j* 的熵权计算如下：

Step 1: Normalise the data:

步骤1：归一化数据：

$$p_{ij} = \frac{x_{ij}}{\sum_{i=1}^{m} x_{ij}}$$

where *x_{ij}* is the value of indicator *j* for entity *i*, and *m* is the number of entities.

其中 *x_{ij}* 为实体 *i* 的指标 *j* 的值，*m* 为实体数量。

Step 2: Calculate the entropy of indicator *j*:

步骤2：计算指标 *j* 的熵：

$$e_j = -\frac{1}{\ln m} \sum_{i=1}^{m} p_{ij} \ln(p_{ij})$$

Step 3: Calculate the weight:

步骤3：计算权重：

$$w_j = \frac{1 - e_j}{\sum_{j=1}^{n} (1 - e_j)}$$

where *n* is the number of indicators.

其中 *n* 为指标数量。

> **Note**: The entropy method reflects the discriminative power of each indicator but does not capture substantive importance. It should be used in conjunction with expert judgement or as a validation tool rather than as the sole basis for weight assignment.
>
> **注**：熵权法反映每个指标的区分力，但不捕捉实质重要性。它应与专家判断结合使用或作为验证工具，而不应作为权重分配的唯一依据。

### 6.1.4 Hybrid Weighting | 混合法

Hybrid weighting combines two or more of the methods specified in 6.1.1 through 6.1.3. The ranking entity shall document:

混合法组合6.1.1至6.1.3中规定的两种或多种方法。排名实体应记录：

a) the methods combined and the combination formula;

组合的方法及组合公式；

b) the rationale for the combination;

组合的理由；

c) the contribution of each method to the final weights.

每种方法对最终权重的贡献。

A common hybrid approach is to combine expert-based and data-driven weights:

常见的混合方法是将专家赋权与数据驱动赋权相结合：

$$w_j = \alpha \cdot w_j^{\text{expert}} + (1 - \alpha) \cdot w_j^{\text{data}}, \quad \alpha \in [0, 1]$$

where $\alpha$ is the blending parameter, $w_j^{\text{expert}}$ is the expert-derived weight, and $w_j^{\text{data}}$ is the data-driven weight. The value of $\alpha$ shall be justified and documented.

其中 $\alpha$ 为混合参数，$w_j^{\text{expert}}$ 为专家导出的权重，$w_j^{\text{data}}$ 为数据驱动的权重。$\alpha$ 的值应有依据并予以记录。

---

## 6.2 Weight Determination Process | 权重确定流程

The determination of final weights shall follow a structured process that ensures rigour, transparency, and stakeholder involvement.

最终权重的确定应遵循结构化过程，确保严谨性、透明度和利益相关方参与。

### 6.2.1 Methodology Selection Documentation | 方法论选择理由文档化

The ranking entity shall document the following before proceeding with weight determination:

排名实体应在进行权重确定之前记录以下内容：

a) the weight assignment method selected (from 6.1);

选择的权重分配方法（来自6.1）；

b) the rationale for the selection, including:

选择的理由，包括：

1) the theoretical considerations supporting the choice;

支持该选择的理论考量；

2) the data characteristics relevant to the choice;

与该选择相关的数据特征；

3) the practical constraints influencing the choice.

影响该选择的实践约束。

c) any alternative methods considered and the reasons for their rejection.

考虑的任何替代方法及其被拒绝的理由。

### 6.2.2 Stakeholder Participation Rules | 利益相关方参与规则

Stakeholders shall have the opportunity to provide input on the weight assignment. The following rules shall apply:

利益相关方应有机会对权重分配提供意见。以下规则应适用：

a) The ranking entity shall publish the proposed initial weight scheme and invite stakeholder comments for a period of no less than 30 calendar days.

排名实体应公布拟议的初始权重方案，并邀请利益相关方在不少于30个日历日的期限内提供意见。

b) Stakeholder comments shall be documented, including the disposition of each comment (accepted, partially accepted, or rejected with rationale).

利益相关方意见应予以记录，包括每条意见的处理方式（接受、部分接受或拒绝并附理由）。

c) Representatives of ranked entities shall not have decision-making authority over the final weights.

被排实体的代表不应拥有对最终权重的决策权。

d) The ranking entity shall maintain a record of all stakeholder interactions related to weight determination.

排名实体应保存与权重确定相关的所有利益相关方互动记录。

### 6.2.3 Transparency of the Weight Determination Process | 权重确定过程的透明度要求

The entire weight determination process shall be transparent. The ranking entity shall:

权重确定的整个过程应是透明的。排名实体应：

a) publish the weight determination methodology before its application;

在应用之前公布权重确定方法论；

b) disclose all intermediate results (e.g., expert panel responses, factor loadings, entropy values);

披露所有中间结果（如专家小组回应、因子载荷、熵值）；

c) provide a clear audit trail from initial weights to final weights.

提供从初始权重到最终权重的清晰审计轨迹。

---

## 6.3 Sensitivity Analysis Requirements | 敏感性分析要求

The ranking entity shall conduct sensitivity analysis on the weights to assess the robustness of the ranking results.

排名实体应对权重进行敏感性分析，以评估排名结果的稳健性。

### 6.3.1 Mandatory Sensitivity Analysis | 必须进行的敏感性分析

The ranking entity shall perform at least the following sensitivity analyses:

排名实体应至少进行以下敏感性分析：

a) **±10 % weight variation test** | **±10%权重变动测试**: Each weight shall be individually increased and decreased by 10 percentage points (redistributing the difference proportionally among the remaining weights). The impact on the ranking of each entity shall be recorded.

每个权重应单独增减10个百分点（将差额按比例在其余权重间重新分配）。对每个实体排名的影响应予以记录。

b) **Extreme weight scenario test** | **极端权重情景测试**: The ranking shall be computed with each weight individually set to zero (redistributing to other weights) and with each weight individually set to dominate (≥ 50 % of total weight). The impact on the ranking shall be recorded.

应在每个权重单独设为零（重新分配给其他权重）和每个权重单独占主导（≥总权重的50%）的情况下计算排名。对排名的影响应予以记录。

c) **Equal weight comparison** | **等权比较**: The ranking produced by the final weights shall be compared with the ranking produced by equal weights. The correlation between the two rankings (e.g., Spearman's ρ) and the number and magnitude of rank changes shall be reported.

最终权重产生的排名应与等权法产生的排名进行比较。两个排名之间的相关性（如Spearman ρ）以及排名变化的数量和幅度应予以报告。

### 6.3.2 Reporting of Sensitivity | 敏感程度报告

The ranking entity shall report:

排名实体应报告：

a) the overall sensitivity of the ranking to weight changes, expressed as:

排名对权重变化的总体敏感度，表示为：

1) the average rank change across all ranked entities;

所有被排实体的平均排名变化；

2) the maximum rank change for any single entity;

任何单一实体的最大排名变化；

3) the proportion of entities whose rank changes by more than 5 positions (or 10 % of the total number of ranked entities, whichever is greater).

排名变化超过5位（或被排实体总数的10%，取较大者）的实体比例。

b) the identification of entities whose ranking is highly sensitive to weight changes, which shall be flagged in the publication.

识别排名对权重变化高度敏感的实体，该类实体应在发布中予以标记。

> **Note**: If the sensitivity analysis reveals that the ranking is highly sensitive to small weight changes (e.g., average rank change > 10 positions under ±10% weight variation), the ranking entity should review the indicator system for potential redundancy or instability and should consider increasing the number of data points or improving indicator quality.
>
> **注**：如果敏感性分析揭示排名对小权重变化高度敏感（如在±10%权重变动下平均排名变化>10位），排名实体宜审查指标体系是否存在冗余或不稳定，并宜考虑增加数据点数量或改善指标质量。

---

## 6.4 Weight Disclosure Requirements | 权重披露要求

### 6.4.1 Full Weight Disclosure | 全部权重披露

All indicator weights shall be publicly disclosed in the ranking publication. The disclosure shall include:

所有指标权重应在排名发布中公开披露。披露应包括：

a) the numerical value of each weight, reported to at least three decimal places;

每个权重的数值，至少报告至三位小数；

b) the hierarchical level at which each weight applies;

每个权重适用的层级；

c) the sum of weights at each hierarchical level (which shall equal 1.000).

每个层级权重之和（应等于1.000）。

### 6.4.2 Weight Methodology Disclosure | 权重方法论披露

The method used to determine the weights shall be disclosed, including:

确定权重所使用的方法应予以披露，包括：

a) the name and description of the method;

方法的名称和描述；

b) the data and inputs used in the weight determination process;

权重确定过程中使用的数据和输入；

c) the key parameters and assumptions of the method;

方法的关键参数和假设；

d) the results of any sensitivity analysis (see 6.3).

任何敏感性分析的结果（见6.3）。

### 6.4.3 Weight Change Disclosure | 权重变动披露

When the weights differ from those used in the previous ranking cycle, the ranking entity shall:

当权重与上一排名周期使用的权重不同时，排名实体应：

a) disclose the previous and current weights side by side;

并排披露先前权重和当前权重；

b) provide a reasoned explanation for each weight change that exceeds ±0.01 in absolute terms;

对绝对值超过±0.01的每项权重变动提供理由说明；

c) report the impact of the weight changes on the ranking results, including the number of entities that changed rank by more than 5 positions.

报告权重变化对排名结果的影响，包括排名变化超过5位的实体数量。

---

## 6.5 Prohibited Practices | 禁止行为

The following practices are prohibited under this standard:

本标准禁止以下行为：

### 6.5.1 Commercially Motivated Weight Adjustment | 禁止根据商业利益调整权重

Weights shall not be adjusted to favour any ranked entity for commercial benefit to the ranking entity or any affiliated party. This includes, but is not limited to:

权重不应为排名实体或任何关联方的商业利益而调整以有利于任何被排实体。这包括但不限于：

a) increasing the weight of indicators on which a paying entity scores highly;

增加付费实体得分较高指标的权重；

b) decreasing the weight of indicators on which a paying entity scores poorly;

降低付费实体得分较低指标的权重；

c) creating or modifying indicators and their weights to accommodate sponsorship or advertising agreements.

创建或修改指标及其权重以适应赞助或广告协议。

### 6.5.2 Entity-Specific Weight Customisation | 禁止为特定被排实体定制权重

The weight scheme shall be uniform across all ranked entities. It is prohibited to:

权重方案应在所有被排实体间统一。禁止：

a) apply different weights to different ranked entities;

对不同被排实体适用不同权重；

b) select weights that are optimised for a specific entity's data profile;

选择针对特定实体数据特征优化的权重；

c) adjust weights post hoc based on preliminary ranking results.

基于初步排名结果事后调整权重。

### 6.5.3 Intra-Cycle Weight Modification | 权重变动不得在排名周期内临时修改

Once the weight scheme for a ranking cycle has been finalised and published, it shall not be modified within that cycle. Any necessary changes shall be implemented in the next cycle, following the process specified in 6.2 and 5.5.

一旦排名周期的权重方案已最终确定并发布，不应在该周期内修改。任何必要的变更应在下一个周期按照6.2和5.5规定的程序实施。

> **Note**: The prohibition in 6.5.3 does not preclude the correction of computational errors; however, any such correction shall be documented and disclosed in accordance with the transparency requirements of 4.2.
>
> **注**：6.5.3的禁止不排除计算错误的更正；但任何此类更正应按照4.2的透明度要求予以记录和披露。

---

## 6.6 Cross-Domain Weight Coordination | 跨领域权重协调

### 6.6.1 Core-Layer Weight Methodology Uniformity | 核心层权重方法论的统一性

The weight assignment methodology specified in this chapter shall apply uniformly across all ranking domains covered by this standard. This ensures that:

本章规定的权重分配方法论应在本标准涵盖的所有排名领域统一适用。这确保：

a) all ranking systems under this standard employ a consistent methodological framework for weight determination;

本标准下所有排名系统采用一致的权重确定方法论框架；

b) the validity and comparability of weighting practices are maintained across domains;

赋权实践的有效性和可比性在领域间得到保持；

c) users can understand and compare the weighting approaches of different ranking systems without needing to learn domain-specific conventions.

用户可以在无需学习领域特定惯例的情况下理解和比较不同排名系统的赋权方法。

### 6.6.2 Extension-Layer Domain Weight Independence | 扩展层领域权重的独立性

Within the methodological framework defined by the core layer, extension modules may define domain-specific weighting practices that reflect the substantive characteristics of the domain. Such practices shall:

在核心层定义的方法论框架内，扩展模块可定义反映领域实质特征的领域特定赋权实践。此类实践应：

a) comply with the general requirements of this chapter;

遵守本章的一般要求；

b) justify any deviations from the core-layer default practices;

论证偏离核心层默认实践的任何情况；

c) be documented in the extension module with reference to this chapter.

在扩展模块中参照本章予以记录。

### 6.6.3 Weight Standardisation for Cross-Domain Comparison | 跨领域比较时的权重标准化方法

Where ranking results from different domains are compared or aggregated, the following standardisation rules shall apply:

当不同领域的排名结果进行比较或聚合时，以下标准化规则应适用：

a) Weights shall be normalised to a common scale (summing to 1) before comparison.

权重应在比较前归一化到共同尺度（总和为1）。

b) The weight determination method shall be the same or equivalent in terms of methodological rigour. Where methods differ, the comparison shall note this limitation.

权重确定方法在方法论严谨性方面应相同或等价。当方法不同时，比较应注明此局限性。

c) Cross-domain comparison shall not be used to imply that entities ranked in different domains are directly comparable on the same scale.

跨领域比较不应用于暗示不同领域中被排名的实体在同一尺度上直接可比。

> **Note**: Cross-domain comparison of ranking results requires careful interpretation. Differences in indicator systems, data availability, and domain conventions may limit the meaningfulness of such comparisons, even when weight standardisation is applied.
>
> **注**：排名结果的跨领域比较需要谨慎解读。指标体系、数据可得性和领域惯例的差异可能限制此类比较的意义，即使已应用权重标准化。
