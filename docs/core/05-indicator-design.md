# Chapter 5: Indicator System Design

**ICO Std 2002:2026 — Chapter 5**

---

This chapter specifies the requirements for designing indicator systems used in ranking methodologies. It establishes rules for indicator selection, hierarchical organisation, validity verification, initial weight assignment, update mechanisms, and the relationship between core-layer and extension-layer indicators.

---

## 5.1 Indicator Selection Criteria

Each indicator included in a ranking system shall satisfy the criteria specified in 5.1.1 through 5.1.5. The ranking entity shall document the justification for each indicator's inclusion with reference to these criteria.

### 5.1.1 Relevance

An indicator shall be directly relevant to the ranking purpose as defined in the methodology. Relevance shall be established by demonstrating a logical or empirical link between the indicator and the attribute being measured.

a) The ranking entity shall define the conceptual domain that the ranking is intended to measure.

b) Each indicator shall map to at least one defined concept within that domain.

c) Indicators that are included solely due to data availability, without a demonstrated link to the ranking purpose, shall not be used.

### 5.1.2 Measurability

An indicator shall be measurable, either through quantitative measurement or through a defined coding scheme that permits consistent qualitative assessment.

a) Quantitative indicators shall have a defined unit of measurement and an unambiguous operational definition.

b) Qualitative indicators shall have a defined coding scheme with clearly distinguishable levels and coding rules.

c) Indicators for which no reliable measurement or coding procedure exists shall not be included until such a procedure is developed and validated.

### 5.1.3 Data Availability

Data required for an indicator shall be obtainable from accessible sources within a reasonable timeframe and at a reasonable cost, as specified in Chapter 7.

a) The ranking entity shall assess the availability of data for each proposed indicator before inclusion.

b) Where data availability varies significantly across ranked entities, the ranking entity shall evaluate whether the indicator introduces systematic bias (see 4.7).

### 5.1.4 Independence

Indicators within the same level of the hierarchy shall exhibit low mutual redundancy. The ranking entity shall assess the inter-correlation among indicators and take measures to reduce redundancy.

a) The pairwise correlation between indicators at the same hierarchical level shall be examined. Where the absolute value of the correlation coefficient exceeds 0.80, the ranking entity shall consider:

1) merging the correlated indicators into a single composite indicator;

2) removing one of the correlated indicators;

3) retaining both indicators with documented justification for their separate inclusion.

b) Multicollinearity among indicators shall be assessed using appropriate methods (e.g., variance inflation factor). Indicators with a variance inflation factor (VIF) exceeding 10 should be reviewed for potential removal or consolidation.

### 5.1.5 Robustness

An indicator shall be robust against the influence of outliers and measurement errors. The ranking entity shall:

a) test each indicator's sensitivity to outliers using appropriate methods (e.g., influence functions, trimmed means);

b) document the outlier handling procedure for each indicator (see also 7.4.2);

c) exclude indicators whose results are dominated by a small number of extreme observations, unless the extreme observations are substantively meaningful.

---

## 5.2 Indicator Hierarchy

The indicator system shall be organised into a hierarchical structure that reflects the logical decomposition of the ranking purpose into measurable components.

### 5.2.1 Hierarchical Levels

The indicator hierarchy shall consist of the following levels:

a) **Level 1 — Dimensions**: The broadest categories representing the major aspects of the ranking purpose. Level 1 indicators define the structural framework of the indicator system.

b) **Level 2 — Sub-dimensions**: More specific components within each dimension. Level 2 indicators decompose the dimensions into measurable aspects.

c) **Level 3 — Specific measures**: The most granular, directly measurable variables. Level 3 indicators are the operationalised variables for which data is collected.

### 5.2.2 Hierarchy Depth

The indicator hierarchy shall not exceed three levels. Where a ranking purpose requires more granular decomposition, the ranking entity shall:

a) consolidate the lower-level indicators into Level 3 composite measures; or

b) document the justification for exceeding three levels and obtain peer review approval (see 4.5.4).

### 5.2.3 Logical Relationships Between Levels

The relationship between indicators at adjacent levels shall be clearly defined:

a) Each Level 1 indicator shall be decomposable into at least two Level 2 indicators.

b) Each Level 2 indicator shall be decomposable into at least two Level 3 indicators.

c) The set of Level 2 indicators under a given Level 1 indicator shall collectively cover the conceptual scope of that Level 1 indicator.

d) The aggregation rule from lower to higher levels shall be specified (see Chapter 6 and Chapter 8).

---

## 5.3 Indicator Validity Verification

The ranking entity shall verify the validity of the indicator system before the first application and following any significant revision. Validity verification shall address the dimensions specified in 5.3.1 through 5.3.3.

### 5.3.1 Content Validity

Content validity assesses whether the indicator system adequately covers the conceptual domain it is intended to measure.

a) The ranking entity shall define the conceptual domain and its boundaries.

b) A panel of at least three domain experts shall evaluate whether the indicator system provides comprehensive coverage of the defined domain.

c) Gaps identified by the expert panel shall be addressed by adding indicators, revising existing indicators, or documenting the limitation.

### 5.3.2 Construct Validity

Construct validity assesses whether the indicators measure the theoretical constructs they are intended to measure.

a) The ranking entity shall apply appropriate statistical methods to assess construct validity, which may include:

1) exploratory or confirmatory factor analysis to examine whether indicators load onto the expected dimensions;

2) convergent validity analysis to assess whether indicators that should be related are in fact correlated;

3) discriminant validity analysis to assess whether indicators that should be distinct are in fact uncorrelated.

b) The results of construct validity analyses shall be documented, including any indicators that fail to conform to the expected structure and the actions taken.

### 5.3.3 Criterion Validity

Where an external criterion or gold standard exists, the ranking entity should assess criterion validity by examining the correlation between the ranking results and the external criterion.

a) The external criterion shall be independent of the ranking system being validated.

b) The ranking entity shall document the choice of external criterion and the rationale for its selection.

c) Where no suitable external criterion exists, the ranking entity shall document this limitation and the alternative validation methods employed.

### 5.3.4 Validation Documentation

The results of all validity verification analyses shall be documented in the methodology report. The documentation shall include:

a) the methods used and their assumptions;

b) the data and sample on which the analysis was conducted;

c) the results, including statistical test values and their interpretation;

d) any limitations identified and the actions taken to address them.

---

## 5.4 Initial Weight Assignment

Prior to the formal weight determination process (see Chapter 6), the ranking entity shall establish an initial weight scheme. The initial weight scheme serves as a starting point for stakeholder consultation and sensitivity analysis.

### 5.4.1 Equal Weighting

Where no strong theoretical or empirical basis exists for differential weighting, the ranking entity shall use equal weighting as the initial scheme. Under equal weighting, all indicators at the same hierarchical level receive the same weight.

For *n* indicators at a given level, the equal weight for each indicator *i* is:

$$w_i = \frac{1}{n}, \quad i = 1, 2, \ldots, n$$

where $\sum_{i=1}^{n} w_i = 1$.

> **Note**: Equal weighting does not imply equal importance; it reflects the absence of a defensible basis for differential weighting. The ranking entity should seek to establish a more informed weighting scheme through the methods described in Chapter 6.
>

### 5.4.2 Delphi Method

The Delphi method may be used to derive initial weights through structured expert consultation. The process shall include:

a) selection of a panel of at least five domain experts;

b) at least two rounds of anonymous expert assessment;

c) provision of statistical feedback (median and interquartile range) between rounds;

d) convergence criteria (e.g., interquartile range below a defined threshold) to determine when sufficient consensus is reached.

### 5.4.3 Analytic Hierarchy Process (AHP)

The Analytic Hierarchy Process may be used to derive initial weights through pairwise comparison of indicators. The AHP process shall comply with the following requirements:

a) Pairwise comparison matrices shall be constructed for indicators at each level of the hierarchy.

b) The consistency ratio (CR) of each comparison matrix shall not exceed 0.10. Where CR > 0.10, the expert shall revise the comparisons.

c) The priority vectors derived from the comparison matrices shall be normalised to sum to 1.

### 5.4.4 Principal Component Analysis (PCA)

PCA may be used as a data-driven method to inform initial weight assignment. When PCA is used for this purpose:

a) The ranking entity shall report the proportion of variance explained by each retained component.

b) Weights derived from PCA loadings shall be interpreted with caution and validated against domain knowledge, as PCA-derived weights reflect data structure rather than substantive importance.

c) The ranking entity shall document the number of components retained and the retention criteria used.

### 5.4.5 Relationship Between Initial and Final Weights

The initial weight scheme is provisional and shall be subject to the full weight determination process specified in Chapter 6. The final weights may differ from the initial weights as a result of:

a) stakeholder consultation;

b) sensitivity analysis (see 6.3);

c) methodological refinement.

The ranking entity shall document the difference between initial and final weights and the reasons for any significant changes.

---

## 5.5 Indicator Update Mechanism

The indicator system shall be subject to periodic review and, where necessary, updated to ensure its continued relevance and validity.

### 5.5.1 Review Cycle

The ranking entity shall conduct a formal review of the indicator system at intervals not exceeding five years. The review shall assess:

a) whether the indicators remain relevant to the ranking purpose;

b) whether the data landscape has changed significantly;

c) whether new indicators should be added or existing indicators removed;

d) whether the validity of the indicator system has been maintained (see 5.3).

### 5.5.2 Trigger Conditions for Indicator Changes

In addition to the periodic review, an indicator review shall be triggered by:

a) a material change in the ranking purpose or scope;

b) the permanent unavailability of a data source relied upon by one or more indicators;

c) the publication of significant new research that challenges the validity or relevance of an indicator;

d) the identification of systematic bias attributable to an indicator (see 4.7).

### 5.5.3 Indicator Change Process

Any change to the indicator system shall follow a documented process that includes:

a) a proposal documenting the change and its rationale;

b) an impact assessment of the proposed change on the ranking results;

c) a consultation period allowing stakeholder input of no less than 30 calendar days;

d) a decision by the ranking entity with documented justification;

e) public announcement of the change at least one ranking cycle before implementation, unless the change is required to address a compliance or ethical issue.

### 5.5.4 Version Management

Each version of the indicator system shall be uniquely identified. The version identifier shall include:

a) a version number following a defined schema (e.g., major.minor);

b) the effective date;

c) a summary of changes from the previous version.

All prior versions of the indicator system shall be archived and accessible for audit purposes.

---

## 5.6 Extension Module Indicator Reference Rules

This standard adopts a two-layer architecture: the core layer (this chapter and Chapters 4 through 8) defines methodology requirements applicable to all ranking domains; extension layers define domain-specific indicators and rules.

### 5.6.1 Core-Layer Indicator Design Methodology

The core layer defines the general methodology for indicator selection, hierarchy design, validity verification, weight assignment, and update management. This methodology applies universally, regardless of the ranking domain.

### 5.6.2 Extension-Layer Domain-Specific Indicators

Extension modules may define domain-specific indicators that are not covered by the core layer. Such indicators shall:

a) satisfy all selection criteria specified in 5.1;

b) conform to the hierarchy rules specified in 5.2;

c) undergo validity verification as specified in 5.3;

d) be subject to the update mechanism specified in 5.5.

### 5.6.3 Validation of Extension-Layer Indicators

Extension-layer indicators shall be validated using the methodology specified in this chapter. The validation shall be documented in the extension module and shall be subject to the same transparency requirements as core-layer indicators.

a) The ranking entity shall verify that extension-layer indicators do not conflict with the principles specified in Chapter 4.

b) Where extension-layer indicators employ domain-specific measurement methods, those methods shall be documented with sufficient detail to permit independent verification.

c) The results of extension-layer indicator validation shall be referenced in the core methodology documentation.

---

> **Note**: The two-layer architecture enables domain flexibility while maintaining methodological consistency. Extension modules should reference this chapter explicitly and declare their compliance with the core-layer requirements, rather than re-specifying the requirements.
>
