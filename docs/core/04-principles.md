# Chapter 4: General Principles

**ICO Std 2002:2026 — Chapter 4**

---

This chapter establishes the fundamental principles that shall govern the design, execution, and governance of all ranking methodologies under this International Standard. These principles constitute the normative foundation upon which subsequent chapters build specific technical requirements.

---

## 4.1 Independence

The design and execution of a ranking methodology shall be independent of any stakeholder that has a material interest in the ranking outcome.

### 4.1.1 Organisational Independence

The entity responsible for designing and executing the ranking methodology (the "ranking entity") shall not be the same entity as, nor a subsidiary of, any entity that is subject to the ranking (a "ranked entity").

### 4.1.2 Conflict of Interest Identification

The ranking entity shall maintain a register of all actual and potential conflicts of interest, including but not limited to:

a) financial relationships between the ranking entity and any ranked entity or its affiliates;

b) employment or advisory relationships between personnel involved in the ranking process and any ranked entity;

c) sponsorship, advertising, or licensing revenue derived from ranked entities;

d) ownership interests in entities that could benefit from the ranking outcome.

### 4.1.3 Conflict of Interest Disclosure

All identified conflicts of interest shall be disclosed in the ranking methodology documentation and in the ranking publication. The disclosure shall include:

a) the nature and scope of the conflict;

b) the parties involved;

c) the measures taken to mitigate the conflict.

### 4.1.4 Conflict of Interest Recusal

Where a conflict of interest is identified that cannot be adequately mitigated, the ranking entity shall recuse the affected personnel from the relevant aspects of the ranking process. Where the conflict is systemic and cannot be resolved by recusal, the ranking entity shall disclose this limitation prominently in the ranking publication and methodology documentation.

> **Note**: The principle of independence does not preclude the ranking entity from seeking expert input or data from ranked entities, provided that such input is subject to verification and does not influence the methodological design or scoring.
>

---

## 4.2 Transparency

The ranking methodology shall be publicly accessible and sufficiently detailed to enable an informed assessment of its rigour and fairness.

### 4.2.1 Methodology Disclosure

The ranking entity shall publish a complete description of the ranking methodology, including:

a) the purpose and scope of the ranking;

b) the indicator system and its rationale;

c) the weight assignment method and resulting weights;

d) the data sources and collection procedures;

e) the scoring, normalisation, and aggregation methods;

f) the ranking rules, including tie-breaking procedures.

### 4.2.2 Data Source Traceability

All data used in the ranking shall be traceable to its source. For each data point, the following shall be documented:

a) the originating source (institution, database, publication);

b) the date of acquisition;

c) any transformations applied to the data prior to use.

### 4.2.3 Scoring Rule Verifiability

The scoring rules shall be specified with sufficient precision that a third party, given the same input data, can verify the correctness of the reported scores and rankings. Where scoring rules involve expert judgement, the criteria for such judgement shall be documented.

> **Note**: Transparency does not require the disclosure of proprietary algorithms in source code form; however, the functional specification of the algorithm shall be disclosed with sufficient detail to permit independent verification.
>

---

## 4.3 Reproducibility

Given identical input data and the same methodology, the ranking process shall produce identical results. Third parties shall be able to independently reproduce the ranking results to a reasonable degree of precision.

### 4.3.1 Computational Reproducibility

The ranking entity shall ensure that the computational steps of the ranking process are deterministic. Where stochastic methods are employed, the random seed or equivalent parameter shall be documented to enable exact replication.

### 4.3.2 Methodological Reproducibility

The methodology documentation shall contain all information necessary for an independent party to replicate the ranking. This includes, at a minimum:

a) precise mathematical definitions of all scoring and aggregation functions;

b) the handling rules for missing data, outliers, and boundary conditions;

c) the version identifiers of all data sources and software tools used.

### 4.3.3 Reproducibility Verification

The ranking entity should conduct or commission periodic reproducibility audits, in which an independent party attempts to replicate the ranking results from the published methodology and data.

---

## 4.4 Impartiality

The ranking methodology shall treat all ranked entities equally and shall not confer advantages or disadvantages based on factors unrelated to the ranking criteria.

### 4.4.1 Prohibition of Paid Listing

The inclusion, exclusion, or relative position of any entity in a ranking shall not be influenced by payment, whether direct or indirect. A ranked entity shall not be able to purchase a favourable position in the ranking.

### 4.4.2 Prohibition of Stakeholder Interference

No stakeholder, including but not limited to ranked entities, sponsors, advertisers, or governmental bodies, shall be permitted to influence the scoring or ranking of any entity. The ranking entity shall have sole authority over methodological decisions.

### 4.4.3 Uniform Application of Criteria

The scoring criteria shall be applied uniformly to all ranked entities within the same ranking cycle. No entity shall be assessed using a different set of indicators, weights, or scoring thresholds unless such differentiation is explicitly justified in the methodology and applied on the basis of objective, pre-defined rules.

---

## 4.5 Scientific Rigour

The ranking methodology shall be grounded in established scientific methods and theoretical frameworks appropriate to the domain of the ranking.

### 4.5.1 Theoretical Basis for Indicator Selection

Each indicator included in the ranking shall have a documented theoretical or empirical basis demonstrating its relevance to the ranking purpose. Indicators shall not be selected solely on the basis of data availability or convenience.

### 4.5.2 Methodological Support for Weight Assignment

The assignment of weights to indicators shall be supported by a documented methodology. The choice of weight assignment method (see Chapter 6) shall be justified with reference to the ranking purpose, data characteristics, and domain conventions.

### 4.5.3 Appropriate Use of Statistical Methods

Statistical methods used in the ranking process shall be appropriate for the data characteristics and the analytical objectives. The ranking entity shall document:

a) the assumptions underlying each statistical method used;

b) the results of assumption testing (e.g., normality tests, homoscedasticity tests);

c) any deviations from standard statistical practice and the justifications thereof.

### 4.5.4 Peer Review

The ranking methodology should be subject to peer review by qualified domain experts and methodologists prior to its first publication and following any major methodological revision.

---

## 4.6 Proportionality

The complexity and granularity of a ranking methodology shall be proportionate to the purpose of the ranking and the needs of its intended users.

### 4.6.1 Complexity Alignment

The number of indicators, the depth of the indicator hierarchy, and the sophistication of the aggregation method shall be proportionate to:

a) the significance and reach of the ranking;

b) the availability and quality of data;

c) the capacity of intended users to understand and use the results.

### 4.6.2 Avoidance of Over-Quantification

The ranking entity shall not attempt to quantify attributes that are inherently qualitative in nature unless a valid operationalisation framework exists. Where qualitative judgements are necessary, they shall be clearly identified as such and the criteria for judgement shall be documented.

> **Note**: Over-quantification can create a false impression of precision and may mislead users into attributing more objectivity to the ranking than the underlying data supports.
>

---

## 4.7 Non-discrimination

The ranking methodology shall not produce systematic bias against any country, region, or organisational type that is unrelated to the substantive criteria of the ranking.

### 4.7.1 Structural Bias Assessment

Prior to publication, the ranking entity shall assess whether the methodology introduces structural biases against specific groups of ranked entities. Such assessment shall include, at a minimum:

a) an analysis of whether the indicator set disproportionately favours or disadvantages entities of a particular geographic, economic, or organisational character;

b) an examination of whether data availability disparities across groups systematically affect ranking outcomes;

c) a review of whether normalisation or scoring methods embed implicit assumptions that disadvantage certain groups.

### 4.7.2 Mitigation of Identified Bias

Where structural bias is identified, the ranking entity shall take reasonable steps to mitigate it, such as adjusting indicators, employing group-specific normalisation, or clearly disclosing the limitation. The mitigation measures and their rationale shall be documented.

### 4.7.3 Cultural Sensitivity

The ranking methodology shall be designed with awareness of cultural differences that may affect the interpretation and comparability of indicators across contexts. Indicators that are meaningful only within a specific cultural context shall be identified as such.

---

## 4.8 Sustainability

The ranking methodology shall consider the long-term consequences of its application and shall not create incentives for short-term behaviour that undermines the ranking's stated purpose.

### 4.8.1 Long-term Impact Assessment

The ranking entity should assess and document the potential long-term effects of the ranking on ranked entities and their stakeholders, including:

a) whether the ranking incentivises gaming behaviour (e.g., teaching to the test, window-dressing of financial statements);

b) whether the ranking encourages substantive improvement or merely cosmetic compliance;

c) whether the ranking creates perverse incentives that may harm the very attributes it seeks to measure.

### 4.8.2 Incentive Alignment

Where feasible, the ranking methodology should be designed so that actions taken by ranked entities to improve their ranking position also contribute to genuine improvement in the attributes being measured.

### 4.8.3 Periodic Methodological Review

The ranking entity shall conduct periodic reviews of the methodology to assess whether it continues to serve its intended purpose and does not produce adverse long-term effects. The review interval shall not exceed five years.

---

## 4.9 Alignment with the IREG Berlin Principles

The principles in this chapter are aligned with the Berlin Principles on Ranking of Higher Education Institutions, as adopted by the International Ranking Expert Group (IREG) in 2006, extended here to apply to all ranking domains covered by this standard. The following table summarises the correspondence:

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

---

> **Note**: The principles in this chapter are normative. A ranking methodology that does not conform to any of these principles shall not claim compliance with ICO Std 2002. Where a principle cannot be fully satisfied due to objective constraints, the ranking entity shall document the deviation, the reason for the deviation, and the mitigation measures taken (see Chapter 11).
>
