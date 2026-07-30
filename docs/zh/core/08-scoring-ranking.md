> **ICO Std 2002:2026 — 中文版 — 第8章 评分与排序方法**

# 第8章 评分与排序方法

---

本章规定了排名系统中评分、归一化、聚合和排序实体的方法。它确立了评分函数的选择和记录要求、并列和不确定性的处理、排名结果的验证以及排名发布的标准格式。

---

## 评分方法

排名实体应选择适合指标性质和排名目的的评分方法。认可以下方法：

### 线性评分

线性评分通过线性函数将原始指标值转换为得分。

对于具有定义的最小值 *x_min* 和最大值 *x_max* 的原始值 *x*：

**正向指标（越高越好）**:

**负向指标（越低越好）**:

其中 $S_{\text{range}} = S_{\max} - S_{\min}$ 为得分范围。

**适用场景**：当原始值与底层构念之间的关系近似线性时，线性评分适用。

### 分段评分

分段评分将原始值的范围划分为多个段，并对每个段适用不同的评分规则。

对于断点集合 $\{b_0, b_1, \ldots, b_k\}$，其中 $b_0 = x_{\min}$ 且 $b_k = x_{\max}$：

其中 $S_j$ 为断点 $b_j$ 对应的得分。

**适用场景**：当指标额外单位的边际价值在范围内变化时（如递减收益、阈值效应），分段评分适用。

排名实体应记录断点选择的理由及每个段分配的得分。

### 百分位排名

百分位排名基于经验分布将原始值转换为百分位位置。

其中 *m* 为被排实体总数。

**适用场景**：当指标的绝对量级不如相对位置有意义，或分布高度偏斜时，百分位排名适用。

> **注**：百分位排名是非线性的，会压缩尺度，使得百分位得分的等差并不对应底层属性的等差。当使用百分位排名时，排名实体应披露此性质。

### Z-score 标准化

Z-score标准化将原始值转换为偏离均值的标准差单位。

其中 $\bar{x}$ 为样本均值，$s$ 为样本标准差。

**适用场景**：当指标分布近似正态且实体间比较基于相对偏离均值的程度时，Z-score标准化适用。

**局限性**：Z-score可为负值，这可能对某些聚合方法（如几何平均）造成问题。当Z-score与此类聚合方法联合使用时，排名实体应解决此局限性。

### T-score 标准化

T-score标准化将Z-score转换为均值为50、标准差为10的尺度。

**适用场景**：当需要正值得分且期望标准化尺度时，T-score标准化适用。它保留了Z-score的序数性质，同时消除了负值（对于|z| < 5的典型分布）。

---

## 归一化方法

聚合前，以不同尺度测量的指标值应归一化到共同尺度。排名实体应选择适合数据特征的归一化方法。

### Min-Max 归一化

Min-Max归一化将值重新缩放到固定区间，通常为[0, 1]或[0, 100]。

**适用场景**：当最小值和最大值是有意义的边界且分布不包含极端异常值时，Min-Max归一化适用。

**局限性**：Min-Max归一化对异常值敏感，单一极端值可压缩分布的其余部分。

### Z-score 归一化

Z-score归一化（标准化）将值转换为均值为0、标准差为1，如8.1.4所规定。

**适用场景**：当指标具有不同的尺度和单位，且相对位置的比较比绝对水平更重要时，Z-score归一化适用。

### 小数定标归一化

小数定标归一化通过除以10的幂来调整值。

其中 *j* 是使 $\max(|x'_i|) < 1$ 的最小整数。

**适用场景**：当指标值跨越多个数量级且期望简单、可解释的缩放时，小数定标归一化适用。

### 归一化方法的选择依据

排名实体应基于以下准则选择归一化方法：

a) **分布特征**: If the indicator distribution is approximately normal, Z-score normalisation is preferred. If the distribution is bounded and without significant outliers, Min-Max normalisation is preferred.

如果指标分布近似正态，优先选择Z-score归一化。如果分布有界且无显著异常值，优先选择Min-Max归一化。

b) **异常值敏感性**: If the indicator is prone to extreme outliers, Z-score normalisation or robust normalisation methods (e.g., median and MAD-based) should be used instead of Min-Max.

如果指标容易出现极端异常值，宜使用Z-score归一化或稳健归一化方法（如基于中位数和MAD的方法），而非Min-Max。

c) **聚合兼容性**: If the aggregation method requires non-negative inputs (e.g., geometric mean), a normalisation method that produces non-negative values shall be used, or the normalised values shall be shifted to a positive range.

如果聚合方法需要非负输入（如几何平均），应使用产生非负值的归一化方法，或将归一化值平移到正值范围。

d) **可解释性**: The chosen method should produce scores that are interpretable for the intended users of the ranking.

选择的方法应产生对排名预期用户可解释的得分。

排名实体应记录每个指标选择的归一化方法及选择理由。

---

## 综合评分计算

综合评分将归一化指标得分聚合为每个被排实体的单一总体得分。

### 加权求和法

加权算术平均是最常见的聚合方法：

其中 $C_i$ 为实体 *i* 的综合得分，$w_j$ 为指标 *j* 的权重，$s_{ij}$ 为实体 *i* 在指标 *j* 上的归一化得分，且 $\sum_{j=1}^{n} w_j = 1$。

**适用场景**：当指标具有补偿性时——即在某一指标上的高得分可以抵消另一指标上的低得分——WAM适用。

**局限性**：WAM允许指标间的完全补偿，当所有指标代表必要条件时可能不适当。

### 加权几何平均法

加权几何平均为：

其中 $s_{ij} > 0$ 对所有 *i* 和 *j* 成立，且 $\sum_{j=1}^{n} w_j = 1$。

加权几何平均在以下情况下适用：

指标是非补偿性或部分补偿性的——即任何指标的低得分显著降低综合得分；

指标以比率或乘法因子测量；

所有指标得分严格为正。

**局限性**：几何平均要求所有得分为正。它对低值比算术平均更敏感，这取决于具体语境可能是期望的或不期望的。

### 有序加权平均法

OWA算子将权重应用于指标的有序值而非特定指标：

其中 $s_{i(1)} \geq s_{i(2)} \geq \cdots \geq s_{i(n)}$ 为实体 *i* 的有序得分，$v_j$ 为顺序权重，且 $\sum_{j=1}^{n} v_j = 1$。

OWA在排名实体希望通过调整顺序权重来控制指标间补偿程度时适用：

设 $v_1 = 1$（所有其他 $v_j = 0$）得到最大值算子（乐观聚合）。

设 $v_n = 1$（所有其他 $v_j = 0$）得到最小值算子（悲观聚合）。

设 $v_j = 1/n$ 得到算术平均（完全补偿）。

设 $v_1 = v_n = 0.5$ 得到中程（最佳和最差的平均）。

### 方法选择的方法论依据

排名实体应记录选择聚合方法的方法论依据。文档应包括：

指标间的理论关系（补偿性、非补偿性或部分补偿性）；

排名目的的性质（是否要求所有维度的卓越，或补偿性权衡是否可接受）；

指标得分的分布性质及其与所选方法的兼容性；

比较替代聚合方法的稳健性测试结果。

---

## 排序规则

### 主排序规则

实体应按其综合得分降序排列。综合得分最高的实体应获得第1名。

其中 $R_i$ 为实体 *i* 的排名，$|\{k : C_k > C_i\}|$ 为综合得分严格大于 $C_i$ 的实体数量。

### 并列处理规则

当两个或多个实体具有相同综合得分时，应按顺序适用以下并列处理规则：

a) **最高权重指标**: The entity with the higher score on the indicator with the greatest weight shall receive the higher rank.

在权重最大指标上得分较高的实体应获得较高排名。

b) **次高权重指标**: If the tie persists, the entity with the higher score on the indicator with the second-greatest weight shall receive the higher rank.

如并列持续，在权重第二大的指标上得分较高的实体应获得较高排名。

c) **顺序适用**: Steps 1 and 2 shall be repeated, proceeding through indicators in descending order of weight, until the tie is resolved.

应重复步骤1和2，按权重降序遍历指标，直至并列解决。

d) **并列排名**: If the tie cannot be resolved after applying all indicators, the tied entities shall share the same rank. The next rank(s) shall be skipped accordingly (e.g., if two entities share rank 5, the next entity receives rank 7).

如果在适用所有指标后仍无法解决并列，并列实体应共享相同排名。下一个排名应相应跳过（如两个实体并列第5名，下一个实体获得第7名）。

并列处理程序应在方法论中记录并在排名发布中披露。

### 排名区间与置信区间

排名实体宜报告排名位置的不确定性，可包括：

a) **排名区间**: A range of ranks within which an entity's true rank is expected to fall, given the uncertainty in the data and methodology.

排名区间：给定数据和方法论的不确定性，实体真实排名预期落入的排名范围。

b) **置信区间**: Statistical confidence intervals for composite scores, estimated through methods such as bootstrapping.

综合得分的统计置信区间，通过自助法等方法估计。

其中 $\hat{\text{se}}(\hat{C}_i)$ 为综合得分的估计标准误，通常通过自助重抽样获得。

c) **重叠报告**: The ranking entity should identify and report entities whose confidence intervals overlap, indicating that their rank differences are not statistically meaningful.

排名实体宜识别并报告置信区间重叠的实体，表明其排名差异不具有统计意义。

> **注**：排名区间和置信区间对于影响重大决策的排名（如资金分配、监管分类）尤为重要。当未报告此类区间时，排名实体应披露此局限性。

---

## 排名结果验证

排名实体应在发布前使用8.5.1至8.5.3规定的方法验证排名结果。

### 内部一致性检验

内部一致性评估排名系统中的指标是否衡量了一致的基础构念。

a) **克朗巴赫α**: For ranking systems where indicators are expected to be correlated, Cronbach's alpha shall be computed:

对于指标预期相关的排名系统，应计算克朗巴赫α：

其中 *n* 为指标数量，$s_j^2$ 为指标 *j* 的方差，$s_{\text{total}}^2$ 为总（和）得分的方差。

整体指标系统应达到至少0.70的克朗巴赫α。当α低于0.70时，排名实体应调查原因并考虑指标修订。

应报告每个指标与总得分的相关性（经重叠校正）。校正项总相关性低于0.30的指标宜进行审查以考虑移除。

### 外部效度检验

外部效度评估排名结果是否与外部基准或准则一致。

排名实体宜将排名结果与至少一个独立的外部基准进行比较，当此类基准存在时。

比较方法应予以记录，包括基准的选择、使用的相关性度量（如Spearman ρ、Kendall τ）以及结果的解释。

当不存在合适的外部基准时，排名实体应记录此情况，并应转而依赖内部一致性和稳健性检查。

### 稳健性检验

稳健性检查评估排名结果在方法论变化下是否稳定。

排名实体应至少进行以下稳健性检查：

a) **自助重抽样**: The ranking shall be recomputed on a large number (at least 1 000) of bootstrap samples drawn with replacement from the original data. For each entity, the following shall be reported:

排名应在从原始数据有放回抽取的大量（至少1000个）自助样本上重新计算。对每个实体，应报告：

自助样本中的平均排名；

自助样本中排名的标准差；

实体排名在自助样本中落在发布排名±5位以内的比例。

b) **方法变异测试**: The ranking shall be recomputed using at least one alternative aggregation method (e.g., if WAM is the primary method, geometric mean shall be tested as an alternative). The correlation between the primary and alternative rankings shall be reported.

排名应使用至少一种替代聚合方法重新计算（如WAM为主要方法，应以几何平均作为替代进行测试）。主要排名和替代排名之间的相关性应予以报告。

c) **数据扰动测试**: The ranking shall be recomputed after adding random noise (within the estimated measurement error range) to the input data. The stability of the ranking shall be assessed.

应在向输入数据添加随机噪声（在估计的测量误差范围内）后重新计算排名。排名的稳定性应予以评估。

---

## 排名发布格式

### 标准排名表格式

排名应以表格格式发布，至少包括以下列：

| 列 | 描述 |
| 排名 | 实体的序数位置 |
| 实体标识 | 被排实体的名称或代码 |
| 综合得分 | 实体的总体综合得分 |
| 指标得分 | 实体在每项一级指标上的得分 |

### 分项得分披露

除标准排名表外，排名实体应披露：

每个实体在所有二级指标（子维度）上的得分；

每个实体在所有三级指标（具体度量）上的归一化得分，或导出这些得分的原始数据。

> **注**：当指标数量使表格展示不切实际时，三级指标得分的披露可在补充材料（如可下载数据文件）中提供，而非在主要发布中。

### 方法论摘要伴随要求

每次排名发布应附带方法论摘要，包括：

标准标识符和版本（如ICO Std 2002:2026，第8章，版本1.0）；

所用评分方法的简要描述；

所用归一化方法的简要描述；

所用聚合方法的简要描述；

被排实体总数及排除出排名的实体数量及排除原因；

完整方法论文件的引用；

发布日期；

排名实体的联系信息。

> **注**：方法论摘要的目的是使用户无需阅读完整文件即可了解关键方法论选择。摘要不替代4.2.1要求的完整方法论披露。

---

> **注**：本章规定的评分和排序方法旨在领域无关。领域特定评分调整（如行业特定基准、区域归一化）应在相关扩展模块中定义，并应遵守本文件规定的核心层要求。