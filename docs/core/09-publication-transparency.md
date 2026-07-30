# Chapter 9: Result Publication and Transparency

**ICO Std 2002:2026 — Chapter 9**

---

This chapter specifies the requirements for the publication of ranking results, methodological transparency, stakeholder communication, and historical data preservation. It establishes a comprehensive transparency framework that enables reproducibility, accountability, and public scrutiny of ranking outcomes. The provisions in this chapter are aligned with the IREG Berlin Principles on Ranking of Higher Education Institutions, specifically Principle R5 (Data Collection) and Principle R6 (Outcome Presentation), which mandate that ranking outcomes shall be presented in a transparent and accessible manner.

---

## 9.1 Publication Requirements

All ranking results shall be published in accordance with the requirements specified in 9.1.1 through 9.1.4. The ranking entity shall ensure that publication occurs within the declared timeline and that all mandatory disclosures are included in the publication.

### 9.1.1 Minimum Disclosure Set

Each ranking publication shall include, at a minimum, the following information:

a) **Ranking title and version**: The official title of the ranking and the version identifier of the methodology applied (see 5.5.4).

b) **Publication date**: The date on which the ranking results are officially released, expressed in ISO 8601 format (YYYY-MM-DD).

c) **Reference period**: The time period to which the data and ranking results apply.

d) **Ranked entities**: The complete list of entities included in the ranking, together with their composite scores and ranking positions.

e) **Excluded entities**: The list of entities considered for inclusion but excluded from the final ranking, together with the reasons for exclusion.

f) **Indicator scores**: The scores of each ranked entity on all Level 1 indicators, as specified in 8.6.1.

g) **Methodology summary**: A methodology summary conforming to the requirements of 8.6.3.

h) **Data source summary**: A summary of data sources used, organised by tier (see 7.1), including the proportion of data points sourced from each tier.

i) **Contact information**: The name and contact details of the ranking entity responsible for the publication.

### 9.1.2 Methodology Statement

The ranking entity shall publish a methodology statement that provides sufficient detail for an informed reader to understand and critically evaluate the ranking process. The methodology statement shall include:

a) the ranking purpose and target audience (see 4.1.1);

b) the indicator system and its hierarchical structure (see 5.2);

c) the indicator selection criteria and their application (see 5.1);

d) the weighting scheme and the method by which weights were determined (see Chapter 6);

e) the data collection methodology, including source tiers and verification procedures (see Chapter 7);

f) the normalisation method(s) applied (see 8.2);

g) the scoring and aggregation method(s) applied (see 8.1 and 8.3);

h) the robustness and sensitivity analysis results (see 6.3 and 8.5.3);

i) any deviations from the provisions of this standard, with justification.

### 9.1.3 Data Summary

The ranking entity shall publish a data summary that includes:

a) the total number of data points collected, by indicator tier;

b) the coverage rate for each indicator, expressed as:

$$\text{Coverage}_j = \frac{n_{\text{available},j}}{n_{\text{total},j}} \times 100\%$$

where $n_{\text{available},j}$ is the number of entities for which data is available for indicator $j$, and $n_{\text{total},j}$ is the total number of entities in the ranking population for indicator $j$.

c) the missing data handling method applied (see 7.4.1);

d) a summary of data quality metrics (see 7.3);

e) any known data limitations or caveats.

### 9.1.4 Limitations Disclosure

The ranking entity shall disclose the following limitations in the publication:

a) the conceptual limitations of the indicator system, including any aspects of the ranking purpose that are not fully captured by the indicators;

b) the methodological limitations, including the sensitivity of results to methodological choices (e.g., normalisation method, aggregation method, weighting scheme);

c) the data limitations, including coverage gaps, measurement errors, and the use of Tier 3 data sources (see 7.1.3);

d) the temporal limitations, including the relevance of the data to the current state of the ranked entities;

e) the scope of interpretation, specifying what the ranking does and does not measure, and warning against over-interpretation of small rank differences.

> **Note**: The limitations disclosure is aligned with IREG Berlin Principle R15 (Limitations Disclosure). The purpose is not to undermine the credibility of the ranking, but to enable informed and appropriate use of the results by all stakeholders.
>

---

## 9.2 Transparency Levels

The transparency of a ranking publication shall be classified into one of four levels, as defined in 9.2.1 through 9.2.4. The ranking entity shall declare the transparency level of each publication.

### 9.2.1 Level 1: Summary Transparency

Level 1 transparency provides the minimum disclosure set specified in 9.1.1 and the methodology summary specified in 9.1.2, but does not disclose detailed indicator-level data or the full methodology documentation.

Level 1 transparency shall be considered the absolute minimum for any ranking publication. Rankings published at Level 1 transparency shall not be used for purposes that require independent verification of the results.

### 9.2.2 Level 2: Methodology Transparency

Level 2 transparency provides, in addition to Level 1 requirements:

a) the full methodology documentation, including all provisions specified in 9.1.2;

b) the weighting scheme with all weights at each hierarchical level;

c) the robustness and sensitivity analysis results;

d) the data summary specified in 9.1.3.

Level 2 transparency enables an informed reader to understand and critically evaluate the ranking methodology. Rankings published at Level 2 transparency may be used for purposes that require methodological scrutiny, but do not allow independent reproduction of the results.

### 9.2.3 Level 3: Data Transparency

Level 3 transparency provides, in addition to Level 2 requirements:

a) the normalised scores of each ranked entity on all Level 2 and Level 3 indicators;

b) the raw data for each ranked entity on all indicators, or a reference to a publicly accessible data repository containing such data;

c) the code or algorithms used for normalisation, scoring, and aggregation, or a reference to a publicly accessible repository containing such code.

Level 3 transparency enables independent verification of the ranking results by allowing external parties to recompute the ranking from the underlying data. Rankings published at Level 3 transparency shall be used for purposes that require independent verification.

### 9.2.4 Level 4: Full Reproducibility

Level 4 transparency provides, in addition to Level 3 requirements:

a) the complete computational environment specification, including software versions, parameter settings, and any random seeds used;

b) the audit trail from raw data to final ranking results (see 10.2);

c) the data provenance records for all data sources (see 7.2.4);

d) the complete change history of the methodology and data since the previous ranking cycle.

Level 4 transparency enables full independent reproduction of the ranking results. The ranking entity should aspire to Level 4 transparency as the target standard for all publications.

> **Note**: The transparency levels are cumulative: each higher level includes all the requirements of the lower levels. The ranking entity shall declare the achieved transparency level in each publication. The relationship between transparency levels and the IREG Berlin Principles is as follows: Level 2 satisfies Principle R3 (Methodology Transparency); Level 3 satisfies Principle R10 (Reproducibility); Level 4 exceeds the Berlin Principles requirements.
>

---

## 9.3 Correction and Retraction

The ranking entity shall establish and maintain procedures for correcting errors in published ranking results and, where necessary, retracting ranking publications.

### 9.3.1 Error Correction Protocol

When an error in a published ranking is identified, the ranking entity shall follow the error correction protocol specified below.

a) **Error classification**: Errors shall be classified according to their severity:

1) **Critical error**: An error that changes the composite score of any ranked entity by more than $\Delta_{\text{critical}}$ or changes the rank of any entity by more than $R_{\text{critical}}$ positions, where $\Delta_{\text{critical}}$ and $R_{\text{critical}}$ are thresholds defined in the methodology documentation.

2) **Material error**: An error that changes the composite score or rank of any entity, but does not meet the threshold for a critical error.

3) **Minor error**: An error that does not affect the composite scores or ranking positions, such as a typographical error in the methodology statement.

b) **Correction timeline**:

1) Critical errors shall be corrected within 7 calendar days of confirmation.

2) Material errors shall be corrected within 30 calendar days of confirmation.

3) Minor errors shall be corrected in the next scheduled publication or within 90 calendar days, whichever is sooner.

c) **Correction notice**: Each correction shall be accompanied by a public notice that includes:

1) a description of the error and its cause;

2) the impact of the error on the ranking results;

3) the corrected values and the resulting changes in ranking positions;

4) a reference to the original publication version (see 9.3.3).

d) **Notification of affected entities**: The ranking entity shall notify all entities whose ranking position or composite score is affected by the correction, prior to the public correction notice where feasible.

> **Note**: This protocol is aligned with IREG Berlin Principle R13 (Error Correction). The requirement for prior notification of affected entities reflects the principle that ranked entities should not learn about changes to their ranking from the general public.
>

### 9.3.2 Ranking Retraction Criteria

A ranking publication shall be retracted when:

a) a critical error affects the ranking results of a substantial proportion (more than 10%) of ranked entities;

b) the data upon which the ranking is based is found to be fundamentally flawed or fraudulent;

c) the methodology is found to contain a fundamental error that invalidates the ranking results;

d) the ranking was published in violation of ethical requirements specified in Chapter 4.

A retraction shall:

1) remove the ranking from active circulation and mark it as retracted in all repositories where it is hosted;

2) publish a retraction notice that includes the reason for retraction, the scope of impact, and any remedial actions planned;

3) remain accessible for the historical record, with a prominent retraction label, to preserve the audit trail (see 10.2).

### 9.3.3 Version Control of Published Results

All published ranking results shall be subject to version control. The version control system shall:

a) assign a unique version identifier to each publication, following a defined schema (e.g., v1.0, v1.1, v2.0), where:

1) major version increments indicate a change in methodology that affects the comparability of results across versions;

2) minor version increments indicate corrections or updates that do not affect methodological comparability.

b) maintain an accessible archive of all published versions, including retracted versions;

c) publish a change log that records all changes between versions, including:

1) the date and nature of each change;

2) the sections or data affected;

3) the reason for the change.

d) ensure that any entity accessing a superseded version is notified that a newer version exists.

---

## 9.4 Stakeholder Communication

The ranking entity shall establish and maintain effective communication channels with all stakeholders, including ranked entities, users of the ranking, and the general public.

### 9.4.1 Pre-publication Review

Prior to the publication of ranking results, the ranking entity shall conduct a pre-publication review process that includes:

a) **Technical review**: An internal review of the computational accuracy of the ranking results, verifying that:

1) all data has been correctly entered and processed;

2) the normalisation, scoring, and aggregation computations are free of errors;

3) the ranking positions are correctly derived from the composite scores.

b) **Methodology review**: A review by at least two qualified reviewers who were not directly involved in the data collection and scoring process, confirming that:

1) the methodology has been applied as documented;

2) any deviations from the documented methodology are identified and justified;

3) the limitations disclosure (see 9.1.4) is adequate and accurate.

c) **Factual review by ranked entities**: The ranking entity should provide ranked entities with the opportunity to review the factual accuracy of their own data before publication, subject to the following conditions:

1) the review period shall be no less than 10 and no more than 30 calendar days;

2) the review shall be limited to factual accuracy of the entity's own data and shall not extend to methodological choices;

3) the ranking entity shall document all factual corrections made as a result of the review.

> **Note**: Pre-publication factual review by ranked entities is aligned with IREG Berlin Principle R5, which emphasises that ranked entities should have the opportunity to verify the accuracy of data attributed to them. This does not imply that ranked entities have veto power over the ranking results.
>

### 9.4.2 Feedback Mechanism

The ranking entity shall maintain a public feedback mechanism that allows any stakeholder to submit comments, questions, or concerns regarding the ranking. The feedback mechanism shall:

a) be accessible through at least one publicly available channel (e.g., dedicated email address, web portal);

b) provide an acknowledgment of receipt within 5 business days;

c) provide a substantive response within 30 calendar days for feedback related to data accuracy, and within 60 calendar days for feedback related to methodology;

d) maintain a public log of feedback received and responses provided, with personally identifiable information redacted.

### 9.4.3 Appeal Process

The ranking entity shall establish a formal appeal process for ranked entities that wish to challenge the ranking results or the methodology applied to them. The appeal process shall:

a) be documented and publicly accessible;

b) specify the grounds on which an appeal may be filed, which shall include:

1) factual errors in the data attributed to the appealing entity;

2) procedural errors in the application of the methodology to the appealing entity;

3) evidence of bias or conflict of interest affecting the ranking of the appealing entity.

c) specify the procedures for filing an appeal, including:

1) the time limit for filing an appeal, which shall be no less than 30 calendar days from the publication date;

2) the information and evidence to be submitted with the appeal;

3) the identity of the appeal review body.

d) ensure that the appeal is reviewed by a body or panel that is independent of the individuals who produced the original ranking;

e) issue a written decision within 60 calendar days of receiving the appeal, including:

1) the findings of the appeal review body;

2) the decision and its rationale;

3) any corrective actions to be taken.

f) not require the appealing entity to pay fees for the appeal process that are disproportionate to the nature of the appeal.

> **Note**: The appeal process is aligned with IREG Berlin Principle R6, which requires that ranking entities provide a mechanism for ranked entities to challenge the results. The independence of the appeal review body is essential to the credibility of the process.
>

---

## 9.5 Historical Data Preservation and Retrospection

The ranking entity shall preserve historical ranking data and methodology records to enable retrospection, longitudinal analysis, and audit.

### 9.5.1 Preservation Requirements

The ranking entity shall preserve the following records for each ranking cycle:

a) the complete dataset used to produce the ranking, including raw data, normalised data, and derived scores;

b) the methodology documentation applicable to the ranking cycle, including the version of the indicator system, weighting scheme, and computational procedures;

c) the published ranking results and all associated publications;

d) the correction and retraction records, if any;

e) the stakeholder feedback and appeal records, if any;

f) the audit records (see 10.3).

### 9.5.2 Retention Period

Historical records shall be retained for a minimum period of 10 years from the date of publication, or for the period required by applicable law, whichever is longer.

After the minimum retention period, records may be disposed of provided that:

a) a summary record is retained indefinitely, containing the ranking title, publication date, methodology version, and the list of ranked entities with their composite scores;

b) the disposal is documented, including the date of disposal and the identity of the authorising person.

### 9.5.3 Retrospective Analysis

The ranking entity should conduct retrospective analysis of historical rankings to assess:

a) the stability of ranking results over time;

b) the predictive validity of the indicator system (i.e., whether indicators selected in earlier cycles remain relevant);

c) the impact of methodology changes on the comparability of results across ranking cycles.

Retrospective analysis results shall be made available to auditors upon request (see Chapter 10) and should be published as supplementary materials.

### 9.5.4 Cross-Cycle Comparability

Where the ranking entity publishes rankings on a recurring basis, it shall:

a) clearly identify any methodology changes between ranking cycles and their impact on comparability;

b) provide a comparability statement that indicates whether and how results from different cycles can be meaningfully compared;

c) where methodology changes are substantial, provide a bridging analysis that re-computes the prior ranking under the new methodology for comparability purposes.

---

> **Note**: The provisions of this chapter are designed to ensure that ranking publications serve the public interest by enabling transparency, accountability, and informed use. Transparency is not merely a disclosure requirement; it is the foundation upon which the credibility and utility of ranking systems rest. The IREG Berlin Principles R5 and R6, which this chapter primarily aligns with, establish the international baseline for transparency in ranking practices. ICO Std 2002 extends these principles through the four-level transparency framework (9.2), the structured error correction protocol (9.3.1), and the historical data preservation requirements (9.5).
>