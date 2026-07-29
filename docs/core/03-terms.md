# Chapter 3: Terms and Definitions | 第3章 术语和定义

**ICO Std 2002:2026 — Chapter 3**

---

For the purposes of this standard, the following terms and definitions apply. Terms defined in the normative references listed in Chapter 2 retain their defined meanings when used in this standard, except where redefined below.

就本标准而言，下列术语和定义适用。第2章所列规范性引用文件中定义的术语在本标准中使用时保留其已定义的含义，除非下文重新定义。

ISO and IEC maintain terminological databases for use in standardization at the following addresses:

ISO 和 IEC 在以下地址维护用于标准化的术语数据库：

— ISO Online browsing platform: available at https://www.iso.org/obp
— IEC Electropedia: available at https://www.electropedia.org/

---

## 3.1 Core Terms | 核心术语

### 3.1.1 ranking system

**ranking system** | **排名系统**

organized set of processes, methods, and rules that produces a comparative ordering or scoring of a defined set of entities based on specified criteria

基于指定准则，对已定义实体集合产生比较排序或评分的有组织的流程、方法和规则集合

> **Note 1 to entry**: A ranking system encompasses the entire lifecycle from design to publication, including indicator selection, data collection, scoring, and result dissemination.
>
> **注1**：排名系统涵盖从设计到发布的整个生命周期，包括指标选择、数据采集、评分和结果发布。

> **Note 2 to entry**: A ranking system may produce results in the form of ordinal rankings (e.g., 1st, 2nd, 3rd), composite scores, or tier classifications (e.g., five-star ratings).
>
> **注2**：排名系统可以序数排名（如第1、第2、第3）、综合评分或等级分类（如五星评级）的形式产生结果。

**EXAMPLE** | **示例**: The Academic Ranking of World Universities (ARWU), the Global Liveability Index, and the Fortune 500 are all ranking systems.

### 3.1.2 ranking methodology

**ranking methodology** | **排名方法论**

systematic framework of principles, procedures, and rules governing the design, execution, and validation of a ranking system

治理排名系统设计、执行和验证的原则、程序和规则的系统框架

> **Note 1 to entry**: Ranking methodology includes but is not limited to: the selection and definition of indicators, the assignment of weights, the specification of data collection procedures, the choice of scoring and aggregation methods, and the requirements for transparency and audit.
>
> **注1**：排名方法论包括但不限于：指标的选择和定义、权重的分配、数据采集程序的规定、评分和聚合方法的选择，以及透明度和审计的要求。

> **Note 2 to entry**: A ranking methodology is distinct from a ranking system in that it refers to the abstract framework and rules, whereas a ranking system refers to the complete operational instantiation.
>
> **注2**：排名方法论与排名系统的区别在于：方法论指抽象框架和规则，而排名系统指完整的运营实例化。

### 3.1.3 indicator

**indicator** | **指标**

measurable variable used to assess one or more attributes of a ranked entity within a ranking system

在排名系统中用于评估一个或多个被排实体属性的可测量变量

> **Note 1 to entry**: An indicator may be quantitative (e.g., revenue in USD) or qualitative (e.g., expert assessment on a defined scale).
>
> **注1**：指标可以是定量的（如以美元计的收入）或定性的（如在定义量表上的专家评估）。

> **Note 2 to entry**: Indicators are organized hierarchically within a ranking system: a top-level composite indicator may be decomposed into sub-indicators, which may in turn be decomposed into elementary indicators.
>
> **注2**：指标在排名系统中按层级组织：顶层综合指标可分解为子指标，子指标又可分解为基本指标。

**EXAMPLE** | **示例**: "Student-to-faculty ratio" is an indicator used in university ranking systems; "brand awareness" is an indicator used in brand value ranking systems.

### 3.1.4 weighting

**weighting** | **权重**

assignment of relative importance to each indicator within a ranking system, expressed as a numerical coefficient that determines the indicator's contribution to the aggregate score

在排名系统中赋予每个指标的相对重要性，以数值系数表示，决定该指标对总评分的贡献度

> **Note 1 to entry**: Weights are typically normalised so that their sum equals one (or 100%).
>
> **注1**：权重通常归一化，使其总和等于一（或100%）。

> **Note 2 to entry**: The choice of weighting scheme can significantly affect ranking outcomes; therefore, the rationale for weighting decisions shall be documented and disclosed as required by Chapter 6.
>
> **注2**：权重方案的选择可显著影响排名结果；因此，权重决定的理由应按照第6章的要求予以记录和披露。

### 3.1.5 scoring

**scoring** | **评分**

process of assigning a numerical or categorical value to a ranked entity for each indicator or for the aggregate result

对每个指标或汇总结果赋予被排实体数值或类别值的过程

> **Note 1 to entry**: Scoring may involve the application of scoring functions, thresholds, or rubrics, depending on the nature of the indicator.
>
> **注1**：评分可涉及评分函数、阈值或评分规则的应用，取决于指标的性质。

> **Note 2 to entry**: The distinction between scoring and ranking is that scoring assigns values to individual entities, whereas ranking orders entities relative to one another based on their scores.
>
> **注2**：评分与排名的区别在于：评分对个别实体赋值，而排名根据实体的评分将其相对排序。

### 3.1.6 normalization

**normalization** | **归一化**

mathematical transformation applied to indicator values to render them comparable across different measurement scales, units, or distributions

对不同测量尺度、单位或分布的指标值进行数学变换，使其具有可比性

> **Note 1 to entry**: Common normalization methods include min-max normalisation, z-score standardisation, percentile ranking, and rank-order transformation.
>
> **注1**：常见的归一化方法包括最小-最大归一化、z-分数标准化、百分位排名和秩次变换。

> **Note 2 to entry**: The choice of normalization method can affect the distribution of scores and, consequently, the ranking outcome. The normalization method used shall be documented and justified.
>
> **注2**：归一化方法的选择可影响评分分布，进而影响排名结果。所使用的归一化方法应予以记录和论证。

**EXAMPLE** | **示例**: Converting raw revenue figures in different currencies to a common purchasing-power-parity-adjusted index is a form of normalization.

### 3.1.7 data source

**data source** | **数据源**

origin from which data used as input to a ranking system is obtained, including but not limited to official statistics, surveys, expert assessments, and automated data collection

排名系统输入数据的来源，包括但不限于官方统计、调查、专家评估和自动化数据采集

> **Note 1 to entry**: Data sources may be primary (collected directly by or for the ranking entity) or secondary (obtained from third-party providers or publicly available databases).
>
> **注1**：数据源可以是一手的（由排名实体或为其直接采集）或二手的（从第三方提供者或公共数据库获取）。

> **Note 2 to entry**: The identification, documentation, and quality assessment of data sources are critical to the integrity of a ranking system and are governed by the provisions of Chapter 7.
>
> **注2**：数据源的识别、记录和质量评估对排名系统的完整性至关重要，受第7章条款的约束。

### 3.1.8 ranking entity

**ranking entity** | **排名实体**

organization that initiates, designs, and publishes a ranking system and assumes responsibility for its methodological integrity and conformance with this standard

发起、设计和发布排名系统并对其方法论完整性和本标准一致性承担责任的机构

> **Note 1 to entry**: The ranking entity is the primary party accountable for the ranking system. It may carry out the ranking process itself or delegate execution to one or more executing parties (see 1.1.3).
>
> **注1**：排名实体是对排名系统承担主要责任的一方。其可自行执行排名过程或将执行委托给一个或多个执行方（见 1.1.3）。

> **Note 2 to entry**: The ranking entity is responsible for ensuring that the ranking system conforms to this standard, regardless of whether execution is delegated.
>
> **注2**：无论执行是否委托，排名实体均有责任确保排名系统符合本标准。

### 3.1.9 ranked entity

**ranked entity** | **被排实体**

individual, organisation, product, service, or other object that is assessed and positioned within a ranking system

在排名系统中被评估和定位的个人、组织、产品、服务或其他对象

> **Note 1 to entry**: The nature of ranked entities varies across ranking domains: in university rankings, ranked entities are higher education institutions; in brand rankings, ranked entities are brands; in city rankings, ranked entities are cities or urban areas.
>
> **注1**：被排实体的性质因排名领域而异：在大学排名中，被排实体为高等教育机构；在品牌排名中，被排实体为品牌；在城市排名中，被排实体为城市或城区。

> **Note 2 to entry**: A ranked entity may also be referred to as an "assessment object" or "subject of ranking" in other standards and guidelines.
>
> **注2**：被排实体在其他标准和指南中亦可称为"评估对象"或"排名主体"。

### 3.1.10 ranking cycle

**ranking cycle** | **排名周期**

complete iteration of a ranking system from initiation of data collection to publication of results

从启动数据采集到发布结果的排名系统完整迭代

> **Note 1 to entry**: A ranking cycle may be periodic (e.g., annual, biennial) or episodic (e.g., triggered by specific events or thresholds).
>
> **注1**：排名周期可以是定期的（如年度、两年一次）或事件驱动的（如由特定事件或阈值触发）。

> **Note 2 to entry**: Changes in methodology between ranking cycles shall be documented and disclosed in accordance with Chapter 9.
>
> **注2**：排名周期间方法论的变更应按照第9章的要求予以记录和披露。

**EXAMPLE** | **示例**: The annual publication of the QS World University Rankings constitutes one ranking cycle per year.

### 3.1.11 transparency report

**transparency report** | **透明度报告**

document published by the ranking entity that discloses the methodology, data sources, weighting, scoring procedures, and known limitations of the ranking system in sufficient detail to enable stakeholders to assess its validity and fairness

排名实体发布的文件，以足够详细的方式披露排名系统的方法论、数据源、权重、评分程序和已知局限，使利益相关方能评估其有效性和公平性

> **Note 1 to entry**: The transparency report is the primary instrument for meeting the disclosure requirements of Chapter 9 and a primary audit artifact for the purposes of Chapter 10.
>
> **注1**：透明度报告是满足第9章披露要求的主要工具，也是第10章审计目的的主要审计工件。

> **Note 2 to entry**: The transparency report shall be published concurrently with or prior to the publication of ranking results, not subsequently.
>
> **注2**：透明度报告应与排名结果发布同时或在其之前发布，而非之后。

### 3.1.12 audit trail

**audit trail** | **审计轨迹**

chronological record of all methodological decisions, data transformations, and computational steps that enables the reconstruction and verification of the ranking process from source data to published results

方法论决策、数据变换和计算步骤的按时间顺序记录，使从源数据到发布结果的排名过程重建和验证成为可能

> **Note 1 to entry**: An audit trail includes but is not limited to: records of indicator selection decisions, weighting deliberations, data cleaning and transformation procedures, aggregation computations, and any post-hoc adjustments.
>
> **注1**：审计轨迹包括但不限于：指标选择决定的记录、权重审议、数据清洗和变换程序、聚合计算和任何事后调整。

> **Note 2 to entry**: The audit trail is a critical component of the reproducibility requirement (see 3.1.17) and the audit provisions of Chapter 10.
>
> **注2**：审计轨迹是可复现性要求（见 3.1.17）和第10章审计条款的关键组成部分。

### 3.1.13 conformance

**conformance** | **一致性/合规**

fulfilment of a requirement of this standard by a ranking system

排名系统对本标准要求的满足

> **Note 1 to entry**: Conformance may be full (see 1.4.1) or partial (see 1.4.2).
>
> **注1**：一致性可以是完全的（见 1.4.1）或部分的（见 1.4.2）。

> **Note 2 to entry**: Conformance is assessed through independent audit as specified in Chapter 10, except where self-assessment is permitted by the provisions of Chapter 11.
>
> **注2**：一致性通过第10章规定的独立审计评估，除非第11章条款允许自我评估。

### 3.1.14 extension module

**extension module** | **扩展模块**

supplementary part of this standard that specifies domain-specific requirements applicable to a particular category of ranking systems, supplementing the core requirements

本标准的补充部分，规定适用于特定类别排名系统的领域特定要求，补充核心要求

> **Note 1 to entry**: Extension modules are designated SE-01 through SE-09, each corresponding to a specific ranking domain as described in 1.1.1.
>
> **注1**：扩展模块编号为 SE-01 至 SE-09，各对应 1.1.1 所述的特定排名领域。

> **Note 2 to entry**: Conformance with an extension module is required only when a ranking system falls within the corresponding domain (see 1.4.2).
>
> **注2**：仅当排名系统属于相应领域时，才要求对扩展模块的一致性（见 1.4.2）。

### 3.1.15 conflict of interest

**conflict of interest** | **利益冲突**

situation in which the ranking entity, its personnel, or any party involved in the ranking process has a financial, commercial, personal, or other interest that could, or could appear to, compromise the objectivity or impartiality of the ranking process or its results

排名实体、其人员或排名过程中涉及的任何一方具有可能损害或可能被认为损害排名过程或结果客观性或公正性的财务、商业、个人或其他利益的情况

> **Note 1 to entry**: Conflicts of interest may arise from commercial relationships between the ranking entity and ranked entities, from the ranking entity's financial dependence on revenue from ranked entities, or from personal relationships between assessors and assessed parties.
>
> **注1**：利益冲突可产生于排名实体与被排实体之间的商业关系、排名实体对被排实体收入的财务依赖，或评估者与被评估方之间的个人关系。

> **Note 2 to entry**: The identification, disclosure, and management of conflicts of interest are governed by the provisions of Chapter 4 (Principles) and Chapter 9 (Publication and Transparency).
>
> **注2**：利益冲突的识别、披露和管理受第4章（原则）和第9章（发布与透明度）条款的约束。

**EXAMPLE** | **示例**: A ranking entity that derives a significant portion of its revenue from consulting services sold to ranked entities has a financial conflict of interest.

### 3.1.16 sensitivity analysis

**sensitivity analysis** | **敏感性分析**

systematic examination of how variations in inputs, assumptions, or methodological choices affect the outputs of a ranking system

对输入、假设或方法论选择的变动如何影响排名系统输出的系统性检查

> **Note 1 to entry**: Sensitivity analysis is used to assess the robustness of ranking results and to identify indicators or methodological choices that disproportionately influence outcomes.
>
> **注1**：敏感性分析用于评估排名结果的稳健性，识别对结果产生不成比例影响的指标或方法论选择。

> **Note 2 to entry**: This standard requires sensitivity analysis to be performed and documented as specified in Chapter 8.
>
> **注2**：本标准要求按照第8章的规定执行和记录敏感性分析。

**EXAMPLE** | **示例**: Re-computing a ranking with weights varied by ±10% and observing the resulting changes in entity positions constitutes a basic sensitivity analysis.

### 3.1.17 reproducibility

**reproducibility** | **可复现性**

ability of an independent party to obtain the same ranking results when applying the documented methodology to the same data, within the bounds of acceptable computational precision

独立方在将已记录的方法论应用于相同数据时，在可接受计算精度范围内获得相同排名结果的能力

> **Note 1 to entry**: Reproducibility is a necessary condition for the verifiability of a ranking system. It requires that the methodology be documented with sufficient precision and that the underlying data be accessible for verification purposes.
>
> **注1**：可复现性是排名系统可验证性的必要条件。它要求方法论以足够的精度予以记录，且底层数据可访问以供验证。

> **Note 2 to entry**: Reproducibility is distinct from replicability. Reproducibility refers to obtaining consistent results using the same data and methodology; replicability refers to obtaining consistent results using new data collected under the same protocol.
>
> **注2**：可复现性区别于可重复性。可复现性指使用相同数据和方法论获得一致结果；可重复性指在相同方案下采集新数据获得一致结果。

---

> **Note**: This chapter is part of ICO Std 2002 (Tianji Ranking Methodology Standard). The definitions in this chapter are normative. Terms used in this standard that are not defined herein retain their commonly understood meanings or the meanings assigned in the normative references listed in Chapter 2.
>
> **注意**：本章属于 ICO Std 2002（天机排名方法论标准）。本章定义为规范性内容。本标准中使用但未在此定义的术语保留其通用理解含义或第2章所列规范性引用文件中赋予的含义。
