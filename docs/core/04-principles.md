# Chapter 4: General Principles | 第4章 通用原则

**ICO Std 2002:2026 — Chapter 4**

---

This chapter establishes the fundamental principles that shall govern the design, execution, and governance of all ranking methodologies under this International Standard. These principles constitute the normative foundation upon which subsequent chapters build specific technical requirements.

本章确立了治理本国际标准下所有排名方法论设计、执行和治理的基本原则。这些原则构成后续章节构建特定技术要求的规范性基础。

---

## 4.1 Independence | 独立性原则

The design and execution of a ranking methodology shall be independent of any stakeholder that has a material interest in the ranking outcome.

排名方法论的设计与执行应独立于任何对排名结果有实质利益的利益相关方。

### 4.1.1 Organisational Independence | 组织独立性

The entity responsible for designing and executing the ranking methodology (the "ranking entity") shall not be the same entity as, nor a subsidiary of, any entity that is subject to the ranking (a "ranked entity").

负责设计和执行排名方法论的实体（"排名实体"）不应与受排名约束的实体（"被排实体"）为同一实体，亦不应为被排实体的附属机构。

### 4.1.2 Conflict of Interest Identification | 利益冲突识别

The ranking entity shall maintain a register of all actual and potential conflicts of interest, including but not limited to:

排名实体应维护所有实际和潜在利益冲突的登记册，包括但不限于：

a) financial relationships between the ranking entity and any ranked entity or its affiliates;

排名实体与任何被排实体或其关联方之间的财务关系；

b) employment or advisory relationships between personnel involved in the ranking process and any ranked entity;

参与排名过程的人员与任何被排实体之间的雇佣或顾问关系；

c) sponsorship, advertising, or licensing revenue derived from ranked entities;

从被排实体获得的赞助、广告或许可收入；

d) ownership interests in entities that could benefit from the ranking outcome.

可能从排名结果中受益的实体的所有权权益。

### 4.1.3 Conflict of Interest Disclosure | 利益冲突披露

All identified conflicts of interest shall be disclosed in the ranking methodology documentation and in the ranking publication. The disclosure shall include:

所有已识别的利益冲突应在排名方法论文件和排名发布中披露。披露应包括：

a) the nature and scope of the conflict;

冲突的性质和范围；

b) the parties involved;

涉及方；

c) the measures taken to mitigate the conflict.

为缓解冲突所采取的措施。

### 4.1.4 Conflict of Interest Recusal | 利益冲突回避

Where a conflict of interest is identified that cannot be adequately mitigated, the ranking entity shall recuse the affected personnel from the relevant aspects of the ranking process. Where the conflict is systemic and cannot be resolved by recusal, the ranking entity shall disclose this limitation prominently in the ranking publication and methodology documentation.

当识别到无法充分缓解的利益冲突时，排名实体应使受影响的人员回避排名过程的相关环节。当冲突具有系统性且无法通过回避解决时，排名实体应在排名发布和方法论文件中显著披露此局限性。

> **Note**: The principle of independence does not preclude the ranking entity from seeking expert input or data from ranked entities, provided that such input is subject to verification and does not influence the methodological design or scoring.
>
> **注**：独立性原则并不排除排名实体从被排实体获取专家意见或数据，前提是此类意见须经验证且不影响方法论设计或评分。

---

## 4.2 Transparency | 透明度原则

The ranking methodology shall be publicly accessible and sufficiently detailed to enable an informed assessment of its rigour and fairness.

排名方法论应公开可查，且详细程度足以使评估者对其严谨性和公正性做出知情判断。

### 4.2.1 Methodology Disclosure | 方法论披露

The ranking entity shall publish a complete description of the ranking methodology, including:

排名实体应发布排名方法的完整描述，包括：

a) the purpose and scope of the ranking;

排名的目的和范围；

b) the indicator system and its rationale;

指标体系及其依据；

c) the weight assignment method and resulting weights;

权重分配方法及最终权重；

d) the data sources and collection procedures;

数据来源和采集程序；

e) the scoring, normalisation, and aggregation methods;

评分、归一化和聚合方法；

f) the ranking rules, including tie-breaking procedures.

排序规则，包括并列处理程序。

### 4.2.2 Data Source Traceability | 数据来源可追溯性

All data used in the ranking shall be traceable to its source. For each data point, the following shall be documented:

排名中使用的所有数据应可追溯至其来源。对每个数据点，应记录以下信息：

a) the originating source (institution, database, publication);

原始来源（机构、数据库、出版物）；

b) the date of acquisition;

获取日期；

c) any transformations applied to the data prior to use.

使用前对数据施加的任何变换。

### 4.2.3 Scoring Rule Verifiability | 评分规则可验证性

The scoring rules shall be specified with sufficient precision that a third party, given the same input data, can verify the correctness of the reported scores and rankings. Where scoring rules involve expert judgement, the criteria for such judgement shall be documented.

评分规则应具有足够的精确度，使得第三方在获得相同输入数据时能够验证所报告得分和排名的正确性。当评分规则涉及专家判断时，此类判断的准则应予以记录。

> **Note**: Transparency does not require the disclosure of proprietary algorithms in source code form; however, the functional specification of the algorithm shall be disclosed with sufficient detail to permit independent verification.
>
> **注**：透明度不要求以源代码形式披露专有算法；但算法的功能规格应予以披露，详细程度足以允许独立验证。

---

## 4.3 Reproducibility | 可复现性原则

Given identical input data and the same methodology, the ranking process shall produce identical results. Third parties shall be able to independently reproduce the ranking results to a reasonable degree of precision.

给定相同的输入数据和方法论，排名过程应产生相同的结果。第三方应能够独立复现排名结果至合理的精度。

### 4.3.1 Computational Reproducibility | 计算可复现性

The ranking entity shall ensure that the computational steps of the ranking process are deterministic. Where stochastic methods are employed, the random seed or equivalent parameter shall be documented to enable exact replication.

排名实体应确保排名过程的计算步骤是确定性的。当采用随机方法时，应记录随机种子或等效参数以使精确复制成为可能。

### 4.3.2 Methodological Reproducibility | 方法论可复现性

The methodology documentation shall contain all information necessary for an independent party to replicate the ranking. This includes, at a minimum:

方法论文件应包含独立方复制排名所需的所有信息。至少包括：

a) precise mathematical definitions of all scoring and aggregation functions;

所有评分和聚合函数的精确数学定义；

b) the handling rules for missing data, outliers, and boundary conditions;

缺失数据、异常值和边界条件的处理规则；

c) the version identifiers of all data sources and software tools used.

所有使用的数据源和软件工具的版本标识。

### 4.3.3 Reproducibility Verification | 可复现性验证

The ranking entity should conduct or commission periodic reproducibility audits, in which an independent party attempts to replicate the ranking results from the published methodology and data.

排名实体宜进行或委托进行定期的可复现性审计，由独立方尝试根据已发布的方法论和数据复制排名结果。

---

## 4.4 Impartiality | 公正性原则

The ranking methodology shall treat all ranked entities equally and shall not confer advantages or disadvantages based on factors unrelated to the ranking criteria.

排名方法论应平等对待所有被排实体，不应基于与排名准则无关的因素赋予优势或劣势。

### 4.4.1 Prohibition of Paid Listing | 禁止付费上榜

The inclusion, exclusion, or relative position of any entity in a ranking shall not be influenced by payment, whether direct or indirect. A ranked entity shall not be able to purchase a favourable position in the ranking.

任何实体在排名中的纳入、排除或相对位置不应受到付款（无论是直接还是间接）的影响。被排实体不应能够购买排名中的有利位置。

### 4.4.2 Prohibition of Stakeholder Interference | 禁止利益相关方干预

No stakeholder, including but not limited to ranked entities, sponsors, advertisers, or governmental bodies, shall be permitted to influence the scoring or ranking of any entity. The ranking entity shall have sole authority over methodological decisions.

任何利益相关方，包括但不限于被排实体、赞助商、广告商或政府机构，均不应被允许影响任何实体的评分或排名。排名实体应对方法论决策拥有唯一权限。

### 4.4.3 Uniform Application of Criteria | 评分标准一致适用

The scoring criteria shall be applied uniformly to all ranked entities within the same ranking cycle. No entity shall be assessed using a different set of indicators, weights, or scoring thresholds unless such differentiation is explicitly justified in the methodology and applied on the basis of objective, pre-defined rules.

评分准则应在同一排名周期内统一适用于所有被排实体。除非在方法论中有明确依据且基于客观的、预先定义的规则，任何实体不应使用不同的指标集、权重或评分阈值进行评估。

---

## 4.5 Scientific Rigour | 科学性原则

The ranking methodology shall be grounded in established scientific methods and theoretical frameworks appropriate to the domain of the ranking.

排名方法论应以适合排名领域的既定科学方法和理论框架为基础。

### 4.5.1 Theoretical Basis for Indicator Selection | 指标选取的理论依据

Each indicator included in the ranking shall have a documented theoretical or empirical basis demonstrating its relevance to the ranking purpose. Indicators shall not be selected solely on the basis of data availability or convenience.

排名中纳入的每个指标应有记录的理论或实证依据，证明其与排名目的的相关性。指标不应仅基于数据可得性或便利性而选取。

### 4.5.2 Methodological Support for Weight Assignment | 权重分配的方法论支撑

The assignment of weights to indicators shall be supported by a documented methodology. The choice of weight assignment method (see Chapter 6) shall be justified with reference to the ranking purpose, data characteristics, and domain conventions.

指标的权重分配应有记录的方法论支撑。权重分配方法的选择（见第6章）应参照排名目的、数据特征和领域惯例进行论证。

### 4.5.3 Appropriate Use of Statistical Methods | 统计方法的适当使用

Statistical methods used in the ranking process shall be appropriate for the data characteristics and the analytical objectives. The ranking entity shall document:

排名过程中使用的统计方法应适合数据特征和分析目标。排名实体应记录：

a) the assumptions underlying each statistical method used;

所使用的每种统计方法的基本假设；

b) the results of assumption testing (e.g., normality tests, homoscedasticity tests);

假设检验的结果（如正态性检验、同方差性检验）；

c) any deviations from standard statistical practice and the justifications thereof.

偏离标准统计实践的任何情况及其理由。

### 4.5.4 Peer Review | 同行评审

The ranking methodology should be subject to peer review by qualified domain experts and methodologists prior to its first publication and following any major methodological revision.

排名方法论在首次发布前及任何重大方法论修订后，宜接受具备资质的领域专家和方法论专家的同行评审。

---

## 4.6 Proportionality | 比例原则

The complexity and granularity of a ranking methodology shall be proportionate to the purpose of the ranking and the needs of its intended users.

排名方法论的复杂度和精细度应与排名目的及其预期用户的需求相称。

### 4.6.1 Complexity Alignment | 复杂度匹配

The number of indicators, the depth of the indicator hierarchy, and the sophistication of the aggregation method shall be proportionate to:

指标数量、指标层级深度和聚合方法的复杂度应与以下因素相称：

a) the significance and reach of the ranking;

排名的重要性和影响力；

b) the availability and quality of data;

数据的可得性和质量；

c) the capacity of intended users to understand and use the results.

预期用户理解和使用结果的能力。

### 4.6.2 Avoidance of Over-Quantification | 避免过度量化

The ranking entity shall not attempt to quantify attributes that are inherently qualitative in nature unless a valid operationalisation framework exists. Where qualitative judgements are necessary, they shall be clearly identified as such and the criteria for judgement shall be documented.

排名实体不应试图量化本质上属于定性属性的要素，除非存在有效的操作化框架。当定性判断为必要时，应明确标识，且判断准则应予以记录。

> **Note**: Over-quantification can create a false impression of precision and may mislead users into attributing more objectivity to the ranking than the underlying data supports.
>
> **注**：过度量化可能造成精确性的假象，并可能误导用户对排名赋予超出底层数据所支持的客观性。

---

## 4.7 Non-discrimination | 非歧视原则

The ranking methodology shall not produce systematic bias against any country, region, or organisational type that is unrelated to the substantive criteria of the ranking.

排名方法论不应产生与排名实质准则无关的针对任何国家、地区或组织类型的系统性偏见。

### 4.7.1 Structural Bias Assessment | 结构性偏见评估

Prior to publication, the ranking entity shall assess whether the methodology introduces structural biases against specific groups of ranked entities. Such assessment shall include, at a minimum:

在发布前，排名实体应评估方法论是否引入了针对特定被排实体群体的结构性偏见。此类评估至少应包括：

a) an analysis of whether the indicator set disproportionately favours or disadvantages entities of a particular geographic, economic, or organisational character;

分析指标集是否不成比例地有利于或不利于具有特定地理、经济或组织特征的实体；

b) an examination of whether data availability disparities across groups systematically affect ranking outcomes;

审查不同群体间的数据可得性差异是否系统性地影响排名结果；

c) a review of whether normalisation or scoring methods embed implicit assumptions that disadvantage certain groups.

审查归一化或评分方法是否嵌入了不利于某些群体的隐含假设。

### 4.7.2 Mitigation of Identified Bias | 已识别偏见的缓解

Where structural bias is identified, the ranking entity shall take reasonable steps to mitigate it, such as adjusting indicators, employing group-specific normalisation, or clearly disclosing the limitation. The mitigation measures and their rationale shall be documented.

当识别到结构性偏见时，排名实体应采取合理步骤予以缓解，如调整指标、采用分组归一化或明确披露此局限性。缓解措施及其理由应予以记录。

### 4.7.3 Cultural Sensitivity | 文化敏感性

The ranking methodology shall be designed with awareness of cultural differences that may affect the interpretation and comparability of indicators across contexts. Indicators that are meaningful only within a specific cultural context shall be identified as such.

排名方法论的设计应意识到可能影响指标在不同语境下解释和可比性的文化差异。仅在特定文化语境内有意义的指标应予以标识。

---

## 4.8 Sustainability | 可持续性原则

The ranking methodology shall consider the long-term consequences of its application and shall not create incentives for short-term behaviour that undermines the ranking's stated purpose.

排名方法论应考虑其应用的长期后果，不应创造损害排名既定目的的短期行为激励。

### 4.8.1 Long-term Impact Assessment | 长期影响评估

The ranking entity should assess and document the potential long-term effects of the ranking on ranked entities and their stakeholders, including:

排名实体宜评估并记录排名对被排实体及其利益相关方的潜在长期影响，包括：

a) whether the ranking incentivises gaming behaviour (e.g., teaching to the test, window-dressing of financial statements);

排名是否激励博弈行为（如应试教育、财务报表粉饰）；

b) whether the ranking encourages substantive improvement or merely cosmetic compliance;

排名是鼓励实质性改善还是仅促使表面合规；

c) whether the ranking creates perverse incentives that may harm the very attributes it seeks to measure.

排名是否产生可能损害其所衡量属性的反向激励。

### 4.8.2 Incentive Alignment | 激励一致性

Where feasible, the ranking methodology should be designed so that actions taken by ranked entities to improve their ranking position also contribute to genuine improvement in the attributes being measured.

在可行的情况下，排名方法论的设计宜使被排实体为提升排名地位所采取的行动也有助于被衡量属性的真正改善。

### 4.8.3 Periodic Methodological Review | 定期方法论审查

The ranking entity shall conduct periodic reviews of the methodology to assess whether it continues to serve its intended purpose and does not produce adverse long-term effects. The review interval shall not exceed five years.

排名实体应定期审查方法论，以评估其是否继续服务于预期目的且不产生不良长期影响。审查间隔不应超过五年。

---

## 4.9 Alignment with the IREG Berlin Principles | 与 IREG 柏林原则的对标说明

The principles in this chapter are aligned with the Berlin Principles on Ranking of Higher Education Institutions, as adopted by the International Ranking Expert Group (IREG) in 2006, extended here to apply to all ranking domains covered by this standard. The following table summarises the correspondence:

本章原则与高等教育排名国际专家组（IREG）于2006年通过的《高等教育机构排名柏林原则》对齐，并在此扩展适用于本标准涵盖的所有排名领域。下表概述对应关系：

| ICO Std 2002 Principle | Berlin Principle | Alignment |
|---|---|---|
| 4.1 Independence | BP 1 (Purpose) | The ranking shall be designed to serve the stated purpose and shall not be influenced by institutional interests. |
| 4.2 Transparency | BP 2 (Transparency) | The methodology shall be open and transparent, allowing for understanding and replication. |
| 4.3 Reproducibility | BP 3 (Data Collection) | Data collection methods shall be clearly specified and consistently applied, enabling replication. |
| 4.4 Impartiality | BP 4 (Outcome Measures) | Outcomes shall reflect the measured attributes without extraneous influence; paid positioning is prohibited. |
| 4.5 Scientific Rigour | BP 5–6 (Indicators) | Indicators shall be chosen based on relevance and validity, using appropriate statistical methods. |
| 4.6 Proportionality | — | No direct Berlin Principle equivalent; derived from the general requirement for methodological appropriateness. |
| 4.7 Non-discrimination | BP 7 (Language and Context) | Rankings shall account for linguistic and cultural differences to avoid systematic bias. |
| 4.8 Sustainability | BP 8 (Economic and Social Impact) | Rankings shall consider their economic and social impact and avoid perverse incentives. |

> **Note**: The Berlin Principles were originally formulated for higher education rankings. ICO Std 2002 extends and generalises these principles to all ranking domains while preserving their normative intent. Where domain-specific guidance is needed, the relevant extension module (see Chapter 5, Section 5.6) shall provide supplementary requirements.
>
> **注**：柏林原则最初为高等教育排名制定。ICO Std 2002 在保留规范性意图的同时，将这些原则扩展和泛化至所有排名领域。当需要领域特定指导时，相关扩展模块（见第5章第5.6节）应提供补充要求。

---

> **Note**: The principles in this chapter are normative. A ranking methodology that does not conform to any of these principles shall not claim compliance with ICO Std 2002. Where a principle cannot be fully satisfied due to objective constraints, the ranking entity shall document the deviation, the reason for the deviation, and the mitigation measures taken (see Chapter 11).
>
> **注**：本章原则为规范性条款。不符合任何这些原则的排名方法论不应声称符合 ICO Std 2002。当因客观约束无法完全满足某项原则时，排名实体应记录偏离、偏离原因及所采取的缓解措施（见第11章）。
