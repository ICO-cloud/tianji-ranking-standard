# Chapter 8: Scoring and Ranking Methods

**ICO Std 2002:2026 — Chapter 8**

---

This chapter specifies the methods for scoring, normalising, aggregating, and ranking entities in a ranking system. It establishes requirements for the selection and documentation of scoring functions, the handling of ties and uncertainty, the verification of ranking results, and the standard format for ranking publication.

---

## 8.1 Scoring Methods

The ranking entity shall select a scoring method appropriate to the nature of the indicator and the ranking purpose. The following methods are recognised:

### 8.1.1 Linear Scoring

Linear scoring transforms the raw indicator value into a score through a linear function.

For a raw value *x* with defined minimum *x_min* and maximum *x_max*:

**Positive direction (higher is better)**:

$$S(x) = \frac{x - x_{\min}}{x_{\max} - x_{\min}} \times S_{\text{range}} + S_{\min}$$

**Negative direction (lower is better)**:

$$S(x) = \frac{x_{\max} - x}{x_{\max} - x_{\min}} \times S_{\text{range}} + S_{\min}$$

where $S_{\text{range}} = S_{\max} - S_{\min}$ is the score range.

**Applicability**: Linear scoring is appropriate when the relationship between the raw value and the underlying construct is approximately linear.

### 8.1.2 Piecewise Scoring

Piecewise scoring divides the range of raw values into segments and applies different scoring rules to each segment.

For a set of breakpoints $\{b_0, b_1, \ldots, b_k\}$ where $b_0 = x_{\min}$ and $b_k = x_{\max}$:

$$S(x) = S_j + \frac{x - b_j}{b_{j+1} - b_j} \times (S_{j+1} - S_j), \quad \text{for } b_j \leq x < b_{j+1}$$

where $S_j$ is the score assigned to breakpoint $b_j$.

**Applicability**: Piecewise scoring is appropriate when the marginal value of an additional unit of the indicator varies across the range (e.g., diminishing returns, threshold effects).

The ranking entity shall document the rationale for the choice of breakpoints and the scores assigned to each segment.

### 8.1.3 Percentile Ranking

Percentile ranking converts raw values into percentile positions based on the empirical distribution.

$$S(x) = \frac{\text{number of entities with value} \leq x}{m} \times 100$$

where *m* is the total number of ranked entities.

**Applicability**: Percentile ranking is appropriate when the absolute magnitude of the indicator is less meaningful than the relative position, or when the distribution is highly skewed.

> **Note**: Percentile ranking is non-linear and compresses the scale such that equal differences in percentile scores do not correspond to equal differences in the underlying attribute. The ranking entity shall disclose this property when percentile ranking is used.
>

### 8.1.4 Z-score Standardisation

Z-score standardisation transforms raw values into standard deviation units from the mean.

$$z_i = \frac{x_i - \bar{x}}{s}$$

where $\bar{x}$ is the sample mean and $s$ is the sample standard deviation.

**Applicability**: Z-score standardisation is appropriate when the indicator distribution is approximately normal and comparison across entities is based on relative deviation from the mean.

**Limitation**: Z-scores can be negative, which may be problematic for certain aggregation methods (e.g., geometric mean). The ranking entity shall address this limitation when using Z-scores in conjunction with such aggregation methods.

### 8.1.5 T-score Standardisation

T-score standardisation transforms Z-scores to a scale with a mean of 50 and a standard deviation of 10.

$$T_i = 10 \times z_i + 50$$

**Applicability**: T-score standardisation is appropriate when positive scores are required and a standardised scale is desired. It preserves the ordinal properties of Z-scores while eliminating negative values (for typical distributions where |z| < 5).

---

## 8.2 Normalisation Methods

Before aggregation, indicator values measured on different scales shall be normalised to a common scale. The ranking entity shall select a normalisation method appropriate to the data characteristics.

### 8.2.1 Min-Max Normalisation

Min-Max normalisation rescales values to a fixed interval, typically [0, 1] or [0, 100].

$$x'_i = \frac{x_i - x_{\min}}{x_{\max} - x_{\min}}$$

**Applicability**: Min-Max normalisation is appropriate when the minimum and maximum values are meaningful bounds and the distribution does not contain extreme outliers.

**Limitation**: Min-Max normalisation is sensitive to outliers, as a single extreme value can compress the remainder of the distribution.

### 8.2.2 Z-score Normalisation

Z-score normalisation (standardisation) transforms values to have a mean of 0 and a standard deviation of 1, as specified in 8.1.4.

**Applicability**: Z-score normalisation is appropriate when indicators have different scales and units, and the comparison of relative positions is more important than absolute levels.

### 8.2.3 Decimal Scaling Normalisation

Decimal scaling normalisation adjusts values by dividing by a power of 10.

$$x'_i = \frac{x_i}{10^j}$$

where *j* is the smallest integer such that $\max(|x'_i|) < 1$.

**Applicability**: Decimal scaling is appropriate when the indicator values span several orders of magnitude and a simple, interpretable scaling is desired.

### 8.2.4 Selection Criteria for Normalisation Methods

The ranking entity shall select the normalisation method based on the following criteria:

a) **Distributional characteristics**: If the indicator distribution is approximately normal, Z-score normalisation is preferred. If the distribution is bounded and without significant outliers, Min-Max normalisation is preferred.

b) **Outlier sensitivity**: If the indicator is prone to extreme outliers, Z-score normalisation or robust normalisation methods (e.g., median and MAD-based) should be used instead of Min-Max.

c) **Aggregation compatibility**: If the aggregation method requires non-negative inputs (e.g., geometric mean), a normalisation method that produces non-negative values shall be used, or the normalised values shall be shifted to a positive range.

d) **Interpretability**: The chosen method should produce scores that are interpretable for the intended users of the ranking.

The ranking entity shall document the normalisation method selected for each indicator and the rationale for the selection.

---

## 8.3 Composite Score Calculation

Composite scores aggregate normalised indicator scores into a single overall score for each ranked entity.

### 8.3.1 Weighted Arithmetic Mean (WAM)

The weighted arithmetic mean is the most common aggregation method:

$$C_i = \sum_{j=1}^{n} w_j \cdot s_{ij}$$

where $C_i$ is the composite score of entity *i*, $w_j$ is the weight of indicator *j*, and $s_{ij}$ is the normalised score of entity *i* on indicator *j*, subject to $\sum_{j=1}^{n} w_j = 1$.

**Applicability**: The WAM is appropriate when indicators are compensatory — i.e., a high score on one indicator can offset a low score on another.

**Limitation**: The WAM allows full compensation between indicators, which may not be appropriate when all indicators represent essential conditions.

### 8.3.2 Weighted Geometric Mean

The weighted geometric mean is:

$$G_i = \prod_{j=1}^{n} s_{ij}^{w_j}$$

where $s_{ij} > 0$ for all *i* and *j*, and $\sum_{j=1}^{n} w_j = 1$.

**Applicability**: The weighted geometric mean is appropriate when:

a) indicators are non-compensatory or partially compensatory — i.e., a low score on any indicator significantly reduces the composite score;

b) indicators are measured as ratios or multiplicative factors;

c) all indicator scores are strictly positive.

**Limitation**: The geometric mean requires all scores to be positive. It is more sensitive to low values than the arithmetic mean, which may be desirable or undesirable depending on the context.

### 8.3.3 Ordered Weighted Averaging (OWA)

The OWA operator applies weights to the ordered values of indicators rather than to specific indicators:

$$\text{OWA}_i = \sum_{j=1}^{n} v_j \cdot s_{i(j)}$$

where $s_{i(1)} \geq s_{i(2)} \geq \cdots \geq s_{i(n)}$ are the ordered scores of entity *i*, and $v_j$ are the order weights with $\sum_{j=1}^{n} v_j = 1$.

**Applicability**: OWA is appropriate when the ranking entity wishes to control the degree of compensation between indicators by adjusting the order weights:

a) Setting $v_1 = 1$ (all other $v_j = 0$) gives the maximum operator (optimistic aggregation).

b) Setting $v_n = 1$ (all other $v_j = 0$) gives the minimum operator (pessimistic aggregation).

c) Setting $v_j = 1/n$ gives the arithmetic mean (full compensation).

d) Setting $v_1 = v_n = 0.5$ gives the mid-range (average of best and worst).

### 8.3.4 Methodological Basis for Method Selection

The ranking entity shall document the methodological basis for selecting an aggregation method. The documentation shall include:

a) the theoretical relationship between the indicators (compensatory, non-compensatory, or partially compensatory);

b) the nature of the ranking purpose (whether excellence in all dimensions is required or whether compensatory trade-offs are acceptable);

c) the distributional properties of the indicator scores and their compatibility with the chosen method;

d) the results of robustness testing comparing alternative aggregation methods.

---

## 8.4 Ranking Rules

### 8.4.1 Primary Ranking Rule

Entities shall be ranked in descending order of their composite scores. The entity with the highest composite score shall receive rank 1.

$$R_i = 1 + |\{k : C_k > C_i\}|$$

where $R_i$ is the rank of entity *i* and $|\{k : C_k > C_i\}|$ is the number of entities with composite scores strictly greater than $C_i$.

### 8.4.2 Tie-Breaking Rules

When two or more entities have the same composite score, the following tie-breaking rules shall be applied in order:

a) **Step 1 — Highest-weighted indicator**: The entity with the higher score on the indicator with the greatest weight shall receive the higher rank.

b) **Step 2 — Second-highest-weighted indicator**: If the tie persists, the entity with the higher score on the indicator with the second-greatest weight shall receive the higher rank.

c) **Step 3 — Sequential application**: Steps 1 and 2 shall be repeated, proceeding through indicators in descending order of weight, until the tie is resolved.

d) **Step 4 — Shared rank**: If the tie cannot be resolved after applying all indicators, the tied entities shall share the same rank. The next rank(s) shall be skipped accordingly (e.g., if two entities share rank 5, the next entity receives rank 7).

The tie-breaking procedure shall be documented in the methodology and disclosed in the ranking publication.

### 8.4.3 Ranking Intervals and Confidence Intervals

The ranking entity should report uncertainty in the ranking positions, which may include:

a) **Ranking intervals**: A range of ranks within which an entity's true rank is expected to fall, given the uncertainty in the data and methodology.

b) **Confidence intervals**: Statistical confidence intervals for composite scores, estimated through methods such as bootstrapping.

$$\hat{C}_i \pm z_{\alpha/2} \cdot \hat{\text{se}}(\hat{C}_i)$$

where $\hat{\text{se}}(\hat{C}_i)$ is the estimated standard error of the composite score, typically obtained through bootstrap resampling.

c) **Overlap reporting**: The ranking entity should identify and report entities whose confidence intervals overlap, indicating that their rank differences are not statistically meaningful.

> **Note**: Ranking intervals and confidence intervals are particularly important for rankings that influence significant decisions (e.g., funding allocation, regulatory classification). Where such intervals are not reported, the ranking entity shall disclose this limitation.
>

---

## 8.5 Ranking Result Verification

The ranking entity shall verify the ranking results before publication using the methods specified in 8.5.1 through 8.5.3.

### 8.5.1 Internal Consistency Check

Internal consistency assesses whether the indicators in the ranking system measure a coherent underlying construct.

a) **Cronbach's alpha**: For ranking systems where indicators are expected to be correlated, Cronbach's alpha shall be computed:

$$\alpha = \frac{n}{n - 1} \left(1 - \frac{\sum_{j=1}^{n} s_j^2}{s_{\text{total}}^2}\right)$$

where *n* is the number of indicators, $s_j^2$ is the variance of indicator *j*, and $s_{\text{total}}^2$ is the variance of the total (sum) score.

b) **Threshold**: A Cronbach's alpha of at least 0.70 shall be achieved for the overall indicator system. Where the alpha is below 0.70, the ranking entity shall investigate the cause and consider indicator revision.

c) **Item-total correlation**: Each indicator's correlation with the total score (corrected for overlap) shall be reported. Indicators with corrected item-total correlation below 0.30 should be reviewed for potential removal.

### 8.5.2 External Validity Check

External validity assesses whether the ranking results are consistent with external benchmarks or criteria.

a) The ranking entity should compare the ranking results with at least one independent external benchmark, where such a benchmark exists.

b) The comparison method shall be documented, including the choice of benchmark, the correlation measure used (e.g., Spearman's ρ, Kendall's τ), and the interpretation of the results.

c) Where no suitable external benchmark exists, the ranking entity shall document this and shall instead rely on the internal consistency and robustness checks.

### 8.5.3 Robustness Check

Robustness checks assess whether the ranking results are stable under methodological variations.

The ranking entity shall conduct at least the following robustness checks:

a) **Bootstrap resampling**: The ranking shall be recomputed on a large number (at least 1 000) of bootstrap samples drawn with replacement from the original data. For each entity, the following shall be reported:

1) the mean rank across bootstrap samples;

2) the standard deviation of the rank across bootstrap samples;

3) the proportion of bootstrap samples in which the entity's rank falls within ±5 positions of the published rank.

b) **Method variation test**: The ranking shall be recomputed using at least one alternative aggregation method (e.g., if WAM is the primary method, geometric mean shall be tested as an alternative). The correlation between the primary and alternative rankings shall be reported.

c) **Data perturbation test**: The ranking shall be recomputed after adding random noise (within the estimated measurement error range) to the input data. The stability of the ranking shall be assessed.

---

## 8.6 Ranking Publication Format

### 8.6.1 Standard Ranking Table Format

The ranking shall be published in a tabular format that includes, at a minimum, the following columns:

| Column | Description |
|--------|-------------|
| Rank | The ordinal position of the entity |
| Entity identifier | The name or code of the ranked entity |
| Composite score | The overall composite score of the entity |
| Indicator scores | The score of the entity on each Level 1 indicator |

|---|---|

### 8.6.2 Sub-Score Disclosure

In addition to the standard ranking table, the ranking entity shall disclose:

a) the scores of each entity on all Level 2 indicators (sub-dimensions);

b) the normalised scores of each entity on all Level 3 indicators (specific measures), or the raw data from which these scores are derived.

> **Note**: Disclosure of Level 3 indicator scores may be provided in supplementary materials (e.g., downloadable data files) rather than in the primary publication, where the number of indicators makes tabular presentation impractical.
>

### 8.6.3 Methodology Summary Accompaniment

Each ranking publication shall be accompanied by a methodology summary that includes:

a) the standard identifier and version (e.g., ICO Std 2002:2026, Chapter 8, Version 1.0);

b) a brief description of the scoring method(s) used;

c) a brief description of the normalisation method(s) used;

d) a brief description of the aggregation method used;

e) the total number of ranked entities and the number of entities excluded from the ranking, with reasons for exclusion;

f) a reference to the full methodology documentation;

g) the date of publication;

h) the contact information for the ranking entity.

> **Note**: The purpose of the methodology summary is to enable users to understand the key methodological choices without reading the full documentation. The summary does not replace the full methodology disclosure required by 4.2.1.
>

---

> **Note**: The scoring and ranking methods specified in this chapter are intended to be domain-independent. Domain-specific scoring adjustments (e.g., industry-specific benchmarks, regional normalisation) shall be defined in the relevant extension module and shall comply with the core-layer requirements specified herein.
>