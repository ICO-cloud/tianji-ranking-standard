# Annex C: Application Examples

**ICO Std 2002 — Annex C (Informative)**

---

## Purpose

This annex provides illustrative examples of applying ICO Std 2002 across different ranking domains. Each example demonstrates the standard's practical application by walking through the complete ranking lifecycle — from indicator design and weighting to data collection, scoring, and publication. These examples are **illustrative only** and do not represent actual ranking results.

ICO Std 2002。——、——。，。

> **Disclaimer**: The indicator systems, weights, data, and scores used in these examples are hypothetical and are provided solely for the purpose of illustrating the application of ICO Std 2002. They should not be interpreted as actual rankings or evaluations of any real entity, product, or heritage item.
> ：、、，ICO Std 2002。、。

---

## C.1 Example 1: Intangible Cultural Heritage (ICH) Ranking

### C.1.1 Scenario Description

A ranking entity wishes to develop a ranking of intangible cultural heritage (ICH) elements within a specific country, evaluating their safeguarding status, community vitality, and transmission effectiveness. The ranking is intended to inform policy-makers, cultural organisations, and the public about the state of ICH safeguarding, consistent with the UNESCO Convention for the Safeguarding of the Intangible Cultural Heritage (2003).

（ICH），、。、ICH，《》（2003）。

**Applicable standard provisions** | : ICO Std 2002 core layer (§04–§11) and SE-05 (Cultural Heritage) extension module.

### C.1.2 Process Flow Diagram

```
┌─────────────────────────────────────────────────────────────────┐
│  STEP 1: Purpose & Scope Definition (§04, §01)                  │
│                                                     │
│  - Define: ICH safeguarding assessment                          │
│  - Target: Policy-makers, cultural organisations, public       │
│  - Domain: SE-05 (Cultural Heritage)                            │
└───────────────────────────┬─────────────────────────────────────┘
┌─────────────────────────────────────────────────────────────────┐
│  STEP 2: Indicator System Design (§05)                           │
│                                                       │
│  - Level 1: 4 dimensions                                        │
│  - Level 2: 12 sub-dimensions                                   │
│  - Level 3: 36 specific measures                                │
└───────────────────────────┬─────────────────────────────────────┘
┌─────────────────────────────────────────────────────────────────┐
│  STEP 3: Weight Assignment (§06)                                 │
│                                                          │
│  - AHP-based expert weighting                                    │
│  - Sensitivity analysis of weight variations                    │
└───────────────────────────┬─────────────────────────────────────┘
┌─────────────────────────────────────────────────────────────────┐
│  STEP 4: Data Collection (§07)                                   │
│                                                          │
│  - Tier 1: Official ICH registries, government statistics       │
│  - Tier 2: Expert surveys, community interviews                 │
│  - Tier 3: Publicly available media reports                     │
└───────────────────────────┬─────────────────────────────────────┘
┌─────────────────────────────────────────────────────────────────┐
│  STEP 5: Scoring & Ranking (§08)                                 │
│                                                        │
│  - Normalisation: Min-max method                                │
│  - Aggregation: Weighted arithmetic mean (WAM)                  │
│  - Robustness: Bootstrap resampling (1000 iterations)           │
└───────────────────────────┬─────────────────────────────────────┘
┌─────────────────────────────────────────────────────────────────┐
│  STEP 6: Publication & Audit (§09, §10)                          │
│                                                        │
│  - Transparency Level 3 (Data Transparency)                     │
│  - Internal audit + external peer review                        │
└─────────────────────────────────────────────────────────────────┘
```

### C.1.3 Indicator System

#### Level 1 Indicators (Dimensions)

| ID | Dimension | Weight | Description 
| ---- | ----------- | -------- | ------------- 
| D1 | Safeguarding Status | 0.30 | Measures the formal recognition and institutional support for the ICH element 
| D2 | Community Vitality | 0.30 | Measures the active engagement of the bearer community in sustaining the ICH element 
| D3 | Transmission Effectiveness | 0.25 | Measures the effectiveness of inter-generational transmission 
| D4 | Public Awareness & Influence | 0.15 | Measures the broader public awareness and cultural influence of the ICH element 

#### Level 2 Indicators (Sub-dimensions)

| ID | Sub-dimension | Parent | Weight (within parent) | Description 
| ---- | -------------- | -------- | ---------------------- | ------------- 
| D1.1 | Registry status | D1 | 0.35 | Whether the element is inscribed on national/international ICH lists 
| D1.2 | Safeguarding plan | D1 | 0.35 | Existence and quality of safeguarding plans 
| D1.3 | Funding support | D1 | 0.30 | Level of financial support for safeguarding activities 
| D2.1 | Practitioner count | D2 | 0.30 | Number of active practitioners/transmitters 
| D2.2 | Community engagement | D2 | 0.35 | Level of community participation in ICH practices 
| D2.3 | Practice continuity | D2 | 0.35 | Continuity of practice over time (no significant interruptions) 
| D3.1 | Apprenticeship system | D3 | 0.35 | Existence and functioning of formal/informal apprenticeship systems 
| D3.2 | Youth involvement | D3 | 0.35 | Proportion of practitioners under 35 years of age 
| D3.3 | Knowledge documentation | D3 | 0.30 | Completeness of documentation of ICH knowledge and techniques 
| D4.1 | Media coverage | D4 | 0.35 | Volume and quality of media coverage 
| D4.2 | Educational integration | D4 | 0.35 | Integration into formal and informal education 
| D4.3 | Cultural tourism impact | D4 | 0.30 | Contribution to cultural tourism (as a measure of public interest) 

#### Level 3 Indicators (Specific Measures) — Selected Examples

| ID | Measure | Parent | Data Source Tier | Measurement Method 
| ---- | --------- | -------- | ----------------- | ------------------- 
| D1.1.1 | National ICH list inscription | D1.1 | Tier 1 | Binary (1 = inscribed, 0 = not) + tier of inscription (national/international) 
| D1.1.2 | UNESCO ICH list inscription | D1.1 | Tier 1 | Binary (1 = inscribed, 0 = not) 
| D1.2.1 | Safeguarding plan existence | D1.2 | Tier 1 | Binary (1 = exists, 0 = not) 
| D1.2.2 | Safeguarding plan quality score | D1.2 | Tier 2 | Expert assessment on 1–5 scale (rubric-based) 
| D2.1.1 | Number of active practitioners | D2.1 | Tier 1 | Count from official registry or survey 
| D2.2.1 | Community participation rate | D2.2 | Tier 2 | Survey-based estimate (% of community members participating) 
| D3.2.1 | Proportion of practitioners under 35 | D3.2 | Tier 1 | Demographic data from registry/survey 
| D4.1.1 | Annual media mentions | D4.1 | Tier 3 | Count from media database search 

### C.1.4 Weight Assignment

Weights were determined using the Analytic Hierarchy Process (AHP) with a panel of 12 ICH experts (§06.1.2 — Expert Panel Method). The AHP process involved:

（AHP），12ICH（§06.1.2——）。AHP：

a) pairwise comparison of Level 1 dimensions by each expert;

b) aggregation of individual judgments using the geometric mean;

c) calculation of priority weights from the aggregate comparison matrix;

d) consistency check (consistency ratio CR < 0.10 for all experts).
（CR < 0.10）。

**Resulting Level 1 Weights** | :

$$w_{D1} = 0.30, \quad w_{D2} = 0.30, \quad w_{D3} = 0.25, \quad w_{D4} = 0.15$$

### C.1.5 Data Collection |

Data collection followed the three-tier classification system (§7.1):

（§7.1）：

| Data Source Tier | Proportion of Data Points | Examples 
|-----------------|--------------------------|----------
| Tier 1 (Official/Audited) | 65% | National ICH registry, UNESCO lists, government funding records 
| Tier 2 (Survey/Expert) | 30% | Expert assessment of safeguarding plan quality, community surveys 
| Tier 3 (Unverified/Public) | 5% | Media database searches, public web sources 

**Data quality metrics** |  (§7.3):

- Accuracy rate: 94% (Tier 1 data verified against original sources)
- Completeness rate: 87% (13% of data points missing, handled by §7.4.1 methods)
- Timeliness index: 91% (data within the declared reference period)

### C.1.6 Scoring and Ranking |

**Normalisation** |  (§8.2):

Min-max normalisation was applied to all quantitative indicators:

-：

$$s_{ij} = \frac{x_{ij} - \min_k x_{kj}}{\max_k x_{kj} - \min_k x_{kj}}$$

For qualitative indicators (expert assessments on 1–5 scale), scores were normalised to the [0, 1] interval:

$$s_{ij} = \frac{x_{ij} - 1}{5 - 1}$$

**Aggregation** |  (§8.3.1):

The weighted arithmetic mean (WAM) was used for aggregation:

（WAM）：

$$C_i = \sum_{j=1}^{n} w_j \cdot s_{ij}$$

**Illustrative Scoring Results** |  (hypothetical data for 5 ICH elements):

| Rank | ICH Element | D1 (0.30) | D2 (0.30) | D3 (0.25) | D4 (0.15) | Composite Score 
| ------ | ------------- | ----------- | ----------- | ----------- | ----------- | ---------------- 
| 1 | Traditional Silk Weaving | 0.89 | 0.85 | 0.82 | 0.78 | 0.846 
| 2 | Dragon Boat Festival | 0.92 | 0.78 | 0.76 | 0.85 | 0.828 
| 3 | Ceramic Firing Technique | 0.75 | 0.82 | 0.71 | 0.62 | 0.746 
| 4 | Folk Music Tradition | 0.68 | 0.65 | 0.72 | 0.58 | 0.662 
| 5 | Traditional Paper-cutting | 0.71 | 0.55 | 0.48 | 0.65 | 0.588 

**Robustness Check** |  (§8.5.3):

Bootstrap resampling (1,000 iterations) was conducted. Results:

- Mean rank standard deviation across bootstrap samples: 0.3 positions
- Proportion of elements with rank within ±1 of published rank: 92%
- Geometric mean aggregation (alternative method) correlation with WAM: Spearman's ρ = 0.96

### C.1.7 Publication and Audit

The ranking was published at **Transparency Level 3** (Data Transparency, §9.2.3), including:

a) full methodology documentation;

b) all Level 1 and Level 2 indicator scores;

c) downloadable data files with Level 3 indicator scores;

d) robustness analysis results;

e) limitations disclosure (§9.1.4), including the caveat that the ranking measures safeguarding status and should not be used as the sole basis for funding allocation.

---

## C.2 Example 2: Consumer Product Quality Ranking

### C.2.1 Scenario Description

A ranking entity wishes to develop a quality ranking for a specific consumer product category (e.g., smartphones). The ranking evaluates products based on objective quality measures, user experience, and value for money. The ranking must address the significant risk of data manipulation (e.g., fake reviews,) that is prevalent in consumer product rankings.

**Applicable standard provisions** | : ICO Std 2002 core layer (§04–§11) and SE-01 (Products) extension module.

### C.2.2 Process Flow Diagram

```
┌─────────────────────────────────────────────────────────────────┐
│  STEP 1: Purpose & Scope Definition (§04, §01)                  │
│                                                     │
│  - Define: Consumer product quality assessment                  │
│  - Target: Consumers, manufacturers, regulators                │
│  - Domain: SE-01 (Products)                                     │
└───────────────────────────┬─────────────────────────────────────┘
┌─────────────────────────────────────────────────────────────────┐
│  STEP 2: Category-Differentiated Indicator Design (§05)          │
│                                                  │
│  - Core indicators (common across categories)                   │
│  - Category-specific indicators (unique to product type)        │
│  - Anti-fraud indicators (§7.5)                                 │
└───────────────────────────┬─────────────────────────────────────┘
┌─────────────────────────────────────────────────────────────────┐
│  STEP 3: Weight Assignment with Category Adjustment (§06)        │
│                                                    │
│  - Base weights from AHP                                        │
│  - Category-specific adjustments (documented)                   │
└───────────────────────────┬─────────────────────────────────────┘
┌─────────────────────────────────────────────────────────────────┐
│  STEP 4: Data Collection with Anti-Fraud Measures (§07, §7.5)    │
│                                              │
│  - Tier 1: Laboratory test results, certification data          │
│  - Tier 2: Verified user surveys, expert assessments            │
│  - Tier 3: E-commerce reviews (with fraud detection)            │
│  - Anti-fraud: Bot detection, duplicate filtering, outlier flag │
└───────────────────────────┬─────────────────────────────────────┘
┌─────────────────────────────────────────────────────────────────┐
│  STEP 5: Scoring, Ranking & Anti-Brushing Adjustment (§08)       │
│  、                                            │
│  - Normalisation: Z-score standardisation                       │
│  - Aggregation: WAM with anti-fraud penalty                     │
│  - Robustness: Method variation + data perturbation             │
└───────────────────────────┬─────────────────────────────────────┘
┌─────────────────────────────────────────────────────────────────┐
│  STEP 6: Publication & Audit (§09, §10)                          │
│                                                        │
│  - Transparency Level 2 (Methodology Transparency)              │
│  - Anti-fraud audit trail                                       │
└─────────────────────────────────────────────────────────────────┘
```

### C.2.3 Indicator System

#### Level 1 Indicators

| ID | Dimension | Weight | Description 
| ---- | ----------- | -------- | ------------- 
| P1 | Product Performance | 0.35 | Objective technical performance measures 
| P2 | User Experience | 0.30 | Subjective and objective user experience measures 
| P3 | Value for Money | 0.20 | Quality relative to price 
| P4 | Brand Reliability | 0.15 | Brand reputation, after-sales service, warranty 

#### Level 2 Indicators — Category-Specific (Smartphones)

| ID | Sub-dimension | Parent | Weight (within parent) | Measurement 
| ---- | -------------- | -------- | ---------------------- | ------------- 
| P1.1 | Processor performance | P1 | 0.25 | Benchmark score (Tier 1: lab test) 
| P1.2 | Display quality | P1 | 0.20 | Colour accuracy, brightness, resolution (Tier 1) 
| P1.3 | Camera quality | P1 | 0.25 | DxOMark or equivalent score (Tier 1) 
| P1.4 | Battery life | P1 | 0.20 | Standardised battery test (Tier 1) 
| P1.5 | Build quality | P1 | 0.10 | Durability test score (Tier 1) 
| P2.1 | User satisfaction score | P2 | 0.40 | Verified user survey (Tier 2) 
| P2.2 | Ease of use | P2 | 0.30 | Expert assessment (Tier 2) 
| P2.3 | Software experience | P2 | 0.30 | Expert assessment (Tier 2) 
| P3.1 | Performance-to-price ratio | P3 | 0.60 | Composite score / retail price (Tier 1) 
| P3.2 | Feature completeness | P3 | 0.40 | Feature count vs. category average (Tier 1) 
| P4.1 | Brand reputation index | P4 | 0.40 | Brand evaluation score (Tier 2) 
| P4.2 | After-sales service quality | P4 | 0.35 | Customer service satisfaction survey (Tier 2) 
| P4.3 | Warranty coverage | P4 | 0.25 | Warranty terms and coverage (Tier 1) 

### C.2.4 Anti-Fraud Mechanisms

Consumer product rankings are particularly vulnerable to data manipulation. The following anti-fraud measures are applied in accordance with §7.5:

**a) Tier 3 Data Fraud Detection** |

For e-commerce review data (Tier 3), the following detection algorithms are applied:

1. **Duplicate detection** | : Reviews with identical or near-identical text are flagged and excluded. Detection threshold: Jaccard similarity > 0.85.
。：Jaccard > 0.85。

2. **Temporal clustering detection** | : Unusual spikes in review volume (e.g., >3 standard deviations above the mean daily rate) are flagged for manual review.

3. **Account age and activity filter** | : Reviews from accounts with <30 days of registration or <3 prior reviews are excluded from the scoring calculation.

**b) Anti-Brushing Penalty** |

If a product is found to have a statistically significant proportion of fraudulent reviews (as determined by the fraud detection algorithms above), the following penalty is applied:

$$s_{ij}^{\text{adjusted}} = s_{ij} \times (1 - \lambda \cdot p_{\text{fraud}})$$

where $p_{\text{fraud}}$ is the estimated proportion of fraudulent reviews and $\lambda$ is a penalty coefficient (default: $\lambda = 2.0$, meaning the penalty is double the fraud proportion). This ensures that the cost of fraud detection exceeds any potential benefit from manipulation.

$p_{\text{fraud}}$ ，$\lambda$ （：$\lambda = 2.0$，）。。

**Illustrative Example** | :

Product A has a User Satisfaction Score (P2.1) of 0.85 based on 1,000 reviews. Fraud detection identifies 150 reviews as potentially fraudulent ($p_{\text{fraud}} = 0.15$). The adjusted score is:

A1000（P2.1）0.85。150（$p_{\text{fraud}} = 0.15$）。：

$$s_{A,P2.1}^{\text{adjusted}} = 0.85 \times (1 - 2.0 \times 0.15) = 0.85 \times 0.70 = 0.595$$

### C.2.5 Scoring and Ranking

**Normalisation** |  (§8.2):

Z-score standardisation was applied:

$$s_{ij} = \frac{x_{ij} - \mu_j}{\sigma_j}$$

followed by rescaling to [0, 1] using the percentile method to ensure comparability.

[0, 1]。

**Aggregation** |  (§8.3.1):

WAM with anti-fraud penalty adjustments:

WAM：

$$C_i = \sum_{j=1}^{n} w_j \cdot s_{ij}^{\text{adjusted}}$$

**Illustrative Scoring Results** |  (hypothetical data for 5 smartphones):

| Rank | Product | P1 (0.35) | P2 (0.30) | P3 (0.20) | P4 (0.15) | Composite | Fraud Penalty Applied 
| ------ | --------- | ----------- | ----------- | ----------- | ----------- | ----------- | ---------------------- 
| 1 | Phone Alpha | 0.92 | 0.88 | 0.75 | 0.82 | 0.863 | No 
| 2 | Phone Beta | 0.88 | 0.82 | 0.85 | 0.78 | 0.838 | No 
| 3 | Phone Gamma | 0.85 | 0.595 | 0.72 | 0.75 | 0.718 | Yes (P2.1 adjusted) 
| 4 | Phone Delta | 0.72 | 0.75 | 0.68 | 0.70 | 0.716 | No 
| 5 | Phone Epsilon | 0.68 | 0.70 | 0.62 | 0.65 | 0.667 | No 

> **Note**: Phone Gamma's lower User Experience score (P2 = 0.595) reflects the anti-brushing penalty applied to its user satisfaction data. Without the penalty, its P2 score would have been 0.85, and it would have ranked 3rd or higher. The anti-fraud adjustment is documented in the methodology statement and the fraud detection audit trail.
> ：Phone Gamma（P2 = 0.595）。，P20.85，3。。

### C.2.6 Sensitivity Analysis

The following sensitivity analyses were conducted in accordance with §8.5.3:

**a) Weight variation test** | :

All Level 1 weights were varied by ±5 percentage points. The maximum rank change was 1 position, indicating that the ranking is robust to moderate weight variations.

**b) Method variation test** | :

The ranking was recomputed using the geometric mean aggregation method. The Spearman's ρ between WAM and geometric mean rankings was 0.94, indicating high consistency.

。WAMSpearman ρ0.94，。

**c) Data perturbation test** | :

Random noise (±5% of the standard deviation of each indicator) was added to the input data. The ranking was recomputed 100 times. The mean rank stability (proportion of elements with unchanged rank) was 88%.

---

## C.3 Example 3: Cross-Domain Comprehensive Ranking

### C.3.1 Scenario Description

A ranking entity wishes to develop a comprehensive ranking that evaluates entities across multiple dimensions from different domains (e.g., a "City Livability Index" that combines economic, environmental, cultural, and infrastructural indicators). The primary challenge is the meaningful aggregation of indicators from different domains with different measurement scales and units.

**Applicable standard provisions** | : ICO Std 2002 core layer (§04–§11), with cross-references to SE-04 (Cities), SE-08 (Sustainability), and SE-05 (Cultural Heritage).

### C.3.2 Process Flow Diagram

```
┌─────────────────────────────────────────────────────────────────┐
│  STEP 1: Purpose & Scope Definition (§04, §01)                  │
│                                                     │
│  - Define: City livability assessment                           │
│  - Target: Residents, policy-makers, investors                 │
│  - Cross-domain: SE-04 + SE-08 + SE-05                         │
└───────────────────────────┬─────────────────────────────────────┘
┌─────────────────────────────────────────────────────────────────┐
│  STEP 2: Multi-Domain Indicator Design (§05)                     │
│                                                     │
│  - Domain-specific indicators (each domain validated)           │
│  - Cross-domain integration rules                               │
│  - Normalisation method selection for cross-domain comparison   │
└───────────────────────────┬─────────────────────────────────────┘
┌─────────────────────────────────────────────────────────────────┐
│  STEP 3: Cross-Domain Weight Assignment (§06)                    │
│                                                     │
│  - Stakeholder consultation for inter-domain weights            │
│  - AHP for intra-domain weights                                │
│  - Sensitivity analysis across domain weight variations         │
└───────────────────────────┬─────────────────────────────────────┘
┌─────────────────────────────────────────────────────────────────┐
│  STEP 4: Data Collection (§07)                                   │
│                                                          │
│  - Tier 1: Official statistics, government databases            │
│  - Tier 2: Resident surveys, expert assessments                │
│  - Tier 3: Social media, public web sources                    │
│  - Cross-domain data harmonisation                              │
└───────────────────────────┬─────────────────────────────────────┘
┌─────────────────────────────────────────────────────────────────┐
│  STEP 5: Scoring, Ranking & Sensitivity Analysis (§08)           │
│  、                                            │
│  - Normalisation: Percentile ranking (cross-domain comparable)  │
│  - Aggregation: WAM with domain interaction effects             │
│  - Sensitivity: Multi-dimensional weight sensitivity analysis   │
│  - Robustness: Bootstrap + method variation + domain exclusion  │
└───────────────────────────┬─────────────────────────────────────┘
┌─────────────────────────────────────────────────────────────────┐
│  STEP 6: Publication & Audit (§09, §10)                          │
│                                                        │
│  - Transparency Level 4 (Full Reproducibility)                 │
│  - Interactive ranking tool (§06.4)                             │
│  - Comprehensive sensitivity analysis report                    │
└─────────────────────────────────────────────────────────────────┘
```

### C.3.3 Indicator System

#### Level 1 Indicators (Domains)

| ID | Domain | Weight | Source Module | Description 
| ---- | -------- | -------- | -------------- | ------------- 
| L1 | Economic Vitality | 0.25 | SE-04 | Economic output, employment, innovation 
| L2 | Environmental Quality | 0.25 | SE-08 | Air quality, green space, GHG emissions 
| L3 | Cultural Richness | 0.20 | SE-05 | Cultural heritage, creative industries, cultural participation 
| L4 | Infrastructure & Services | 0.30 | SE-04 | Transportation, healthcare, education, housing 

#### Level 2 and Level 3 Indicators — Selected Examples

| ID | Sub-dimension / Measure | Parent | Data Source | Normalisation 
| ---- | ------------------------ | -------- | ------------ | --------------- 
| L1.1 | GDP per capita | L1 | Tier 1 (National statistics) | Percentile ranking 
| L1.2 | Employment rate | L1 | Tier 1 (Labour statistics) | Percentile ranking 
| L1.3 | Innovation index | L1 | Tier 2 (Composite index) | Percentile ranking 
| L2.1 | Air quality index (AQI) | L2 | Tier 1 (Environmental monitoring) | Inverse percentile (lower AQI = better) 
| L2.2 | Green space per capita | L2 | Tier 1 (Urban planning data) | Percentile ranking 
| L2.3 | GHG emissions per capita | L2 | Tier 1 (ISO 14064 compliant) | Inverse percentile 
| L3.1 | Cultural heritage density | L3 | Tier 1 (Heritage registry) | Percentile ranking 
| L3.2 | Creative industry employment | L3 | Tier 1 (Labour statistics) | Percentile ranking 
| L3.3 | Cultural participation rate | L3 | Tier 2 (Resident survey) | Percentile ranking 
| L4.1 | Public transport coverage | L4 | Tier 1 (Transport authority) | Percentile ranking 
| L4.2 | Healthcare access index | L4 | Tier 2 (Survey + official data) | Percentile ranking 
| L4.3 | Education quality index | L4 | Tier 2 (Survey + official data) | Percentile ranking 
| L4.4 | Housing affordability | L4 | Tier 1 (Real estate data) | Percentile ranking 

### C.3.4 Cross-Domain Normalisation

**Challenge** | : Indicators from different domains have different measurement scales (e.g., GDP in currency units, AQI in index units, employment rates in percentages). Direct comparison requires a common normalisation method.

（GDP、AQI、）。。

**Method** | : Percentile ranking normalisation (§8.2) was selected for its robustness to outliers and its ability to produce comparable scores across different scales:

$$s_{ij} = \frac{R_{ij} - 1}{N - 1}$$

where $R_{ij}$ is the rank of entity $i$ on indicator $j$ and $N$ is the total number of entities.

$R_{ij}$  $i$  $j$ ，$N$ 。

For indicators where lower values are better (e.g., AQI, GHG emissions), inverse ranking is applied:

（AQI、GHG），：

$$s_{ij} = 1 - \frac{R_{ij} - 1}{N - 1}$$

### C.3.5 Weight Assignment

Weights were determined through a combination of stakeholder consultation and expert panel methods (§06.1):

a) **Inter-domain weights** (Level 1): Determined through stakeholder consultation with 200 residents, 30 policy-makers, and 20 investors. The final weights were calibrated to reflect the consensus priorities of the target audience.

b) **Intra-domain weights** (Level 2 and Level 3): Determined through AHP with a panel of 8 domain experts (2 per domain).
（）：8（2）AHP。

### C.3.6 Sensitivity Analysis

Cross-domain rankings are particularly sensitive to the choice of domain weights. The following multi-dimensional sensitivity analysis was conducted:

**a) One-at-a-time (OAT) weight variation** | :

Each Level 1 weight was independently varied by ±5 and ±10 percentage points, with the remaining weights adjusted proportionally. The maximum rank change for any entity was:

| Weight Variation | Max Rank Change | Entities with ≥2 Position Change 
| ----------------- | ----------------- | ---------------------------------- 
| ±5 pp | 2 positions | 3 of 50 cities 
| ±10 pp | 4 positions | 8 of 50 cities 

**b) Multi-dimensional weight sensitivity** | :

A Monte Carlo simulation was conducted with 10,000 random weight combinations (drawn from a Dirichlet distribution with the mean equal to the published weights). For each entity, the following statistics were computed:

10,000（Dirichlet）。：

| Statistic | Description 
| ----------- | ------------- 
| Mean rank | Average rank across all weight combinations 
| Rank standard deviation | Variability of rank across weight combinations 
| 90% rank interval | 5th to 95th percentile of rank distribution 
| Rank stability index | Proportion of weight combinations where rank is within ±3 of published rank 

**Illustrative Results** |  (for 5 hypothetical cities):

| City | Published Rank | Mean Rank | Rank SD | 90% Interval | Stability Index 
| ------ | --------------- | ----------- | --------- | -------------- | ---------------- 
| City A | 1 | 1.2 | 0.5 | [1, 2] | 98% 
| City B | 2 | 2.8 | 1.1 | [1, 5] | 72% 
| City C | 3 | 3.5 | 1.8 | [1, 7] | 55% 
| City D | 4 | 4.2 | 1.5 | [2, 8] | 48% 
| City E | 5 | 4.8 | 1.2 | [2, 7] | 62% 

> **Note**: City B's relatively low stability index (72%) indicates that its rank is sensitive to the choice of domain weights. This is because City B excels in Economic Vitality (L1) but is weaker in Environmental Quality (L2), and the relative importance of these domains significantly affects its ranking. This sensitivity is disclosed in the limitations section (§9.1.4).
> ：City B（72%）。City B（L1），（L2），。（§9.1.4）。

**c) Domain exclusion test** | :

The ranking was recomputed with each domain excluded in turn. This test identifies which domains have the greatest influence on the ranking:

| Excluded Domain | Mean Rank Change | Max Rank Change 
| ---------------- | ----------------- | ----------------- 
| L1 (Economic) | 2.8 positions | 8 positions 
| L2 (Environmental) | 2.2 positions | 6 positions 
| L3 (Cultural) | 1.5 positions | 5 positions 
| L4 (Infrastructure) | 3.2 positions | 10 positions 

The results indicate that Infrastructure & Services (L4) has the greatest influence on the ranking, which is consistent with its highest weight (0.30). This finding is documented in the methodology statement.

### C.3.7 Interactive Ranking Tool

In accordance with §06.4 (User-Adjustable Weights), an interactive ranking tool was provided that allows users to:

a) adjust the Level 1 domain weights using slider controls;

b) recompute the ranking in real time based on the adjusted weights;

c) compare the user-adjusted ranking with the default ranking entity ranking;

d) view the sensitivity analysis results for each entity.

The tool prominently displays the default (ranking entity) weights alongside any user-adjusted results, with a clear notice that user-adjusted rankings are not the official ranking.

### C.3.8 Publication

The ranking was published at **Transparency Level 4** (Full Reproducibility, §9.2.4), including:

a) complete methodology documentation;

b) all indicator scores at every hierarchical level;

c) complete dataset (downloadable in CSV format);
（CSV）；

d) analysis code (Python scripts for scoring, aggregation, and sensitivity analysis);
（、Python）；

e) comprehensive sensitivity analysis report;

f) interactive ranking tool with user-adjustable weights;

g) limitations disclosure (§9.1.4), including the caveat that the ranking measures relative livability and should not be used as the sole basis for relocation or investment decisions.

---

## C.4 Cross-Example Comparison

| Aspect | Example 1 (ICH) | Example 2 (Consumer Products) | Example 3 (Cross-Domain) 
| -------- | ----------------- | ------------------------------ | -------------------------- 
| Domain | Cultural Heritage | Consumer Products | City Livability 
| Extension Module | SE-05 | SE-01 | SE-04 + SE-05 + SE-08 
| Primary Challenge | Valuing intangible attributes | Anti-fraud / anti-brushing | Cross-domain aggregation 
| Normalisation | Min-max | Z-score + percentile | Percentile ranking 
| Aggregation | WAM | WAM + anti-fraud penalty | WAM 
| Weighting Method | AHP (expert panel) | AHP (expert panel) | Stakeholder consultation + AHP 
| Key Risk | Cultural bias in expert assessment | Data manipulation by ranked entities | Weight sensitivity across domains 
| Transparency Level | Level 3 | Level 2 | Level 4 
| Anti-Fraud | Not applicable | Tier 3 fraud detection + penalty | Not applicable 
| Sensitivity Analysis | Bootstrap + method variation | Weight variation + method variation + data perturbation | OAT + Monte Carlo + domain exclusion 
| Key Robustness Result | Spearman's ρ = 0.96 (WAM vs. geometric) | Max rank change = 1 position (±5pp weight) | Mean stability index = 67% across entities 

---

## C.5 Key Implementation Lessons

### C.5.1 Indicator Design

a) Indicator selection must be driven by the ranking purpose (§05.1), not by data availability. In Example 1, the indicator system includes qualitative measures (e.g., safeguarding plan quality) that require Tier 2 data collection, even though Tier 1 data alone would have been easier to collect.

b) Domain-specific indicators should be validated by domain experts (§05.1). In all three examples, domain experts were involved in the indicator selection process.

### C.5.2 Weight Assignment

a) The choice of weighting method should be documented and justified (§06.1). AHP is suitable when expert judgment is available; stakeholder consultation is appropriate when the ranking target audience has diverse perspectives.
（§06.1）。，AHP；，。

b) Weight sensitivity analysis (§8.5.3) is essential for cross-domain rankings where the relative importance of different domains may vary across stakeholders.

### C.5.3 Data Quality and Anti-Fraud

a) The three-tier data source classification (§7.1) provides a practical framework for managing data quality across different source types.

b) Anti-fraud mechanisms (§7.5) are essential for consumer product rankings where data manipulation is a known risk. The anti-brushing penalty mechanism provides a deterrent that is proportional to the detected fraud.

### C.5.4 Transparency and Reproducibility

a) The four-level transparency system (§9.2) provides a practical framework for progressively improving the transparency of ranking publications. Ranking entities should aim for the highest achievable transparency level, given the sensitivity of the data and the needs of the target audience.

b) User-adjustable weights (§06.4) are particularly valuable for cross-domain rankings where different stakeholders may have different priorities. The interactive ranking tool provides a mechanism for stakeholder engagement that goes beyond the Berlin Principles' recommendation of consumer choice.

---

> **Note**: This annex is informative and part of ICO Std 2002 (Tianji Ranking Methodology Standard). The examples are illustrative only and do not represent actual rankings. All data, scores, and entity names are hypothetical.
> ：，ICO Std 2002（）。，。、。
