# SE-01 : Consumer Products

**ICO Std 2002 — Extension SE-01**

---

This extension module specifies the requirements and methodologies for ranking and evaluating consumer products. Consumer product rankings present distinctive methodological challenges: the diversity of product categories requires differentiated indicator systems; the prevalence of manipulated data (e.g., fake reviews, brush-ordering) demands robust filtering mechanisms; and the integration of objective testing with subjective user experience necessitates carefully designed composite scoring. This module extends the core-layer methodology (Chapters 4 through 10) by defining domain-specific indicators, data collection protocols, anti-fraud mechanisms, and scoring procedures for consumer product evaluation. It is applicable to rankings across all consumer product categories, from food and daily necessities to electronics and durable goods.

---

## SE-01.1 Scope and Applicable Objects

### SE-01.1.1 Scope

This module applies to the design, execution, and publication of rankings that evaluate consumer products. It covers:

a) physical consumer goods, including food and beverages, clothing, electronics, household appliances, cosmetics, and durable goods;

b) digital consumer products, including software applications, digital content, and subscription services;

c) product categories as defined by recognised classification systems (e.g., UNSD Central Product Classification, national product taxonomies).

### SE-01.1.2 Applicable Objects

This module shall apply to rankings of:

a) individual products within a defined category;

b) product lines or series from a single manufacturer;

c) product brands evaluated on aggregate product quality metrics.

### SE-01.1.3 Exclusions

This module does not apply to:

a) industrial or B2B products not marketed to end consumers;

b) financial products and investment instruments;

c) medical devices and pharmaceutical products, which are subject to separate regulatory ranking frameworks.

---

## SE-01.2 Normative References

The following referenced documents are indispensable for the application of this module.

a) ISO 9001:2015 — Quality management systems — Requirements;

b) ISO 10002:2018 — Quality management — Customer satisfaction — Guidelines for complaints handling in organizations;

c) ISO 20400:2017 — Sustainable procurement — Guidance;

d) ICO Std 2002 Core Layer (Chapters 4 through 10);

e) United Nations Guidelines for Consumer Protection (2015 revision).

---

## SE-01.3 Indicator System

### SE-01.3.1 Indicator Hierarchy

The consumer product indicator system shall be organised into the following three-level hierarchy:

a) **Level 1 — Dimensions**: Product Quality, Safety and Compliance, Value for Money, User Satisfaction, Brand Reputation;

b) **Level 2 — Sub-dimensions**: Decompositions of each dimension as specified in SE-01.3.2 through SE-01.3.6;

c) **Level 3 — Specific measures**: Operationalised variables for which data is collected, as specified in each sub-dimension.

### SE-01.3.2 Product Quality

Product quality assesses the objective performance characteristics of a product relative to its intended function and comparable products.

a) **Functional Performance**: The degree to which the product fulfils its stated or implied functional specifications. The ranking entity shall define performance benchmarks based on:

1) manufacturer specifications and claimed performance;

2) category-specific industry standards;

3) comparative testing against peer products.

b) **Durability and Reliability**: The ability of the product to maintain performance over time and under normal conditions of use. Assessment shall include:

1) mean time between failures (MTBF) or equivalent reliability metrics for durable goods;

2) accelerated aging test results where available;

3) warranty claim rates and return rates as supplementary indicators.

c) **Material and Workmanship**: The quality of materials used and the standard of manufacturing workmanship. The ranking entity shall assess:

1) material grade and composition verified through testing or certification;

2) manufacturing precision and consistency;

3) finish quality and attention to detail.

### SE-01.3.3 Safety and Compliance

Safety and compliance assesses the degree to which a product meets safety standards and regulatory requirements.

a) **Regulatory Compliance**: The product's compliance with applicable safety regulations, mandatory standards, and certification requirements in the jurisdiction(s) where it is sold. The ranking entity shall:

1) verify compliance with at least one recognised product safety certification system (e.g., CE marking, CCC certification, UL listing);

2) record any recalls, safety alerts, or regulatory enforcement actions associated with the product;

3) assign a compliance score based on the breadth and depth of certifications held.

b) **Hazard Assessment**: For product categories with inherent safety risks (e.g., children's products, electrical goods, food), the ranking entity shall conduct or reference a hazard assessment that evaluates:

1) the presence and severity of identified hazards;

2) the adequacy of risk mitigation measures (e.g., warning labels, safety features);

3) the product's safety record as evidenced by incident reports or injury data.

c) **Chemical Safety**: For products with potential chemical exposure (e.g., cosmetics, food containers, textiles), the ranking entity shall assess compliance with:

1) applicable chemical substance regulations (e.g., REACH, RoHS, national food contact material standards);

2) the results of independent chemical testing where available.

### SE-01.3.4 Value for Money

Value for money assesses the relationship between a product's price and its performance, quality, and features relative to competing products.

a) **Price-Performance Ratio**: The normalised ratio of aggregate quality score to market price. The ranking entity shall calculate:

$$VPP = \frac{S_{\text{quality}}}{P_{\text{norm}}}$$

where $S_{\text{quality}}$ is the product quality score (0 to 1) and $P_{\text{norm}}$ is the normalised price (product price divided by the median price of the comparable product set).

b) **Feature Completeness**: The proportion of expected or standard features for the product category that the product offers, relative to its price tier.

c) **Total Cost of Ownership**: For durable goods, the ranking entity should estimate the total cost of ownership over the expected product lifespan, including:

1) purchase price;

2) consumables and replacement parts;

3) energy consumption costs;

4) maintenance and repair costs.

d) **Residual Value**: For categories with active secondary markets (e.g., electronics, vehicles), the ranking entity may include residual value as a component of value for money.

### SE-01.3.5 User Satisfaction

User satisfaction assesses the degree to which product users report satisfaction with their purchase and use experience.

a) **Aggregated User Ratings**: The statistical aggregation of user ratings from verified sources. The ranking entity shall:

1) collect user ratings from at least three independent platforms;

2) apply the anti-fraud filtering procedures specified in SE-01.5 before aggregation;

3) report both the mean rating and the number of reviews after filtering.

b) **Sentiment Analysis of Reviews**: The ranking entity shall conduct or reference sentiment analysis of textual user reviews to assess:

1) the distribution of positive, neutral, and negative sentiments;

2) the frequency of specific complaints or praise themes;

3) the correlation between sentiment scores and numerical ratings.

c) **Customer Service Experience**: The quality and responsiveness of post-purchase customer service, including:

1) average response time for customer inquiries;

2) complaint resolution rate;

3) warranty fulfilment rate.

d) **Repeat Purchase and Recommendation**: The degree to which users indicate willingness to repurchase or recommend the product, measured through:

1) verified repeat purchase data where available;

2) Net Promoter Score (NPS) or equivalent recommendation metrics;

3) social sharing and referral rates.

### SE-01.3.6 Brand Reputation

Brand reputation assesses the trustworthiness and credibility of the product's brand based on historical performance, corporate practices, and public perception.

a) **Track Record**: The brand's historical performance in product quality, safety incidents, and regulatory compliance. The ranking entity shall assess:

1) the number and severity of product recalls in the preceding five years;

2) patterns of quality complaints across product lines;

3) consistency of quality ratings over time.

b) **Corporate Responsibility**: The brand's demonstrated commitment to ethical and sustainable practices, including:

1) supply chain transparency and labour practices;

2) environmental commitments and performance;

3) consumer data protection and privacy practices.

c) **Market Reputation**: Independent assessments of the brand's market reputation, including:

1) media coverage sentiment;

2) industry awards and recognition;

3) expert and influencer assessments.

---

## SE-01.4 Data Collection

### SE-01.4.1 Data Source Categories

The ranking entity shall collect data from the following categories of sources:

a) **Laboratory Testing Data**: Results from accredited testing laboratories (e.g., ISO/IEC 17025 accredited) for performance, safety, and chemical testing.

b) **E-Commerce Platform Data**: Product listings, pricing, sales volumes, user ratings, and reviews from major e-commerce platforms. The ranking entity shall specify the platforms used and the data extraction methodology.

c) **Consumer Review Data**: User-generated reviews and ratings from independent review platforms, social media, and consumer forums.

d) **Regulatory and Certification Records**: Product certification databases, recall records, regulatory enforcement actions, and safety alert databases.

e) **Market Research Data**: Market share data, brand perception surveys, and consumer satisfaction studies from established market research providers.

f) **Manufacturer-Provided Data**: Product specifications, test reports, and warranty data provided by the manufacturer. Manufacturer-provided data shall be clearly marked and cross-verified against independent sources.

### SE-01.4.2 Product Category Differentiation

a) The ranking entity shall define product category-specific data collection requirements that reflect the distinctive characteristics of each category. At a minimum, the ranking entity shall differentiate between:

1) **Food and beverages**: microbiological testing, nutritional analysis, ingredient traceability;

2) **Electronics**: performance benchmarking, electromagnetic compatibility, battery safety;

3) **Cosmetics and personal care**: ingredient safety, allergen testing, efficacy claims verification;

4) **Clothing and textiles**: fabric quality, colourfastness, chemical residue testing;

5) **Household appliances**: energy efficiency, noise levels, safety interlocks.

b) For each product category, the ranking entity shall document the specific indicators, data sources, and measurement methods used, and shall justify any deviations from the general indicator system.

### SE-01.4.3 Price Data Collection

a) Price data shall be collected from at least three independent retailers or platforms to reflect market pricing accurately.

b) The ranking entity shall record the date of price data collection and shall use the median price across sources as the reference price.

c) For products with significant price variation over time (e.g., seasonal products, electronics), the ranking entity should collect price data at multiple time points and report the price stability index.

---

## SE-01.5 Anti-Fraud Mechanisms

### SE-01.5.1 General Requirements

The ranking entity shall implement robust anti-fraud mechanisms to protect the integrity of consumer product rankings. Given the prevalence of manipulated data in e-commerce environments, anti-fraud measures are not optional but mandatory for all product rankings that incorporate user-generated data.

### SE-01.5.2 Anti-Brush-Order Filtering

a) The ranking entity shall implement procedures to identify and filter brush-ordering (fabricated transactions designed to inflate sales volume and ratings). The filtering procedures shall include:

1) **Transaction Pattern Analysis**: Detection of abnormal transaction patterns, including:

- clustering of purchases at unusual times or in unusual quantities;

- high concentration of purchases from specific geographic regions or IP address ranges;

- unusually short intervals between purchase and review posting.

2) **Account Analysis**: Identification of suspicious reviewer or buyer accounts, including:

- accounts with disproportionately high review activity;

- accounts that review only products from a single brand or seller;

- newly created accounts with high review volume.

3) **Cross-Platform Verification**: Comparison of sales volume and rating patterns across multiple e-commerce platforms to detect platform-specific anomalies.

b) Sales volume data that is suspected of being inflated by brush-ordering shall be excluded from ranking calculations. The ranking entity shall document the filtering criteria and the proportion of data excluded.

### SE-01.5.3 Anti-Fake-Review Filtering

a) The ranking entity shall implement procedures to identify and filter fake reviews (fabricated or incentivised reviews that do not reflect genuine user experience). The filtering procedures shall include:

1) **Textual Analysis**: Natural language processing techniques to detect:

- reviews with generic or templated language inconsistent with genuine product experience;

- reviews with duplicated or near-duplicated text across different products or platforms;

- reviews that disproportionately use promotional or marketing language.

2) **Incentivised Review Detection**: Identification of reviews that may have been produced in exchange for incentives, including:

- reviews that disclose or imply receipt of free or discounted products;

- reviews posted in coordinated batches following product launch;

- reviews from participants in seller-organised review programmes.

3) **Rating Distribution Analysis**: Statistical analysis of rating distributions to detect anomalies, including:

- distributions that deviate significantly from the expected bell-shaped or J-shaped curve for the product category;

- anomalous spikes in ratings at specific score levels;

- statistically significant differences between verified and unverified purchase reviews.

b) The ranking entity shall calculate and report a Data Integrity Index for each product, defined as:

$$DII = \frac{N_{\text{authentic}}}{N_{\text{total}}}$$

where $N_{\text{authentic}}$ is the number of reviews passing all filtering criteria and $N_{\text{total}}$ is the total number of reviews collected. Products with $DII < 0.50$ shall be flagged in the ranking publication.

### SE-01.5.4 Ongoing Monitoring

a) The ranking entity shall conduct periodic audits of its anti-fraud mechanisms to evaluate their effectiveness. Audits shall be conducted at least once per ranking cycle.

b) The ranking entity shall update its filtering algorithms and criteria in response to new fraud patterns as they are identified.

c) The ranking entity shall document all anti-fraud procedures, parameters, and outcomes, and shall include a summary of anti-fraud results in the methodology report.

---

## SE-01.6 Scoring Methodology

### SE-01.6.1 Scoring Scale

a) Each Level 3 indicator shall be scored on a normalised scale from 0 to 100.

b) Quantitative indicators shall be normalised using the min-max method or z-score method as specified in Chapter 8 of the core layer.

c) Qualitative indicators shall use defined ordinal scales mapped to numerical scores with documented anchor descriptions.

### SE-01.6.2 Weighting

a) The default weight scheme for the five Level 1 dimensions shall be as follows, unless the ranking entity provides documented justification for alternative weights:

| Dimension | Default Weight |
| --- | --- |
| Product Quality | 0.30 |
| Safety and Compliance | 0.25 |
| Value for Money | 0.20 |
| User Satisfaction | 0.15 |
| Brand Reputation | 0.10 |

b) The default weights reflect the principle that product quality and safety are the primary determinants of consumer product ranking, while recognising the importance of value and user experience.

c) For product categories where safety is of paramount concern (e.g., children's products, food, automotive parts), the ranking entity shall increase the weight of Safety and Compliance to at least 0.35, with corresponding reductions in other dimensions.

d) For product categories where value for money is the primary differentiator (e.g., commodity products, entry-level goods), the ranking entity may increase the weight of Value for Money to at most 0.30.

### SE-01.6.3 Category-Specific Scoring Adjustments

a) The ranking entity shall define category-specific scoring adjustments that reflect the distinctive evaluation priorities of each product category. These adjustments shall be documented and justified.

b) For products subject to mandatory safety certification, a product that lacks required certification shall receive a Safety and Compliance score of zero and shall not be included in the ranking.

c) For products where laboratory testing is a primary data source, the ranking entity shall specify the testing standards and methods used, and shall ensure that testing is conducted by accredited laboratories.

### SE-01.6.4 Aggregation

a) Scores at Level 3 shall be aggregated to Level 2, and Level 2 to Level 1, using the weighted sum method specified in Chapter 8 of the core layer.

b) The overall product score shall be calculated as the weighted sum of Level 1 dimension scores using the weights defined in SE-01.6.2.

c) The ranking entity shall report dimension-level scores alongside the overall score to enable users to understand the profile of each ranked product.

d) The ranking entity shall also report the Data Integrity Index (SE-01.5.3.b) for each product alongside the ranking.

---

## SE-01.7 Alignment with International Standards

### SE-01.7.1 ISO 9001 Alignment

a) The Product Quality dimension (SE-01.3.2) shall be consistent with the quality management principles underlying ISO 9001:2015, particularly:

1) the process approach to quality management;

2) the Plan-Do-Check-Act (PDCA) cycle;

3) risk-based thinking in quality assurance.

b) Where a product's manufacturer holds ISO 9001 certification, this may be considered as supporting evidence for the Product Quality dimension but shall not substitute for direct product testing.

### SE-01.7.2 Consumer Protection Alignment

a) The Safety and Compliance dimension (SE-01.3.3) shall be consistent with the principles of the United Nations Guidelines for Consumer Protection, particularly:

1) the right to safety;

2) the right to information;

3) the right to redress.

b) The ranking entity shall ensure that product safety information presented in the ranking does not substitute for mandatory safety labelling or official safety advisories.

---

## SE-01.8 Publication and Transparency

### SE-01.8.1 Publication Requirements

In addition to the requirements specified in Chapter 9 of the core layer, consumer product ranking publications shall include:

a) the product category definitions and inclusion criteria;

b) the Data Integrity Index for each ranked product;

c) a summary of anti-fraud filtering results (number of reviews filtered, proportion excluded);

d) the category-specific scoring adjustments applied, if any;

e) the date and sources of price data.

### SE-01.8.2 Product Identification

a) Each ranked product shall be uniquely identified using:

1) the product name and model number;

2) the manufacturer or brand name;

3) the specific version or revision being evaluated.

b) The ranking entity shall ensure that product identification is sufficiently precise to prevent confusion between similar products or different versions of the same product.

---

> **Note**: This extension module is part of ICO Std 2002 (Tianji Ranking Methodology Standard). Consumer product rankings are among the most widely consumed types of ranking information and have a direct impact on consumer purchasing decisions. Ranking entities bear a heightened responsibility to ensure the accuracy, fairness, and integrity of product rankings, particularly with respect to data fraud prevention and safety-related information. The anti-fraud mechanisms specified in this module represent minimum requirements; ranking entities should implement additional safeguards as appropriate for the specific product category and market environment.
>
