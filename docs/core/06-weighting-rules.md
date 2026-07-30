# Chapter 6: Weighting Rules

**ICO Std 2002:2026 — Chapter 6**

---

This chapter specifies the methods, procedures, and requirements for assigning weights to indicators in a ranking system. It establishes rules for weight determination, sensitivity analysis, disclosure, prohibited practices, and cross-domain weight coordination.

---

## 6.1 Weight Assignment Methods

The ranking entity shall select a weight assignment method from those specified in 6.1.1 through 6.1.4, or a combination thereof, and shall document the rationale for the selection (see 6.2.1).

### 6.1.1 Equal Weighting

Equal weighting assigns the same weight to all indicators at a given hierarchical level.

For *n* indicators at level *k*, the weight of indicator *i* is:

$$w_i^{(k)} = \frac{1}{n}, \quad i = 1, 2, \ldots, n; \quad \sum_{i=1}^{n} w_i^{(k)} = 1$$

**Applicability**:

a) Where no defensible theoretical or empirical basis exists for differential weighting.

b) As a baseline for sensitivity analysis (see 6.3).

c) For ranking systems with a small number of indicators (typically *n* ≤ 5) where the indicators represent equally important dimensions.

**Limitations**:

a) Equal weighting implicitly assumes that all indicators contribute equally to the ranking purpose, which is rarely the case in practice.

b) Equal weighting does not account for differences in indicator reliability or variance.

c) When indicators have different numbers of sub-indicators, equal weighting at the dimension level may introduce indirect weighting bias at the sub-indicator level.

### 6.1.2 Expert-Based Weighting

Expert-based weighting methods derive weights from the informed judgement of domain experts. The following methods are recognised:

#### 6.1.2.1 Delphi Method

The Delphi method derives weights through iterative, anonymous expert consultation with controlled feedback. The requirements specified in 5.4.2 shall apply, with the following additional requirements:

a) The expert panel shall include at least seven members for weight determination.

b) At least three rounds of consultation shall be conducted.

c) The final weights shall be calculated as the median of the experts' final-round estimates.

d) The dispersion of expert judgements (interquartile range) shall be reported.

#### 6.1.2.2 Analytic Hierarchy Process (AHP)

The AHP derives weights from pairwise comparisons of indicator importance. The requirements specified in 5.4.3 shall apply, with the following additional requirements:

a) The pairwise comparison scale shall follow the Saaty 1–9 scale.

b) The consistency ratio (CR) shall be calculated for each comparison matrix. A matrix with CR > 0.10 shall be revised.

c) When multiple experts participate, individual priority vectors shall be aggregated using the geometric mean method.

### 6.1.3 Data-Driven Weighting

Data-driven weighting methods derive weights from the statistical properties of the data. The following methods are recognised:

#### 6.1.3.1 Principal Component Analysis (PCA)

PCA-derived weights are obtained from the factor loadings of the first principal component or from the proportion of variance explained by each indicator. The requirements specified in 5.4.4 shall apply.

#### 6.1.3.2 Factor Analysis

Factor analysis may be used to derive weights from the factor structure of the indicator data. When factor analysis is used for weighting:

a) The factor extraction method (e.g., maximum likelihood, principal axis factoring) shall be documented.

b) The factor rotation method (if any) shall be documented.

c) Factor scores shall be used to derive weights only after confirming the theoretical meaningfulness of the factor structure.

#### 6.1.3.3 Entropy Method

The entropy method derives weights from the information entropy of each indicator, assigning higher weights to indicators with greater variation. The entropy weight for indicator *j* is calculated as:

Step 1: Normalise the data:

$$p_{ij} = \frac{x_{ij}}{\sum_{i=1}^{m} x_{ij}}$$

where *x_{ij}* is the value of indicator *j* for entity *i*, and *m* is the number of entities.

Step 2: Calculate the entropy of indicator *j*:

$$e_j = -\frac{1}{\ln m} \sum_{i=1}^{m} p_{ij} \ln(p_{ij})$$

Step 3: Calculate the weight:

$$w_j = \frac{1 - e_j}{\sum_{j=1}^{n} (1 - e_j)}$$

where *n* is the number of indicators.

> **Note**: The entropy method reflects the discriminative power of each indicator but does not capture substantive importance. It should be used in conjunction with expert judgement or as a validation tool rather than as the sole basis for weight assignment.
>

### 6.1.4 Hybrid Weighting

Hybrid weighting combines two or more of the methods specified in 6.1.1 through 6.1.3. The ranking entity shall document:

a) the methods combined and the combination formula;

b) the rationale for the combination;

c) the contribution of each method to the final weights.

A common hybrid approach is to combine expert-based and data-driven weights:

$$w_j = \alpha \cdot w_j^{\text{expert}} + (1 - \alpha) \cdot w_j^{\text{data}}, \quad \alpha \in [0, 1]$$

where $\alpha$ is the blending parameter, $w_j^{\text{expert}}$ is the expert-derived weight, and $w_j^{\text{data}}$ is the data-driven weight. The value of $\alpha$ shall be justified and documented.

---

## 6.2 Weight Determination Process

The determination of final weights shall follow a structured process that ensures rigour, transparency, and stakeholder involvement.

### 6.2.1 Methodology Selection Documentation

The ranking entity shall document the following before proceeding with weight determination:

a) the weight assignment method selected (from 6.1);

b) the rationale for the selection, including:

1) the theoretical considerations supporting the choice;

2) the data characteristics relevant to the choice;

3) the practical constraints influencing the choice.

c) any alternative methods considered and the reasons for their rejection.

### 6.2.2 Stakeholder Participation Rules

Stakeholders shall have the opportunity to provide input on the weight assignment. The following rules shall apply:

a) The ranking entity shall publish the proposed initial weight scheme and invite stakeholder comments for a period of no less than 30 calendar days.

b) Stakeholder comments shall be documented, including the disposition of each comment (accepted, partially accepted, or rejected with rationale).

c) Representatives of ranked entities shall not have decision-making authority over the final weights.

d) The ranking entity shall maintain a record of all stakeholder interactions related to weight determination.

### 6.2.3 Transparency of the Weight Determination Process

The entire weight determination process shall be transparent. The ranking entity shall:

a) publish the weight determination methodology before its application;

b) disclose all intermediate results (e.g., expert panel responses, factor loadings, entropy values);

c) provide a clear audit trail from initial weights to final weights.

---

## 6.3 Sensitivity Analysis Requirements

The ranking entity shall conduct sensitivity analysis on the weights to assess the robustness of the ranking results.

### 6.3.1 Mandatory Sensitivity Analysis

The ranking entity shall perform at least the following sensitivity analyses:

a) **±10 % weight variation test**: Each weight shall be individually increased and decreased by 10 percentage points (redistributing the difference proportionally among the remaining weights). The impact on the ranking of each entity shall be recorded.

b) **Extreme weight scenario test**: The ranking shall be computed with each weight individually set to zero (redistributing to other weights) and with each weight individually set to dominate (≥ 50 % of total weight). The impact on the ranking shall be recorded.

c) **Equal weight comparison**: The ranking produced by the final weights shall be compared with the ranking produced by equal weights. The correlation between the two rankings (e.g., Spearman's ρ) and the number and magnitude of rank changes shall be reported.

### 6.3.2 Reporting of Sensitivity

The ranking entity shall report:

a) the overall sensitivity of the ranking to weight changes, expressed as:

1) the average rank change across all ranked entities;

2) the maximum rank change for any single entity;

3) the proportion of entities whose rank changes by more than 5 positions (or 10 % of the total number of ranked entities, whichever is greater).

b) the identification of entities whose ranking is highly sensitive to weight changes, which shall be flagged in the publication.

> **Note**: If the sensitivity analysis reveals that the ranking is highly sensitive to small weight changes (e.g., average rank change > 10 positions under ±10% weight variation), the ranking entity should review the indicator system for potential redundancy or instability and should consider increasing the number of data points or improving indicator quality.
>

---

## 6.4 Weight Disclosure Requirements

### 6.4.1 Full Weight Disclosure

All indicator weights shall be publicly disclosed in the ranking publication. The disclosure shall include:

a) the numerical value of each weight, reported to at least three decimal places;

b) the hierarchical level at which each weight applies;

c) the sum of weights at each hierarchical level (which shall equal 1.000).

### 6.4.2 Weight Methodology Disclosure

The method used to determine the weights shall be disclosed, including:

a) the name and description of the method;

b) the data and inputs used in the weight determination process;

c) the key parameters and assumptions of the method;

d) the results of any sensitivity analysis (see 6.3).

### 6.4.3 Weight Change Disclosure

When the weights differ from those used in the previous ranking cycle, the ranking entity shall:

a) disclose the previous and current weights side by side;

b) provide a reasoned explanation for each weight change that exceeds ±0.01 in absolute terms;

c) report the impact of the weight changes on the ranking results, including the number of entities that changed rank by more than 5 positions.

---

## 6.5 Prohibited Practices

The following practices are prohibited under this standard:

### 6.5.1 Commercially Motivated Weight Adjustment

Weights shall not be adjusted to favour any ranked entity for commercial benefit to the ranking entity or any affiliated party. This includes, but is not limited to:

a) increasing the weight of indicators on which a paying entity scores highly;

b) decreasing the weight of indicators on which a paying entity scores poorly;

c) creating or modifying indicators and their weights to accommodate sponsorship or advertising agreements.

### 6.5.2 Entity-Specific Weight Customisation

The weight scheme shall be uniform across all ranked entities. It is prohibited to:

a) apply different weights to different ranked entities;

b) select weights that are optimised for a specific entity's data profile;

c) adjust weights post hoc based on preliminary ranking results.

### 6.5.3 Intra-Cycle Weight Modification

Once the weight scheme for a ranking cycle has been finalised and published, it shall not be modified within that cycle. Any necessary changes shall be implemented in the next cycle, following the process specified in 6.2 and 5.5.

> **Note**: The prohibition in 6.5.3 does not preclude the correction of computational errors; however, any such correction shall be documented and disclosed in accordance with the transparency requirements of 4.2.
>

---

## 6.6 Cross-Domain Weight Coordination

### 6.6.1 Core-Layer Weight Methodology Uniformity

The weight assignment methodology specified in this chapter shall apply uniformly across all ranking domains covered by this standard. This ensures that:

a) all ranking systems under this standard employ a consistent methodological framework for weight determination;

b) the validity and comparability of weighting practices are maintained across domains;

c) users can understand and compare the weighting approaches of different ranking systems without needing to learn domain-specific conventions.

### 6.6.2 Extension-Layer Domain Weight Independence

Within the methodological framework defined by the core layer, extension modules may define domain-specific weighting practices that reflect the substantive characteristics of the domain. Such practices shall:

a) comply with the general requirements of this chapter;

b) justify any deviations from the core-layer default practices;

c) be documented in the extension module with reference to this chapter.

### 6.6.3 Weight Standardisation for Cross-Domain Comparison

Where ranking results from different domains are compared or aggregated, the following standardisation rules shall apply:

a) Weights shall be normalised to a common scale (summing to 1) before comparison.

b) The weight determination method shall be the same or equivalent in terms of methodological rigour. Where methods differ, the comparison shall note this limitation.

c) Cross-domain comparison shall not be used to imply that entities ranked in different domains are directly comparable on the same scale.

> **Note**: Cross-domain comparison of ranking results requires careful interpretation. Differences in indicator systems, data availability, and domain conventions may limit the meaningfulness of such comparisons, even when weight standardisation is applied.
>
