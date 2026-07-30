# Chapter 10: Audit and Traceability

**ICO Std 2002:2026 — Chapter 10**

---

This chapter specifies the requirements for internal and external audit of ranking processes, traceability from final ranking results to original data, data version control, and alignment with ISO/IEC 17021 (Conformity Assessment). It establishes a comprehensive audit and traceability framework that enables independent verification of ranking processes and outcomes, ensuring that every ranking result can be traced back through its computational lineage to the original input data.

---

## 10.1 Audit Framework

The ranking entity shall establish and maintain an audit framework comprising both internal and external audit functions. The audit framework shall ensure the integrity, accuracy, and compliance of the ranking process.

### 10.1.1 Internal Audit Requirements

The ranking entity shall establish an internal audit function that evaluates the compliance of ranking processes with the provisions of this standard and the entity's own methodology documentation.

a) **Independence**: The internal audit function shall be organisationally independent from the ranking production team. Internal auditors shall not have been involved in the design, data collection, scoring, or publication of the ranking being audited.

b) **Competence**: Internal auditors shall possess:

1) knowledge of the ranking methodology and the provisions of this standard;

2) competence in data quality assessment and statistical verification;

3) understanding of the domain to which the ranking applies.

c) **Scope**: Internal audits shall cover:

1) compliance of the indicator system with the requirements of Chapter 5;

2) compliance of the weighting scheme with the requirements of Chapter 6;

3) compliance of data collection and processing with the requirements of Chapter 7;

4) compliance of scoring and ranking with the requirements of Chapter 8;

5) compliance of publication and transparency with the requirements of Chapter 9;

6) the accuracy and completeness of the computational process;

7) the effectiveness of data quality controls (see 7.3);

8) the handling of corrections, retractions, and appeals (see 9.3 and 9.4).

d) **Reporting**: The internal audit function shall produce a written audit report for each audit, which shall include:

1) the scope and objectives of the audit;

2) the audit methodology and evidence reviewed;

3) the findings, including any nonconformities;

4) recommendations for corrective actions;

5) the follow-up actions and timelines for addressing nonconformities.

### 10.1.2 External Audit Requirements

The ranking entity shall engage an independent external auditor to conduct periodic audits of the ranking process. The external auditor shall be independent of the ranking entity and shall not have any financial or advisory relationship with the ranking entity that could compromise objectivity.

a) **Qualifications**: External auditors shall:

1) be accredited or recognised by a national or international accreditation body in accordance with ISO/IEC 17021;

2) have demonstrated competence in auditing ranking, rating, or evaluation systems;

3) have no conflict of interest with the ranking entity, as defined in 4.2.5.

b) **Frequency**: External audits shall be conducted:

1) at least once every three years for ranking systems that publish annually or more frequently;

2) at least once every five years for ranking systems that publish less frequently than annually;

3) within 12 months of any major methodology change (see 5.5.3).

c) **Scope**: External audits shall cover, at a minimum:

1) the full traceability chain from original data to published ranking results (see 10.2);

2) the compliance of the ranking process with the provisions of this standard;

3) the effectiveness of internal quality controls and the internal audit function;

4) the accuracy and completeness of the published methodology statement (see 9.1.2);

5) the handling of stakeholder feedback, appeals, and corrections (see 9.3 and 9.4).

d) **Report**: The external auditor shall produce a written audit report that includes:

1) the audit opinion (unqualified, qualified, or adverse);

2) the scope, methodology, and evidence basis of the audit;

3) detailed findings and any nonconformities;

4) recommendations for improvement;

5) the ranking entity's response and planned corrective actions.

The external audit report shall be made publicly available, subject to the redaction of commercially sensitive information, within 90 calendar days of completion.

### 10.1.3 Audit Frequency

The minimum audit frequencies specified in 10.1.2 b) shall apply. In addition:

a) the ranking entity shall conduct at least one internal audit per ranking cycle;

b) where a ranking cycle spans more than 12 months, at least one internal audit shall be conducted per 12-month period;

c) where a nonconformity is identified in an internal or external audit, a follow-up audit shall be conducted within 6 months to verify the effectiveness of corrective actions.

### 10.1.4 Audit Scope

The audit scope shall encompass all aspects of the ranking process from indicator design through to publication. The audit scope may be scoped by:

a) **Full-scope audit**: An audit covering all provisions of this standard. A full-scope external audit shall be conducted at least once every three ranking cycles.

b) **Focused audit**: An audit covering specific provisions or processes, conducted in response to identified risks, nonconformities, or methodology changes. A focused audit shall not replace a full-scope audit but may supplement it.

### 10.1.5 Audit Record Retention

All audit records shall be retained for a minimum of 5 years from the date of the audit report, or for the period required by applicable law, whichever is longer.

Audit records to be retained shall include:

a) the audit plan, including scope, objectives, and methodology;

b) all audit evidence reviewed, including data samples, computational outputs, and documentation;

c) the audit working papers and notes;

d) the audit report and the ranking entity's response;

e) the record of follow-up actions and their closure.

> **Note**: The 5-year minimum retention period for audit records is aligned with ISO/IEC 17021-1:2015, Clause 9.6, which requires conformity assessment bodies to retain records for a period sufficient to demonstrate ongoing competence. A 5-year period allows for at least one full external audit cycle to reference prior records.
>

---

## 10.2 Traceability Architecture

The ranking entity shall establish and maintain a traceability architecture that enables the complete reconstruction of the ranking process from original data to published results. The traceability architecture shall ensure that, for any published ranking result, the complete chain of transformations can be identified and reproduced.

### 10.2.1 Data Lineage

The ranking entity shall maintain complete data lineage records that trace each data point from its original source through all transformations to its final use in the ranking.

a) **Source-to-score lineage**: For each data point used in the ranking, the following shall be recorded:

1) the original data source identifier and tier (see 7.1);

2) the date and method of data acquisition;

3) all transformations applied to the data point (e.g., currency conversion, unit normalisation, seasonal adjustment);

4) the normalised score derived from the data point (see 8.2);

5) the composite score and ranking position to which the data point contributes.

b) **Transformation logging**: Each transformation applied to data shall be recorded with:

1) the identity of the person or algorithm that performed the transformation;

2) the date and time of the transformation;

3) the input values and output values of the transformation;

4) the parameters and assumptions of the transformation.

c) **Lineage completeness**: The lineage chain from any composite score to its constituent raw data points shall be complete and unbroken. Where a lineage chain is broken (e.g., due to data obtained from a third party that does not provide full provenance), the gap shall be documented as a traceability limitation.

### 10.2.2 Decision Trail

The ranking entity shall maintain a decision trail that records all methodological and procedural decisions made during the ranking process.

a) **Decision records**: For each methodological decision, the following shall be documented:

1) the decision made (e.g., choice of normalisation method, inclusion or exclusion of an outlier);

2) the rationale for the decision;

3) the alternatives considered and the reasons for their rejection;

4) the person or body responsible for the decision;

5) the date of the decision.

b) **Decision categories**: The decision trail shall cover, at a minimum:

1) indicator selection and exclusion decisions (see 5.1);

2) weighting decisions (see Chapter 6);

3) data source selection decisions (see 7.1);

4) missing data handling decisions (see 7.4.1);

5) outlier handling decisions (see 7.4.2);

6) normalisation method selection (see 8.2);

7) aggregation method selection (see 8.3);

8) entity inclusion and exclusion decisions (see 8.6.3 e)).

### 10.2.3 Computation Log

The ranking entity shall maintain computation logs that record the execution of all computational steps in the ranking process.

a) **Log content**: Computation logs shall include:

1) the identification of the computation (e.g., normalisation of indicator X for entity Y);

2) the input data and parameters;

3) the computational method or algorithm applied, including the software and version;

4) the output values;

5) the date and time of execution;

6) any warnings or errors encountered during execution.

b) **Automated logging**: Where the ranking process is executed using software, computation logs shall be generated automatically. Manual logging is permitted only for computations that cannot be automated.

c) **Log integrity**: Computation logs shall be protected against unauthorised modification. The ranking entity should implement integrity controls such as:

1) write-once storage;

2) cryptographic hashing of log entries;

3) access controls restricting log modification to authorised personnel.

### 10.2.4 Change History

The ranking entity shall maintain a comprehensive change history that records all modifications to the ranking methodology, data, and processes.

a) **Version control**: All ranking artefacts shall be subject to version control, including:

1) the indicator system definition (see 5.5.4);

2) the weighting scheme;

3) the data collection and processing procedures;

4) the computational code and parameters;

5) the published ranking results (see 9.3.3).

b) **Timestamps**: Each version of a ranking artefact shall be timestamped using a reliable time source. Timestamps shall include:

1) the date and time of the change, in ISO 8601 format (YYYY-MM-DDThh:mm:ss±hh:mm);

2) the identity of the person or system that made the change;

3) the version identifier of the artefact before and after the change.

c) **Change log**: A change log shall be maintained that records:

1) a description of each change;

2) the reason for the change;

3) the impact of the change on ranking results, where applicable;

4) the approval authority for the change.

d) **Data versioning**: When input data is modified (e.g., corrections, updates, or supplements), the following shall be recorded:

1) the data points affected, identified by entity and indicator;

2) the original and corrected values;

3) the reason for the modification;

4) the date and author of the modification;

5) the version of the dataset before and after the modification.

> **Note**: The traceability architecture specified in this section is designed to enable the "full reproducibility" transparency level defined in 9.2.4. Even where a ranking is published at a lower transparency level, the traceability records shall be maintained internally and made available to auditors upon request.
>

---

## 10.3 ISO 17021 Alignment

The audit and traceability provisions of this chapter are aligned with the requirements of ISO/IEC 17021-1:2015 (Conformity Assessment — Requirements for Bodies Providing Audit and Certification of Management Systems). This section specifies the alignment and any ICO-specific adaptations.

### 10.3.1 Conformity Assessment Bodies

External auditors of ranking systems shall meet the requirements for conformity assessment bodies (CABs) as specified in ISO/IEC 17021-1:2015, with the following adaptations:

a) **Legal status**: The CAB shall be a legally identifiable entity that is independent of the ranking entity it audits, as required by ISO/IEC 17021-1:2015, Clause 5.1.

b) **Impartiality**: The CAB shall establish and maintain an impartiality mechanism in accordance with ISO/IEC 17021-1:2015, Clause 5.2. The CAB shall not provide consulting services to ranking entities that it audits.

c) **Competence**: The CAB shall ensure that audit team members possess:

1) generic competence as specified in ISO/IEC 17021-1:2015, Clause 7;

2) domain-specific competence in the ranking methodology and statistical methods used;

3) competence in data quality assessment and computational verification.

d) **Accreditation**: The CAB should be accredited by a national or international accreditation body that is a signatory to the ILAC Mutual Recognition Arrangement or a regional equivalent.

### 10.3.2 Auditor Competence Requirements

Auditors conducting audits of ranking systems under this standard shall meet the following competence requirements in addition to the generic requirements of ISO/IEC 17021-1:2015, Clause 7:

a) **Methodology knowledge**: Auditors shall demonstrate understanding of:

1) the principles and provisions of ICO Std 2002;

2) the statistical methods used in ranking systems (e.g., normalisation, aggregation, sensitivity analysis);

3) the data quality requirements specified in Chapter 7.

b) **Practical experience**: Lead auditors shall have participated in at least two complete audits of ranking, rating, or evaluation systems within the preceding five years.

c) **Continuing education**: Auditors shall maintain their competence through continuing education, including:

1) awareness of updates to this standard and relevant ISO standards;

2) training in new methodologies and technologies relevant to ranking systems.

### 10.3.3 Audit Evidence

Auditors shall base their findings on sufficient and appropriate audit evidence, in accordance with ISO/IEC 17021-1:2015, Clause 9.4. Audit evidence for ranking systems shall include:

a) **Documentary evidence**: Methodology documentation, data collection plans, quality control records, and publications.

b) **Computational evidence**: Computation logs (see 10.2.3), software output, and independent re-computation results.

c) **Data evidence**: Samples of input data, intermediate results, and final outputs, verified against source data.

d) **Traceability evidence**: Demonstration of the complete lineage from selected composite scores to their constituent raw data points (see 10.2.1).

e) **Test evidence**: Results of re-performing selected computational steps to verify the accuracy of the original computation.

The audit sample shall be sufficient to provide reasonable assurance of the accuracy of the overall ranking. As a minimum, the audit sample shall include:

1) a random sample of at least 5% of ranked entities, subject to a minimum of 10 entities;

2) all entities for which corrections or appeals have been processed;

3) all entities that are outliers in the ranking distribution.

### 10.3.4 Nonconformity Handling

When an audit identifies a nonconformity with the provisions of this standard, the following procedure shall apply:

a) **Classification**: Nonconformities shall be classified as:

1) **Major nonconformity**: A nonconformity that results in a fundamental failure to achieve the objective of the relevant requirement, or a systematic failure across multiple provisions.

2) **Minor nonconformity**: A nonconformity that does not result in a fundamental failure but indicates a lapse in compliance with a specific requirement.

b) **Corrective action**: For each nonconformity, the ranking entity shall:

1) identify the root cause of the nonconformity;

2) develop a corrective action plan with defined timelines;

3) implement the corrective action within the agreed timeframe;

4) verify the effectiveness of the corrective action.

c) **Timelines**:

1) Major nonconformities shall be addressed within 90 calendar days of the audit report.

2) Minor nonconformities shall be addressed within 180 calendar days of the audit report.

d) **Follow-up**: The auditor shall verify the effectiveness of corrective actions through follow-up audit or documented evidence review, as appropriate.

---

## 10.4 DPP-CQ Integration

This section specifies the integration between the traceability provisions of this chapter and ICO Std 2001 (Digital Product Passport — Credibility & Quality, DPP-CQ). The DPP-CQ framework provides a standardised mechanism for attaching cryptographic proof and provenance information to ranking results.

### 10.4.1 Digital Product Passport for Rankings

A ranking published in accordance with this standard may be accompanied by a Digital Product Passport (DPP) conforming to ICO Std 2001. Where a DPP is provided, it shall include:

a) **Ranking identity**: The unique identifier of the ranking, including the ranking title, version, publication date, and methodology version.

b) **Data provenance summary**: A machine-readable summary of the data sources used, including the tier, coverage rate, and acquisition date for each source.

c) **Methodology fingerprint**: A machine-readable description of the methodology applied, including:

1) the normalisation method and parameters;

2) the scoring method and parameters;

3) the aggregation method and weighting scheme.

d) **Computational integrity claim**: A claim regarding the integrity of the computational process, supported by the computation logs specified in 10.2.3.

### 10.4.2 Cryptographic Verification

Where a DPP is provided, the ranking entity should implement cryptographic verification mechanisms to enhance the trustworthiness of the ranking results. Cryptographic verification may include:

a) **Hash verification**: A cryptographic hash of the complete dataset and computational outputs, enabling verification that the data has not been modified since publication.

b) **Digital signatures**: A digital signature applied by the ranking entity to the published results and methodology documentation, authenticating the origin and integrity of the publication.

c) **Timestamp authority**: A trusted timestamp from a recognised timestamp authority, providing non-repudiable evidence of the time of publication.

> **Note**: Cryptographic verification is optional under this version of the standard. However, as ranking systems are increasingly used in automated decision-making contexts, the ability to verify the integrity and provenance of ranking results through cryptographic means is expected to become a normative requirement in future revisions.
>

### 10.4.3 Blockchain Anchoring (Optional)

The ranking entity may anchor the DPP to a distributed ledger (blockchain) to provide an immutable record of the ranking publication. Where blockchain anchoring is implemented:

a) the anchor shall contain only a cryptographic hash of the ranking data and metadata, not the ranking data itself;

b) the anchoring mechanism shall not compromise the privacy of ranked entities or the confidentiality of proprietary methodology details;

c) the choice of blockchain platform shall be documented, including the rationale for the choice and the governance model of the platform;

d) the ranking entity shall ensure that the blockchain anchoring does not create a dependency that could prevent the correction or retraction of ranking results as required by 9.3.

> **Note**: Blockchain anchoring is a specialised form of cryptographic verification that provides tamper-evidence and non-repudiation. It is not required by this standard and should only be implemented where the additional assurance justifies the complexity and cost.
>

---

> **Note**: The audit and traceability provisions of this chapter are essential for the credibility and accountability of ranking systems. They enable independent verification, support the correction of errors, and provide the evidentiary basis for compliance declarations (see Chapter 11). The alignment with ISO/IEC 17021 ensures that the audit framework is consistent with international best practices for conformity assessment, while the DPP-CQ integration (10.4) provides a forward-looking mechanism for cryptographic verification of ranking integrity.
>