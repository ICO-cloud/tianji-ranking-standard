# Chapter 3: Terms and Definitions

**ICO Std 2002:2026 — Chapter 3**

---

For the purposes of this standard, the following terms and definitions apply. Terms defined in the normative references listed in Chapter 2 retain their defined meanings when used in this standard, except where redefined below.

ISO and IEC maintain terminological databases for use in standardization at the following addresses:

— ISO Online browsing platform: available at https://www.iso.org/obp
— IEC Electropedia: available at https://www.electropedia.org/

---

## 3.1 Core Terms

### 3.1.1 ranking system

**ranking system**

organized set of processes, methods, and rules that produces a comparative ordering or scoring of a defined set of entities based on specified criteria

> **Note 1 to entry**: A ranking system encompasses the entire lifecycle from design to publication, including indicator selection, data collection, scoring, and result dissemination.
>

> **Note 2 to entry**: A ranking system may produce results in the form of ordinal rankings (e.g., 1st, 2nd, 3rd), composite scores, or tier classifications (e.g., five-star ratings).
>

**EXAMPLE** : The Academic Ranking of World Universities (ARWU), the Global Liveability Index, and the Fortune 500 are all ranking systems.

### 3.1.2 ranking methodology

**ranking methodology**

systematic framework of principles, procedures, and rules governing the design, execution, and validation of a ranking system

> **Note 1 to entry**: Ranking methodology includes but is not limited to: the selection and definition of indicators, the assignment of weights, the specification of data collection procedures, the choice of scoring and aggregation methods, and the requirements for transparency and audit.
>

> **Note 2 to entry**: A ranking methodology is distinct from a ranking system in that it refers to the abstract framework and rules, whereas a ranking system refers to the complete operational instantiation.
>

### 3.1.3 indicator

**indicator**

measurable variable used to assess one or more attributes of a ranked entity within a ranking system

> **Note 1 to entry**: An indicator may be quantitative (e.g., revenue in USD) or qualitative (e.g., expert assessment on a defined scale).
>

> **Note 2 to entry**: Indicators are organized hierarchically within a ranking system: a top-level composite indicator may be decomposed into sub-indicators, which may in turn be decomposed into elementary indicators.
>

**EXAMPLE** : "Student-to-faculty ratio" is an indicator used in university ranking systems; "brand awareness" is an indicator used in brand value ranking systems.

### 3.1.4 weighting

**weighting**

assignment of relative importance to each indicator within a ranking system, expressed as a numerical coefficient that determines the indicator's contribution to the aggregate score

> **Note 1 to entry**: Weights are typically normalised so that their sum equals one (or 100%).
>

> **Note 2 to entry**: The choice of weighting scheme can significantly affect ranking outcomes; therefore, the rationale for weighting decisions shall be documented and disclosed as required by Chapter 6.
>

### 3.1.5 scoring

**scoring**

process of assigning a numerical or categorical value to a ranked entity for each indicator or for the aggregate result

> **Note 1 to entry**: Scoring may involve the application of scoring functions, thresholds, or rubrics, depending on the nature of the indicator.
>

> **Note 2 to entry**: The distinction between scoring and ranking is that scoring assigns values to individual entities, whereas ranking orders entities relative to one another based on their scores.
>

### 3.1.6 normalization

**normalization**

mathematical transformation applied to indicator values to render them comparable across different measurement scales, units, or distributions

> **Note 1 to entry**: Common normalization methods include min-max normalisation, z-score standardisation, percentile ranking, and rank-order transformation.
>

> **Note 2 to entry**: The choice of normalization method can affect the distribution of scores and, consequently, the ranking outcome. The normalization method used shall be documented and justified.
>

**EXAMPLE** : Converting raw revenue figures in different currencies to a common purchasing-power-parity-adjusted index is a form of normalization.

### 3.1.7 data source

**data source**

origin from which data used as input to a ranking system is obtained, including but not limited to official statistics, surveys, expert assessments, and automated data collection

> **Note 1 to entry**: Data sources may be primary (collected directly by or for the ranking entity) or secondary (obtained from third-party providers or publicly available databases).
>

> **Note 2 to entry**: The identification, documentation, and quality assessment of data sources are critical to the integrity of a ranking system and are governed by the provisions of Chapter 7.
>

### 3.1.8 ranking entity

**ranking entity**

organization that initiates, designs, and publishes a ranking system and assumes responsibility for its methodological integrity and conformance with this standard

> **Note 1 to entry**: The ranking entity is the primary party accountable for the ranking system. It may carry out the ranking process itself or delegate execution to one or more executing parties (see 1.1.3).
>

> **Note 2 to entry**: The ranking entity is responsible for ensuring that the ranking system conforms to this standard, regardless of whether execution is delegated.
>

### 3.1.9 ranked entity

**ranked entity**

individual, organisation, product, service, or other object that is assessed and positioned within a ranking system

> **Note 1 to entry**: The nature of ranked entities varies across ranking domains: in university rankings, ranked entities are higher education institutions; in brand rankings, ranked entities are brands; in city rankings, ranked entities are cities or urban areas.
>

> **Note 2 to entry**: A ranked entity may also be referred to as an "assessment object" or "subject of ranking" in other standards and guidelines.
>

### 3.1.10 ranking cycle

**ranking cycle**

complete iteration of a ranking system from initiation of data collection to publication of results

> **Note 1 to entry**: A ranking cycle may be periodic (e.g., annual, biennial) or episodic (e.g., triggered by specific events or thresholds).
>

> **Note 2 to entry**: Changes in methodology between ranking cycles shall be documented and disclosed in accordance with Chapter 9.
>

**EXAMPLE** : The annual publication of the QS World University Rankings constitutes one ranking cycle per year.

### 3.1.11 transparency report

**transparency report**

document published by the ranking entity that discloses the methodology, data sources, weighting, scoring procedures, and known limitations of the ranking system in sufficient detail to enable stakeholders to assess its validity and fairness

> **Note 1 to entry**: The transparency report is the primary instrument for meeting the disclosure requirements of Chapter 9 and a primary audit artifact for the purposes of Chapter 10.
>

> **Note 2 to entry**: The transparency report shall be published concurrently with or prior to the publication of ranking results, not subsequently.
>

### 3.1.12 audit trail

**audit trail**

chronological record of all methodological decisions, data transformations, and computational steps that enables the reconstruction and verification of the ranking process from source data to published results

> **Note 1 to entry**: An audit trail includes but is not limited to: records of indicator selection decisions, weighting deliberations, data cleaning and transformation procedures, aggregation computations, and any post-hoc adjustments.
>

> **Note 2 to entry**: The audit trail is a critical component of the reproducibility requirement (see 3.1.17) and the audit provisions of Chapter 10.
>

### 3.1.13 conformance

**conformance**

fulfilment of a requirement of this standard by a ranking system

> **Note 1 to entry**: Conformance may be full (see 1.4.1) or partial (see 1.4.2).
>

> **Note 2 to entry**: Conformance is assessed through independent audit as specified in Chapter 10, except where self-assessment is permitted by the provisions of Chapter 11.
>

### 3.1.14 extension module

**extension module**

supplementary part of this standard that specifies domain-specific requirements applicable to a particular category of ranking systems, supplementing the core requirements

> **Note 1 to entry**: Extension modules are designated SE-01 through SE-09, each corresponding to a specific ranking domain as described in 1.1.1.
>

> **Note 2 to entry**: Conformance with an extension module is required only when a ranking system falls within the corresponding domain (see 1.4.2).
>

### 3.1.15 conflict of interest

**conflict of interest**

situation in which the ranking entity, its personnel, or any party involved in the ranking process has a financial, commercial, personal, or other interest that could, or could appear to, compromise the objectivity or impartiality of the ranking process or its results

> **Note 1 to entry**: Conflicts of interest may arise from commercial relationships between the ranking entity and ranked entities, from the ranking entity's financial dependence on revenue from ranked entities, or from personal relationships between assessors and assessed parties.
>

> **Note 2 to entry**: The identification, disclosure, and management of conflicts of interest are governed by the provisions of Chapter 4 (Principles) and Chapter 9 (Publication and Transparency).
>

**EXAMPLE** : A ranking entity that derives a significant portion of its revenue from consulting services sold to ranked entities has a financial conflict of interest.

### 3.1.16 sensitivity analysis

**sensitivity analysis**

systematic examination of how variations in inputs, assumptions, or methodological choices affect the outputs of a ranking system

> **Note 1 to entry**: Sensitivity analysis is used to assess the robustness of ranking results and to identify indicators or methodological choices that disproportionately influence outcomes.
>

> **Note 2 to entry**: This standard requires sensitivity analysis to be performed and documented as specified in Chapter 8.
>

**EXAMPLE** : Re-computing a ranking with weights varied by ±10% and observing the resulting changes in entity positions constitutes a basic sensitivity analysis.

### 3.1.17 reproducibility

**reproducibility**

ability of an independent party to obtain the same ranking results when applying the documented methodology to the same data, within the bounds of acceptable computational precision

> **Note 1 to entry**: Reproducibility is a necessary condition for the verifiability of a ranking system. It requires that the methodology be documented with sufficient precision and that the underlying data be accessible for verification purposes.
>

> **Note 2 to entry**: Reproducibility is distinct from replicability. Reproducibility refers to obtaining consistent results using the same data and methodology; replicability refers to obtaining consistent results using new data collected under the same protocol.
>

---

> **Note**: This chapter is part of ICO Std 2002 (Tianji Ranking Methodology Standard). The definitions in this chapter are normative. Terms used in this standard that are not defined herein retain their commonly understood meanings or the meanings assigned in the normative references listed in Chapter 2.
>
