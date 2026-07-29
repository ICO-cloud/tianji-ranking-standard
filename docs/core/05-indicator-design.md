# Chapter 5: Indicator System Design | 第5章 指标体系设计

**ICO Std 2002:2026 — Chapter 5**

---

This chapter specifies the requirements for designing indicator systems used in ranking methodologies. It establishes rules for indicator selection, hierarchical organisation, validity verification, initial weight assignment, update mechanisms, and the relationship between core-layer and extension-layer indicators.

本章规定了排名方法论中指标体系设计的要求。它确立了指标选取、层级组织、有效性验证、权重初设、更新机制以及核心层与扩展层指标关系的规则。

---

## 5.1 Indicator Selection Criteria | 指标选取规则

Each indicator included in a ranking system shall satisfy the criteria specified in 5.1.1 through 5.1.5. The ranking entity shall document the justification for each indicator's inclusion with reference to these criteria.

排名系统中纳入的每个指标应满足5.1.1至5.1.5规定的准则。排名实体应参照这些准则记录每个指标纳入的理由。

### 5.1.1 Relevance | 相关性

An indicator shall be directly relevant to the ranking purpose as defined in the methodology. Relevance shall be established by demonstrating a logical or empirical link between the indicator and the attribute being measured.

指标应与方法论中定义的排名目的直接相关。相关性应通过证明指标与被衡量属性之间的逻辑或实证联系来确立。

a) The ranking entity shall define the conceptual domain that the ranking is intended to measure.

排名实体应定义排名旨在衡量的概念域。

b) Each indicator shall map to at least one defined concept within that domain.

每个指标应映射到该域内至少一个已定义概念。

c) Indicators that are included solely due to data availability, without a demonstrated link to the ranking purpose, shall not be used.

仅因数据可得性而纳入、与排名目的无已证联系的指标不应使用。

### 5.1.2 Measurability | 可量化性

An indicator shall be measurable, either through quantitative measurement or through a defined coding scheme that permits consistent qualitative assessment.

指标应可通过定量测量或通过允许一致性定性评估的已定义编码方案进行量化。

a) Quantitative indicators shall have a defined unit of measurement and an unambiguous operational definition.

定量指标应具有定义的计量单位和明确的操作定义。

b) Qualitative indicators shall have a defined coding scheme with clearly distinguishable levels and coding rules.

定性指标应具有定义的编码方案，包含清晰可辨的等级和编码规则。

c) Indicators for which no reliable measurement or coding procedure exists shall not be included until such a procedure is developed and validated.

不存在可靠测量或编码程序的指标，在程序开发和验证之前不应纳入。

### 5.1.3 Data Availability | 可获得性

Data required for an indicator shall be obtainable from accessible sources within a reasonable timeframe and at a reasonable cost, as specified in Chapter 7.

指标所需数据应能从可访问的来源在合理时间范围和合理成本内获取，如第7章所规定。

a) The ranking entity shall assess the availability of data for each proposed indicator before inclusion.

排名实体应在纳入前评估每个候选指标的数据可得性。

b) Where data availability varies significantly across ranked entities, the ranking entity shall evaluate whether the indicator introduces systematic bias (see 4.7).

当数据可得性在被排实体间差异显著时，排名实体应评估指标是否引入系统性偏见（见4.7）。

### 5.1.4 Independence | 独立性

Indicators within the same level of the hierarchy shall exhibit low mutual redundancy. The ranking entity shall assess the inter-correlation among indicators and take measures to reduce redundancy.

同一层级内的指标应表现出低互冗余性。排名实体应评估指标间的相互相关性并采取措施减少冗余。

a) The pairwise correlation between indicators at the same hierarchical level shall be examined. Where the absolute value of the correlation coefficient exceeds 0.80, the ranking entity shall consider:

应检查同一层级指标间的配对相关性。当相关系数的绝对值超过0.80时，排名实体应考虑：

1) merging the correlated indicators into a single composite indicator;

将相关指标合并为单一复合指标；

2) removing one of the correlated indicators;

移除其中一个相关指标；

3) retaining both indicators with documented justification for their separate inclusion.

保留两个指标并记录其分别纳入的理由。

b) Multicollinearity among indicators shall be assessed using appropriate methods (e.g., variance inflation factor). Indicators with a variance inflation factor (VIF) exceeding 10 should be reviewed for potential removal or consolidation.

应使用适当方法（如方差膨胀因子）评估指标间的多重共线性。方差膨胀因子（VIF）超过10的指标宜进行审查，以考虑移除或合并。

### 5.1.5 Robustness | 稳健性

An indicator shall be robust against the influence of outliers and measurement errors. The ranking entity shall:

指标应对异常值和测量误差的影响具有稳健性。排名实体应：

a) test each indicator's sensitivity to outliers using appropriate methods (e.g., influence functions, trimmed means);

使用适当方法（如影响函数、截尾均值）测试每个指标对异常值的敏感性；

b) document the outlier handling procedure for each indicator (see also 7.4.2);

记录每个指标的异常值处理程序（另见7.4.2）；

c) exclude indicators whose results are dominated by a small number of extreme observations, unless the extreme observations are substantively meaningful.

排除结果由少量极端观测值主导的指标，除非极端观测值具有实质意义。

---

## 5.2 Indicator Hierarchy | 指标层级结构

The indicator system shall be organised into a hierarchical structure that reflects the logical decomposition of the ranking purpose into measurable components.

指标体系应组织为层级结构，反映排名目的向可测量组分的逻辑分解。

### 5.2.1 Hierarchical Levels | 层级定义

The indicator hierarchy shall consist of the following levels:

指标层级应由以下层级组成：

a) **Level 1 — Dimensions** | **一级指标（维度）**: The broadest categories representing the major aspects of the ranking purpose. Level 1 indicators define the structural framework of the indicator system.

代表排名目的主要方面的最广泛类别。一级指标定义指标体系的结构框架。

b) **Level 2 — Sub-dimensions** | **二级指标（子维度）**: More specific components within each dimension. Level 2 indicators decompose the dimensions into measurable aspects.

每个维度内更具体的组分。二级指标将维度分解为可测量的方面。

c) **Level 3 — Specific measures** | **三级指标（具体度量）**: The most granular, directly measurable variables. Level 3 indicators are the operationalised variables for which data is collected.

最精细的、可直接测量的变量。三级指标是采集数据的操作化变量。

### 5.2.2 Hierarchy Depth | 层级深度

The indicator hierarchy shall not exceed three levels. Where a ranking purpose requires more granular decomposition, the ranking entity shall:

指标层级不应超过三层。当排名目的需要更精细的分解时，排名实体应：

a) consolidate the lower-level indicators into Level 3 composite measures; or

将较低层级指标整合为三级复合度量；或

b) document the justification for exceeding three levels and obtain peer review approval (see 4.5.4).

记录超过三层的理由并获得同行评审批准（见4.5.4）。

### 5.2.3 Logical Relationships Between Levels | 层级间的逻辑关系

The relationship between indicators at adjacent levels shall be clearly defined:

相邻层级指标间的关系应明确定义：

a) Each Level 1 indicator shall be decomposable into at least two Level 2 indicators.

每个一级指标应可分解为至少两个二级指标。

b) Each Level 2 indicator shall be decomposable into at least two Level 3 indicators.

每个二级指标应可分解为至少两个三级指标。

c) The set of Level 2 indicators under a given Level 1 indicator shall collectively cover the conceptual scope of that Level 1 indicator.

给定一级指标下的二级指标集合应共同覆盖该一级指标的概念范围。

d) The aggregation rule from lower to higher levels shall be specified (see Chapter 6 and Chapter 8).

从较低层级到较高层级的聚合规则应予以规定（见第6章和第8章）。

---

## 5.3 Indicator Validity Verification | 指标有效性验证

The ranking entity shall verify the validity of the indicator system before the first application and following any significant revision. Validity verification shall address the dimensions specified in 5.3.1 through 5.3.3.

排名实体应在首次应用前及任何重大修订后验证指标体系的有效性。有效性验证应涉及5.3.1至5.3.3规定的维度。

### 5.3.1 Content Validity | 内容效度

Content validity assesses whether the indicator system adequately covers the conceptual domain it is intended to measure.

内容效度评估指标体系是否充分覆盖其旨在衡量的概念域。

a) The ranking entity shall define the conceptual domain and its boundaries.

排名实体应定义概念域及其边界。

b) A panel of at least three domain experts shall evaluate whether the indicator system provides comprehensive coverage of the defined domain.

至少三名领域专家组成的小组应评估指标体系是否对定义的域提供全面覆盖。

c) Gaps identified by the expert panel shall be addressed by adding indicators, revising existing indicators, or documenting the limitation.

专家小组识别的缺口应通过增加指标、修订现有指标或记录局限性来解决。

### 5.3.2 Construct Validity | 结构效度

Construct validity assesses whether the indicators measure the theoretical constructs they are intended to measure.

结构效度评估指标是否测量了其旨在测量的理论构念。

a) The ranking entity shall apply appropriate statistical methods to assess construct validity, which may include:

排名实体应采用适当的统计方法评估结构效度，可包括：

1) exploratory or confirmatory factor analysis to examine whether indicators load onto the expected dimensions;

探索性或验证性因子分析，以检查指标是否载荷到预期维度；

2) convergent validity analysis to assess whether indicators that should be related are in fact correlated;

收敛效度分析，以评估应相关的指标是否实际相关；

3) discriminant validity analysis to assess whether indicators that should be distinct are in fact uncorrelated.

区分效度分析，以评估应有区别的指标是否实际不相关。

b) The results of construct validity analyses shall be documented, including any indicators that fail to conform to the expected structure and the actions taken.

结构效度分析的结果应予以记录，包括任何不符合预期结构的指标及所采取的行动。

### 5.3.3 Criterion Validity | 效标效度

Where an external criterion or gold standard exists, the ranking entity should assess criterion validity by examining the correlation between the ranking results and the external criterion.

当存在外部准则或金标准时，排名实体宜通过检验排名结果与外部准则之间的相关性来评估效标效度。

a) The external criterion shall be independent of the ranking system being validated.

外部准则应独立于被验证的排名系统。

b) The ranking entity shall document the choice of external criterion and the rationale for its selection.

排名实体应记录外部准则的选择及其选择理由。

c) Where no suitable external criterion exists, the ranking entity shall document this limitation and the alternative validation methods employed.

当不存在合适的外部准则时，排名实体应记录此局限性及所采用的替代验证方法。

### 5.3.4 Validation Documentation | 验证文档化

The results of all validity verification analyses shall be documented in the methodology report. The documentation shall include:

所有有效性验证分析的结果应在方法论报告中记录。文档应包括：

a) the methods used and their assumptions;

使用的方法及其假设；

b) the data and sample on which the analysis was conducted;

进行分析所基于的数据和样本；

c) the results, including statistical test values and their interpretation;

结果，包括统计检验值及其解释；

d) any limitations identified and the actions taken to address them.

识别的任何局限性及为解决这些局限性所采取的行动。

---

## 5.4 Initial Weight Assignment | 指标权重初设

Prior to the formal weight determination process (see Chapter 6), the ranking entity shall establish an initial weight scheme. The initial weight scheme serves as a starting point for stakeholder consultation and sensitivity analysis.

在正式权重确定过程（见第6章）之前，排名实体应建立初始权重方案。初始权重方案作为利益相关方协商和敏感性分析的起点。

### 5.4.1 Equal Weighting | 等权法

Where no strong theoretical or empirical basis exists for differential weighting, the ranking entity shall use equal weighting as the initial scheme. Under equal weighting, all indicators at the same hierarchical level receive the same weight.

当不存在差异赋权的强理论或实证依据时，排名实体应使用等权法作为初始方案。在等权法下，同一层级的所有指标获得相同权重。

For *n* indicators at a given level, the equal weight for each indicator *i* is:

对于给定层级的 *n* 个指标，每个指标 *i* 的等权重为：

$$w_i = \frac{1}{n}, \quad i = 1, 2, \ldots, n$$

where $\sum_{i=1}^{n} w_i = 1$.

> **Note**: Equal weighting does not imply equal importance; it reflects the absence of a defensible basis for differential weighting. The ranking entity should seek to establish a more informed weighting scheme through the methods described in Chapter 6.
>
> **注**：等权并不意味着同等重要性；它反映了缺乏差异赋权的可辩护依据。排名实体宜通过第6章所述方法寻求建立更有依据的权重方案。

### 5.4.2 Delphi Method | 德尔菲法

The Delphi method may be used to derive initial weights through structured expert consultation. The process shall include:

德尔菲法可用于通过结构化专家咨询导出初始权重。过程应包括：

a) selection of a panel of at least five domain experts;

选择至少五名领域专家组成小组；

b) at least two rounds of anonymous expert assessment;

至少两轮匿名专家评估；

c) provision of statistical feedback (median and interquartile range) between rounds;

轮次间提供统计反馈（中位数和四分位距）；

d) convergence criteria (e.g., interquartile range below a defined threshold) to determine when sufficient consensus is reached.

收敛标准（如四分位距低于定义阈值）以确定何时达成充分共识。

### 5.4.3 Analytic Hierarchy Process (AHP) | 层次分析法

The Analytic Hierarchy Process may be used to derive initial weights through pairwise comparison of indicators. The AHP process shall comply with the following requirements:

层次分析法可用于通过指标的配对比较导出初始权重。AHP过程应符合以下要求：

a) Pairwise comparison matrices shall be constructed for indicators at each level of the hierarchy.

应为指标层级的每一层构建配对比较矩阵。

b) The consistency ratio (CR) of each comparison matrix shall not exceed 0.10. Where CR > 0.10, the expert shall revise the comparisons.

每个比较矩阵的一致性比率（CR）不应超过0.10。当CR > 0.10时，专家应修订比较。

c) The priority vectors derived from the comparison matrices shall be normalised to sum to 1.

从比较矩阵导出的优先向量应归一化为总和为1。

### 5.4.4 Principal Component Analysis (PCA) | 主成分分析

PCA may be used as a data-driven method to inform initial weight assignment. When PCA is used for this purpose:

主成分分析可用作数据驱动方法来为初始权重赋值提供依据。当为此目的使用PCA时：

a) The ranking entity shall report the proportion of variance explained by each retained component.

排名实体应报告每个保留成分解释的方差比例。

b) Weights derived from PCA loadings shall be interpreted with caution and validated against domain knowledge, as PCA-derived weights reflect data structure rather than substantive importance.

从PCA载荷导出的权重应谨慎解释并对照领域知识进行验证，因为PCA导出的权重反映的是数据结构而非实质重要性。

c) The ranking entity shall document the number of components retained and the retention criteria used.

排名实体应记录保留的成分数量和使用的保留标准。

### 5.4.5 Relationship Between Initial and Final Weights | 权重初设与最终权重的关系

The initial weight scheme is provisional and shall be subject to the full weight determination process specified in Chapter 6. The final weights may differ from the initial weights as a result of:

初始权重方案是临时的，应接受第6章规定的完整权重确定过程。最终权重可能因以下原因与初始权重不同：

a) stakeholder consultation;

利益相关方协商；

b) sensitivity analysis (see 6.3);

敏感性分析（见6.3）；

c) methodological refinement.

方法论优化。

The ranking entity shall document the difference between initial and final weights and the reasons for any significant changes.

排名实体应记录初始权重与最终权重之间的差异及任何重大变更的理由。

---

## 5.5 Indicator Update Mechanism | 指标更新机制

The indicator system shall be subject to periodic review and, where necessary, updated to ensure its continued relevance and validity.

指标体系应接受定期审查，并在必要时更新，以确保其持续的相关性和有效性。

### 5.5.1 Review Cycle | 评审周期

The ranking entity shall conduct a formal review of the indicator system at intervals not exceeding five years. The review shall assess:

排名实体应以不超过五年的间隔对指标体系进行正式审查。审查应评估：

a) whether the indicators remain relevant to the ranking purpose;

指标是否仍然与排名目的相关；

b) whether the data landscape has changed significantly;

数据环境是否发生重大变化；

c) whether new indicators should be added or existing indicators removed;

是否应增加新指标或移除现有指标；

d) whether the validity of the indicator system has been maintained (see 5.3).

指标体系的有效性是否得到保持（见5.3）。

### 5.5.2 Trigger Conditions for Indicator Changes | 指标变更的触发条件

In addition to the periodic review, an indicator review shall be triggered by:

除定期审查外，指标审查应由以下条件触发：

a) a material change in the ranking purpose or scope;

排名目的或范围发生实质变化；

b) the permanent unavailability of a data source relied upon by one or more indicators;

一个或多个指标所依赖的数据源永久不可用；

c) the publication of significant new research that challenges the validity or relevance of an indicator;

发表重大新研究质疑某指标的有效性或相关性；

d) the identification of systematic bias attributable to an indicator (see 4.7).

识别到可归因于某指标的系统性偏见（见4.7）。

### 5.5.3 Indicator Change Process | 指标变更流程

Any change to the indicator system shall follow a documented process that includes:

指标体系的任何变更应遵循记录的过程，包括：

a) a proposal documenting the change and its rationale;

记录变更及其理由的提案；

b) an impact assessment of the proposed change on the ranking results;

拟议变更对排名结果的影响评估；

c) a consultation period allowing stakeholder input of no less than 30 calendar days;

不少于30个日历日的利益相关方意见征求期；

d) a decision by the ranking entity with documented justification;

排名实体做出决定并记录理由；

e) public announcement of the change at least one ranking cycle before implementation, unless the change is required to address a compliance or ethical issue.

在实施前至少一个排名周期公开宣布变更，除非变更为解决合规或伦理问题所必需。

### 5.5.4 Version Management | 版本管理

Each version of the indicator system shall be uniquely identified. The version identifier shall include:

指标体系的每个版本应唯一标识。版本标识应包括：

a) a version number following a defined schema (e.g., major.minor);

遵循定义方案的版本号（如主版本号.次版本号）；

b) the effective date;

生效日期；

c) a summary of changes from the previous version.

与前一版本的变更摘要。

All prior versions of the indicator system shall be archived and accessible for audit purposes.

指标体系的所有先前版本应予以归档，并可供审计使用。

---

## 5.6 Extension Module Indicator Reference Rules | 扩展模块指标引用规则

This standard adopts a two-layer architecture: the core layer (this chapter and Chapters 4 through 8) defines methodology requirements applicable to all ranking domains; extension layers define domain-specific indicators and rules.

本标准采用两层架构：核心层（本章及第4章至第8章）定义适用于所有排名领域的方法论要求；扩展层定义领域特定指标和规则。

### 5.6.1 Core-Layer Indicator Design Methodology | 核心层指标设计方法论

The core layer defines the general methodology for indicator selection, hierarchy design, validity verification, weight assignment, and update management. This methodology applies universally, regardless of the ranking domain.

核心层定义指标选取、层级设计、有效性验证、权重赋值和更新管理的通用方法论。该方法论普遍适用，不因排名领域而异。

### 5.6.2 Extension-Layer Domain-Specific Indicators | 扩展层领域特定指标

Extension modules may define domain-specific indicators that are not covered by the core layer. Such indicators shall:

扩展模块可定义核心层未涵盖的领域特定指标。此类指标应：

a) satisfy all selection criteria specified in 5.1;

满足5.1规定的所有选取准则；

b) conform to the hierarchy rules specified in 5.2;

符合5.2规定的层级规则；

c) undergo validity verification as specified in 5.3;

按照5.3的规定进行有效性验证；

d) be subject to the update mechanism specified in 5.5.

接受5.5规定的更新机制。

### 5.6.3 Validation of Extension-Layer Indicators | 扩展层指标的核心层方法论验证

Extension-layer indicators shall be validated using the methodology specified in this chapter. The validation shall be documented in the extension module and shall be subject to the same transparency requirements as core-layer indicators.

扩展层指标应使用本章规定的方法论进行验证。验证应在扩展模块中记录，并应遵守与核心层指标相同的透明度要求。

a) The ranking entity shall verify that extension-layer indicators do not conflict with the principles specified in Chapter 4.

排名实体应验证扩展层指标不与第4章规定的原则冲突。

b) Where extension-layer indicators employ domain-specific measurement methods, those methods shall be documented with sufficient detail to permit independent verification.

当扩展层指标采用领域特定测量方法时，这些方法应以足够的细节记录，以允许独立验证。

c) The results of extension-layer indicator validation shall be referenced in the core methodology documentation.

扩展层指标验证的结果应在核心方法论文件中引用。

---

> **Note**: The two-layer architecture enables domain flexibility while maintaining methodological consistency. Extension modules should reference this chapter explicitly and declare their compliance with the core-layer requirements, rather than re-specifying the requirements.
>
> **注**：两层架构在保持方法论一致性的同时实现了领域灵活性。扩展模块应明确引用本章并声明其对核心层要求的符合性，而非重新规定这些要求。
