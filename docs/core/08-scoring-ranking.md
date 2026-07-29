# Chapter 8: Scoring and Ranking Methods | 第8章 评分与排序方法

**ICO Std 2002:2026 — Chapter 8**

---

This chapter specifies the methods for scoring, normalising, aggregating, and ranking entities in a ranking system. It establishes requirements for the selection and documentation of scoring functions, the handling of ties and uncertainty, the verification of ranking results, and the standard format for ranking publication.

本章规定了排名系统中评分、归一化、聚合和排序实体的方法。它确立了评分函数的选择和记录要求、并列和不确定性的处理、排名结果的验证以及排名发布的标准格式。

---

## 8.1 Scoring Methods | 评分方法

The ranking entity shall select a scoring method appropriate to the nature of the indicator and the ranking purpose. The following methods are recognised:

排名实体应选择适合指标性质和排名目的的评分方法。认可以下方法：

### 8.1.1 Linear Scoring | 线性评分

Linear scoring transforms the raw indicator value into a score through a linear function.

线性评分通过线性函数将原始指标值转换为得分。

For a raw value *x* with defined minimum *x_min* and maximum *x_max*:

对于具有定义的最小值 *x_min* 和最大值 *x_max* 的原始值 *x*：

**Positive direction (higher is better)** | **正向指标（越高越好）**:

$$S(x) = \frac{x - x_{\min}}{x_{\max} - x_{\min}} \times S_{\text{range}} + S_{\min}$$

**Negative direction (lower is better)** | **负向指标（越低越好）**:

$$S(x) = \frac{x_{\max} - x}{x_{\max} - x_{\min}} \times S_{\text{range}} + S_{\min}$$

where $S_{\text{range}} = S_{\max} - S_{\min}$ is the score range.

其中 $S_{\text{range}} = S_{\max} - S_{\min}$ 为得分范围。

**Applicability**: Linear scoring is appropriate when the relationship between the raw value and the underlying construct is approximately linear.

**适用场景**：当原始值与底层构念之间的关系近似线性时，线性评分适用。

### 8.1.2 Piecewise Scoring | 分段评分

Piecewise scoring divides the range of raw values into segments and applies different scoring rules to each segment.

分段评分将原始值的范围划分为多个段，并对每个段适用不同的评分规则。

For a set of breakpoints $\{b_0, b_1, \ldots, b_k\}$ where $b_0 = x_{\min}$ and $b_k = x_{\max}$:

对于断点集合 $\{b_0, b_1, \ldots, b_k\}$，其中 $b_0 = x_{\min}$ 且 $b_k = x_{\max}$：

$$S(x) = S_j + \frac{x - b_j}{b_{j+1} - b_j} \times (S_{j+1} - S_j), \quad \text{for } b_j \leq x < b_{j+1}$$

where $S_j$ is the score assigned to breakpoint $b_j$.

其中 $S_j$ 为断点 $b_j$ 对应的得分。

**Applicability**: Piecewise scoring is appropriate when the marginal value of an additional unit of the indicator varies across the range (e.g., diminishing returns, threshold effects).

**适用场景**：当指标额外单位的边际价值在范围内变化时（如递减收益、阈值效应），分段评分适用。

The ranking entity shall document the rationale for the choice of breakpoints and the scores assigned to each segment.

排名实体应记录断点选择的理由及每个段分配的得分。

### 8.1.3 Percentile Ranking | 百分位排名

Percentile ranking converts raw values into percentile positions based on the empirical distribution.

百分位排名基于经验分布将原始值转换为百分位位置。

$$S(x) = \frac{\text{number of entities with value} \leq x}{m} \times 100$$

where *m* is the total number of ranked entities.

其中 *m* 为被排实体总数。

**Applicability**: Percentile ranking is appropriate when the absolute magnitude of the indicator is less meaningful than the relative position, or when the distribution is highly skewed.

**适用场景**：当指标的绝对量级不如相对位置有意义，或分布高度偏斜时，百分位排名适用。

> **Note**: Percentile ranking is non-linear and compresses the scale such that equal differences in percentile scores do not correspond to equal differences in the underlying attribute. The ranking entity shall disclose this property when percentile ranking is used.
>
> **注**：百分位排名是非线性的，会压缩尺度，使得百分位得分的等差并不对应底层属性的等差。当使用百分位排名时，排名实体应披露此性质。

### 8.1.4 Z-score Standardisation | Z-score 标准化

Z-score standardisation transforms raw values into standard deviation units from the mean.

Z-score标准化将原始值转换为偏离均值的标准差单位。

$$z_i = \frac{x_i - \bar{x}}{s}$$

where $\bar{x}$ is the sample mean and $s$ is the sample standard deviation.

其中 $\bar{x}$ 为样本均值，$s$ 为样本标准差。

**Applicability**: Z-score standardisation is appropriate when the indicator distribution is approximately normal and comparison across entities is based on relative deviation from the mean.

**适用场景**：当指标分布近似正态且实体间比较基于相对偏离均值的程度时，Z-score标准化适用。

**Limitation**: Z-scores can be negative, which may be problematic for certain aggregation methods (e.g., geometric mean). The ranking entity shall address this limitation when using Z-scores in conjunction with such aggregation methods.

**局限性**：Z-score可为负值，这可能对某些聚合方法（如几何平均）造成问题。当Z-score与此类聚合方法联合使用时，排名实体应解决此局限性。

### 8.1.5 T-score Standardisation | T-score 标准化

T-score standardisation transforms Z-scores to a scale with a mean of 50 and a standard deviation of 10.

T-score标准化将Z-score转换为均值为50、标准差为10的尺度。

$$T_i = 10 \times z_i + 50$$

**Applicability**: T-score standardisation is appropriate when positive scores are required and a standardised scale is desired. It preserves the ordinal properties of Z-scores while eliminating negative values (for typical distributions where |z| < 5).

**适用场景**：当需要正值得分且期望标准化尺度时，T-score标准化适用。它保留了Z-score的序数性质，同时消除了负值（对于|z| < 5的典型分布）。

---

## 8.2 Normalisation Methods | 归一化方法

Before aggregation, indicator values measured on different scales shall be normalised to a common scale. The ranking entity shall select a normalisation method appropriate to the data characteristics.

聚合前，以不同尺度测量的指标值应归一化到共同尺度。排名实体应选择适合数据特征的归一化方法。

### 8.2.1 Min-Max Normalisation | Min-Max 归一化

Min-Max normalisation rescales values to a fixed interval, typically [0, 1] or [0, 100].

Min-Max归一化将值重新缩放到固定区间，通常为[0, 1]或[0, 100]。

$$x'_i = \frac{x_i - x_{\min}}{x_{\max} - x_{\min}}$$

**Applicability**: Min-Max normalisation is appropriate when the minimum and maximum values are meaningful bounds and the distribution does not contain extreme outliers.

**适用场景**：当最小值和最大值是有意义的边界且分布不包含极端异常值时，Min-Max归一化适用。

**Limitation**: Min-Max normalisation is sensitive to outliers, as a single extreme value can compress the remainder of the distribution.

**局限性**：Min-Max归一化对异常值敏感，单一极端值可压缩分布的其余部分。

### 8.2.2 Z-score Normalisation | Z-score 归一化

Z-score normalisation (standardisation) transforms values to have a mean of 0 and a standard deviation of 1, as specified in 8.1.4.

Z-score归一化（标准化）将值转换为均值为0、标准差为1，如8.1.4所规定。

**Applicability**: Z-score normalisation is appropriate when indicators have different scales and units, and the comparison of relative positions is more important than absolute levels.

**适用场景**：当指标具有不同的尺度和单位，且相对位置的比较比绝对水平更重要时，Z-score归一化适用。

### 8.2.3 Decimal Scaling Normalisation | 小数定标归一化

Decimal scaling normalisation adjusts values by dividing by a power of 10.

小数定标归一化通过除以10的幂来调整值。

$$x'_i = \frac{x_i}{10^j}$$

where *j* is the smallest integer such that $\max(|x'_i|) < 1$.

其中 *j* 是使 $\max(|x'_i|) < 1$ 的最小整数。

**Applicability**: Decimal scaling is appropriate when the indicator values span several orders of magnitude and a simple, interpretable scaling is desired.

**适用场景**：当指标值跨越多个数量级且期望简单、可解释的缩放时，小数定标归一化适用。

### 8.2.4 Selection Criteria for Normalisation Methods | 归一化方法的选择依据

The ranking entity shall select the normalisation method based on the following criteria:

排名实体应基于以下准则选择归一化方法：

a) **Distributional characteristics** | **分布特征**: If the indicator distribution is approximately normal, Z-score normalisation is preferred. If the distribution is bounded and without significant outliers, Min-Max normalisation is preferred.

如果指标分布近似正态，优先选择Z-score归一化。如果分布有界且无显著异常值，优先选择Min-Max归一化。

b) **Outlier sensitivity** | **异常值敏感性**: If the indicator is prone to extreme outliers, Z-score normalisation or robust normalisation methods (e.g., median and MAD-based) should be used instead of Min-Max.

如果指标容易出现极端异常值，宜使用Z-score归一化或稳健归一化方法（如基于中位数和MAD的方法），而非Min-Max。

c) **Aggregation compatibility** | **聚合兼容性**: If the aggregation method requires non-negative inputs (e.g., geometric mean), a normalisation method that produces non-negative values shall be used, or the normalised values shall be shifted to a positive range.

如果聚合方法需要非负输入（如几何平均），应使用产生非负值的归一化方法，或将归一化值平移到正值范围。

d) **Interpretability** | **可解释性**: The chosen method should produce scores that are interpretable for the intended users of the ranking.

选择的方法应产生对排名预期用户可解释的得分。

The ranking entity shall document the normalisation method selected for each indicator and the rationale for the selection.

排名实体应记录每个指标选择的归一化方法及选择理由。

---

## 8.3 Composite Score Calculation | 综合评分计算

Composite scores aggregate normalised indicator scores into a single overall score for each ranked entity.

综合评分将归一化指标得分聚合为每个被排实体的单一总体得分。

### 8.3.1 Weighted Arithmetic Mean (WAM) | 加权求和法

The weighted arithmetic mean is the most common aggregation method:

加权算术平均是最常见的聚合方法：

$$C_i = \sum_{j=1}^{n} w_j \cdot s_{ij}$$

where $C_i$ is the composite score of entity *i*, $w_j$ is the weight of indicator *j*, and $s_{ij}$ is the normalised score of entity *i* on indicator *j*, subject to $\sum_{j=1}^{n} w_j = 1$.

其中 $C_i$ 为实体 *i* 的综合得分，$w_j$ 为指标 *j* 的权重，$s_{ij}$ 为实体 *i* 在指标 *j* 上的归一化得分，且 $\sum_{j=1}^{n} w_j = 1$。

**Applicability**: The WAM is appropriate when indicators are compensatory — i.e., a high score on one indicator can offset a low score on another.

**适用场景**：当指标具有补偿性时——即在某一指标上的高得分可以抵消另一指标上的低得分——WAM适用。

**Limitation**: The WAM allows full compensation between indicators, which may not be appropriate when all indicators represent essential conditions.

**局限性**：WAM允许指标间的完全补偿，当所有指标代表必要条件时可能不适当。

### 8.3.2 Weighted Geometric Mean | 加权几何平均法

The weighted geometric mean is:

加权几何平均为：

$$G_i = \prod_{j=1}^{n} s_{ij}^{w_j}$$

where $s_{ij} > 0$ for all *i* and *j*, and $\sum_{j=1}^{n} w_j = 1$.

其中 $s_{ij} > 0$ 对所有 *i* 和 *j* 成立，且 $\sum_{j=1}^{n} w_j = 1$。

**Applicability**: The weighted geometric mean is appropriate when:

加权几何平均在以下情况下适用：

a) indicators are non-compensatory or partially compensatory — i.e., a low score on any indicator significantly reduces the composite score;

指标是非补偿性或部分补偿性的——即任何指标的低得分显著降低综合得分；

b) indicators are measured as ratios or multiplicative factors;

指标以比率或乘法因子测量；

c) all indicator scores are strictly positive.

所有指标得分严格为正。

**Limitation**: The geometric mean requires all scores to be positive. It is more sensitive to low values than the arithmetic mean, which may be desirable or undesirable depending on the context.

**局限性**：几何平均要求所有得分为正。它对低值比算术平均更敏感，这取决于具体语境可能是期望的或不期望的。

### 8.3.3 Ordered Weighted Averaging (OWA) | 有序加权平均法

The OWA operator applies weights to the ordered values of indicators rather than to specific indicators:

OWA算子将权重应用于指标的有序值而非特定指标：

$$\text{OWA}_i = \sum_{j=1}^{n} v_j \cdot s_{i(j)}$$

where $s_{i(1)} \geq s_{i(2)} \geq \cdots \geq s_{i(n)}$ are the ordered scores of entity *i*, and $v_j$ are the order weights with $\sum_{j=1}^{n} v_j = 1$.

其中 $s_{i(1)} \geq s_{i(2)} \geq \cdots \geq s_{i(n)}$ 为实体 *i* 的有序得分，$v_j$ 为顺序权重，且 $\sum_{j=1}^{n} v_j = 1$。

**Applicability**: OWA is appropriate when the ranking entity wishes to control the degree of compensation between indicators by adjusting the order weights:

OWA在排名实体希望通过调整顺序权重来控制指标间补偿程度时适用：

a) Setting $v_1 = 1$ (all other $v_j = 0$) gives the maximum operator (optimistic aggregation).

设 $v_1 = 1$（所有其他 $v_j = 0$）得到最大值算子（乐观聚合）。

b) Setting $v_n = 1$ (all other $v_j = 0$) gives the minimum operator (pessimistic aggregation).

设 $v_n = 1$（所有其他 $v_j = 0$）得到最小值算子（悲观聚合）。

c) Setting $v_j = 1/n$ gives the arithmetic mean (full compensation).

设 $v_j = 1/n$ 得到算术平均（完全补偿）。

d) Setting $v_1 = v_n = 0.5$ gives the mid-range (average of best and worst).

设 $v_1 = v_n = 0.5$ 得到中程（最佳和最差的平均）。

### 8.3.4 Methodological Basis for Method Selection | 方法选择的方法论依据

The ranking entity shall document the methodological basis for selecting an aggregation method. The documentation shall include:

排名实体应记录选择聚合方法的方法论依据。文档应包括：

a) the theoretical relationship between the indicators (compensatory, non-compensatory, or partially compensatory);

指标间的理论关系（补偿性、非补偿性或部分补偿性）；

b) the nature of the ranking purpose (whether excellence in all dimensions is required or whether compensatory trade-offs are acceptable);

排名目的的性质（是否要求所有维度的卓越，或补偿性权衡是否可接受）；

c) the distributional properties of the indicator scores and their compatibility with the chosen method;

指标得分的分布性质及其与所选方法的兼容性；

d) the results of robustness testing comparing alternative aggregation methods.

比较替代聚合方法的稳健性测试结果。

---

## 8.4 Ranking Rules | 排序规则

### 8.4.1 Primary Ranking Rule | 主排序规则

Entities shall be ranked in descending order of their composite scores. The entity with the highest composite score shall receive rank 1.

实体应按其综合得分降序排列。综合得分最高的实体应获得第1名。

$$R_i = 1 + |\{k : C_k > C_i\}|$$

where $R_i$ is the rank of entity *i* and $|\{k : C_k > C_i\}|$ is the number of entities with composite scores strictly greater than $C_i$.

其中 $R_i$ 为实体 *i* 的排名，$|\{k : C_k > C_i\}|$ 为综合得分严格大于 $C_i$ 的实体数量。

### 8.4.2 Tie-Breaking Rules | 并列处理规则

When two or more entities have the same composite score, the following tie-breaking rules shall be applied in order:

当两个或多个实体具有相同综合得分时，应按顺序适用以下并列处理规则：

a) **Step 1 — Highest-weighted indicator** | **最高权重指标**: The entity with the higher score on the indicator with the greatest weight shall receive the higher rank.

在权重最大指标上得分较高的实体应获得较高排名。

b) **Step 2 — Second-highest-weighted indicator** | **次高权重指标**: If the tie persists, the entity with the higher score on the indicator with the second-greatest weight shall receive the higher rank.

如并列持续，在权重第二大的指标上得分较高的实体应获得较高排名。

c) **Step 3 — Sequential application** | **顺序适用**: Steps 1 and 2 shall be repeated, proceeding through indicators in descending order of weight, until the tie is resolved.

应重复步骤1和2，按权重降序遍历指标，直至并列解决。

d) **Step 4 — Shared rank** | **并列排名**: If the tie cannot be resolved after applying all indicators, the tied entities shall share the same rank. The next rank(s) shall be skipped accordingly (e.g., if two entities share rank 5, the next entity receives rank 7).

如果在适用所有指标后仍无法解决并列，并列实体应共享相同排名。下一个排名应相应跳过（如两个实体并列第5名，下一个实体获得第7名）。

The tie-breaking procedure shall be documented in the methodology and disclosed in the ranking publication.

并列处理程序应在方法论中记录并在排名发布中披露。

### 8.4.3 Ranking Intervals and Confidence Intervals | 排名区间与置信区间

The ranking entity should report uncertainty in the ranking positions, which may include:

排名实体宜报告排名位置的不确定性，可包括：

a) **Ranking intervals** | **排名区间**: A range of ranks within which an entity's true rank is expected to fall, given the uncertainty in the data and methodology.

排名区间：给定数据和方法论的不确定性，实体真实排名预期落入的排名范围。

b) **Confidence intervals** | **置信区间**: Statistical confidence intervals for composite scores, estimated through methods such as bootstrapping.

综合得分的统计置信区间，通过自助法等方法估计。

$$\hat{C}_i \pm z_{\alpha/2} \cdot \hat{\text{se}}(\hat{C}_i)$$

where $\hat{\text{se}}(\hat{C}_i)$ is the estimated standard error of the composite score, typically obtained through bootstrap resampling.

其中 $\hat{\text{se}}(\hat{C}_i)$ 为综合得分的估计标准误，通常通过自助重抽样获得。

c) **Overlap reporting** | **重叠报告**: The ranking entity should identify and report entities whose confidence intervals overlap, indicating that their rank differences are not statistically meaningful.

排名实体宜识别并报告置信区间重叠的实体，表明其排名差异不具有统计意义。

> **Note**: Ranking intervals and confidence intervals are particularly important for rankings that influence significant decisions (e.g., funding allocation, regulatory classification). Where such intervals are not reported, the ranking entity shall disclose this limitation.
>
> **注**：排名区间和置信区间对于影响重大决策的排名（如资金分配、监管分类）尤为重要。当未报告此类区间时，排名实体应披露此局限性。

---

## 8.5 Ranking Result Verification | 排名结果验证

The ranking entity shall verify the ranking results before publication using the methods specified in 8.5.1 through 8.5.3.

排名实体应在发布前使用8.5.1至8.5.3规定的方法验证排名结果。

### 8.5.1 Internal Consistency Check | 内部一致性检验

Internal consistency assesses whether the indicators in the ranking system measure a coherent underlying construct.

内部一致性评估排名系统中的指标是否衡量了一致的基础构念。

a) **Cronbach's alpha** | **克朗巴赫α**: For ranking systems where indicators are expected to be correlated, Cronbach's alpha shall be computed:

对于指标预期相关的排名系统，应计算克朗巴赫α：

$$\alpha = \frac{n}{n - 1} \left(1 - \frac{\sum_{j=1}^{n} s_j^2}{s_{\text{total}}^2}\right)$$

where *n* is the number of indicators, $s_j^2$ is the variance of indicator *j*, and $s_{\text{total}}^2$ is the variance of the total (sum) score.

其中 *n* 为指标数量，$s_j^2$ 为指标 *j* 的方差，$s_{\text{total}}^2$ 为总（和）得分的方差。

b) **Threshold**: A Cronbach's alpha of at least 0.70 shall be achieved for the overall indicator system. Where the alpha is below 0.70, the ranking entity shall investigate the cause and consider indicator revision.

整体指标系统应达到至少0.70的克朗巴赫α。当α低于0.70时，排名实体应调查原因并考虑指标修订。

c) **Item-total correlation**: Each indicator's correlation with the total score (corrected for overlap) shall be reported. Indicators with corrected item-total correlation below 0.30 should be reviewed for potential removal.

应报告每个指标与总得分的相关性（经重叠校正）。校正项总相关性低于0.30的指标宜进行审查以考虑移除。

### 8.5.2 External Validity Check | 外部效度检验

External validity assesses whether the ranking results are consistent with external benchmarks or criteria.

外部效度评估排名结果是否与外部基准或准则一致。

a) The ranking entity should compare the ranking results with at least one independent external benchmark, where such a benchmark exists.

排名实体宜将排名结果与至少一个独立的外部基准进行比较，当此类基准存在时。

b) The comparison method shall be documented, including the choice of benchmark, the correlation measure used (e.g., Spearman's ρ, Kendall's τ), and the interpretation of the results.

比较方法应予以记录，包括基准的选择、使用的相关性度量（如Spearman ρ、Kendall τ）以及结果的解释。

c) Where no suitable external benchmark exists, the ranking entity shall document this and shall instead rely on the internal consistency and robustness checks.

当不存在合适的外部基准时，排名实体应记录此情况，并应转而依赖内部一致性和稳健性检查。

### 8.5.3 Robustness Check | 稳健性检验

Robustness checks assess whether the ranking results are stable under methodological variations.

稳健性检查评估排名结果在方法论变化下是否稳定。

The ranking entity shall conduct at least the following robustness checks:

排名实体应至少进行以下稳健性检查：

a) **Bootstrap resampling** | **自助重抽样**: The ranking shall be recomputed on a large number (at least 1 000) of bootstrap samples drawn with replacement from the original data. For each entity, the following shall be reported:

排名应在从原始数据有放回抽取的大量（至少1000个）自助样本上重新计算。对每个实体，应报告：

1) the mean rank across bootstrap samples;

自助样本中的平均排名；

2) the standard deviation of the rank across bootstrap samples;

自助样本中排名的标准差；

3) the proportion of bootstrap samples in which the entity's rank falls within ±5 positions of the published rank.

实体排名在自助样本中落在发布排名±5位以内的比例。

b) **Method variation test** | **方法变异测试**: The ranking shall be recomputed using at least one alternative aggregation method (e.g., if WAM is the primary method, geometric mean shall be tested as an alternative). The correlation between the primary and alternative rankings shall be reported.

排名应使用至少一种替代聚合方法重新计算（如WAM为主要方法，应以几何平均作为替代进行测试）。主要排名和替代排名之间的相关性应予以报告。

c) **Data perturbation test** | **数据扰动测试**: The ranking shall be recomputed after adding random noise (within the estimated measurement error range) to the input data. The stability of the ranking shall be assessed.

应在向输入数据添加随机噪声（在估计的测量误差范围内）后重新计算排名。排名的稳定性应予以评估。

---

## 8.6 Ranking Publication Format | 排名发布格式

### 8.6.1 Standard Ranking Table Format | 标准排名表格式

The ranking shall be published in a tabular format that includes, at a minimum, the following columns:

排名应以表格格式发布，至少包括以下列：

| Column | Description |
|--------|-------------|
| Rank | The ordinal position of the entity |
| Entity identifier | The name or code of the ranked entity |
| Composite score | The overall composite score of the entity |
| Indicator scores | The score of the entity on each Level 1 indicator |

| 列 | 描述 |
|---|---|
| 排名 | 实体的序数位置 |
| 实体标识 | 被排实体的名称或代码 |
| 综合得分 | 实体的总体综合得分 |
| 指标得分 | 实体在每项一级指标上的得分 |

### 8.6.2 Sub-Score Disclosure | 分项得分披露

In addition to the standard ranking table, the ranking entity shall disclose:

除标准排名表外，排名实体应披露：

a) the scores of each entity on all Level 2 indicators (sub-dimensions);

每个实体在所有二级指标（子维度）上的得分；

b) the normalised scores of each entity on all Level 3 indicators (specific measures), or the raw data from which these scores are derived.

每个实体在所有三级指标（具体度量）上的归一化得分，或导出这些得分的原始数据。

> **Note**: Disclosure of Level 3 indicator scores may be provided in supplementary materials (e.g., downloadable data files) rather than in the primary publication, where the number of indicators makes tabular presentation impractical.
>
> **注**：当指标数量使表格展示不切实际时，三级指标得分的披露可在补充材料（如可下载数据文件）中提供，而非在主要发布中。

### 8.6.3 Methodology Summary Accompaniment | 方法论摘要伴随要求

Each ranking publication shall be accompanied by a methodology summary that includes:

每次排名发布应附带方法论摘要，包括：

a) the standard identifier and version (e.g., ICO Std 2002:2026, Chapter 8, Version 1.0);

标准标识符和版本（如ICO Std 2002:2026，第8章，版本1.0）；

b) a brief description of the scoring method(s) used;

所用评分方法的简要描述；

c) a brief description of the normalisation method(s) used;

所用归一化方法的简要描述；

d) a brief description of the aggregation method used;

所用聚合方法的简要描述；

e) the total number of ranked entities and the number of entities excluded from the ranking, with reasons for exclusion;

被排实体总数及排除出排名的实体数量及排除原因；

f) a reference to the full methodology documentation;

完整方法论文件的引用；

g) the date of publication;

发布日期；

h) the contact information for the ranking entity.

排名实体的联系信息。

> **Note**: The purpose of the methodology summary is to enable users to understand the key methodological choices without reading the full documentation. The summary does not replace the full methodology disclosure required by 4.2.1.
>
> **注**：方法论摘要的目的是使用户无需阅读完整文件即可了解关键方法论选择。摘要不替代4.2.1要求的完整方法论披露。

---

> **Note**: The scoring and ranking methods specified in this chapter are intended to be domain-independent. Domain-specific scoring adjustments (e.g., industry-specific benchmarks, regional normalisation) shall be defined in the relevant extension module and shall comply with the core-layer requirements specified herein.
>
> **注**：本章规定的评分和排序方法旨在领域无关。领域特定评分调整（如行业特定基准、区域归一化）应在相关扩展模块中定义，并应遵守本文件规定的核心层要求。
