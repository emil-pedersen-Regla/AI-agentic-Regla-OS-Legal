# QMS Data Access and GDPR Compliance: Research Report

**Project**: OptoCeutics Co-Development Cooperation Agreement
**Author**: Legal Module (AI Research Agent)
**Date**: 2026-02-19
**Version**: v01
**Classification**: Internal - Regla ApS

---

## Executive Summary

This report analyzes the GDPR and data protection landscape for the Regla-OptoCeutics co-development partnership, where Regla will access OptoCeutics' QMS data to develop, train, and validate an AI-powered compliance automation platform. The core finding is that **the vast majority of QMS data is non-personal organizational data to which GDPR simply does not apply**, and for the narrow slice of data that may contain personal data references, well-established mechanisms exist to enable full data access while maintaining compliance. The agreement should be structured to maximize data utility, not minimize data access.

---

## 1. GDPR Applicability to QMS Data: The Line Is Clear and Favorable

### The Fundamental Question

GDPR applies only to "personal data" - information relating to an identified or identifiable natural person (Article 4(1)). QMS data is overwhelmingly organizational, procedural, and technical in nature.

### Data Classification by GDPR Applicability

**Category A: Not Personal Data (GDPR Does Not Apply) - ~90-95% of QMS**

| Data Type | Why Not Personal Data |
|-----------|----------------------|
| SOPs and work instructions | Organizational procedures - no individual identification |
| Quality manuals | Corporate policies and standards |
| Process maps and flowcharts | Abstract process descriptions |
| Document templates and hierarchies | Structural frameworks |
| Risk management files (FMEA, risk-benefit) | Technical product analysis |
| Technical documentation structure | Regulatory submission frameworks |
| Design history files | Product development records |
| Supplier qualification records | Corporate entity data |
| Equipment calibration records | Machine/asset data |
| Environmental monitoring data | Facility data |
| Regulatory submission templates | Standardized document formats |

For all Category A data, there is **no GDPR restriction whatsoever**. Regla can access, copy, analyze, use for AI training, and derive commercial products from this data without any data protection obligation. The agreement needs only standard confidentiality protections (NDA), not GDPR-specific provisions.

**Category B: May Contain Personal Data References - ~5-8% of QMS**

| Data Type | Personal Data Element | Mitigation |
|-----------|----------------------|------------|
| Training records | Employee names, training dates | Simple pseudonymization |
| CAPA records | Names of responsible persons | Replace with role titles |
| Internal audit findings | Auditor/auditee names | Replace with role identifiers |
| Management review minutes | Attendee names, assignments | Pseudonymize participants |
| Complaint handling records | Reporter names, sometimes patient info | Tiered redaction |
| Deviation/nonconformance reports | Who identified, who approved | Replace with role codes |

**Category C: Higher Sensitivity - ~1-3% of QMS**

| Data Type | Personal Data Element | Mitigation |
|-----------|----------------------|------------|
| Clinical evaluation data | May reference patient cohorts | Usually already anonymized in CERs |
| Vigilance/incident reports | Patient identifiers, HCP names | Redaction before sharing |
| Post-market clinical follow-up | Patient-level clinical data | Anonymization/aggregation |

### The Practical Reality

OptoCeutics' QMS is primarily a **documentation management system for regulatory compliance**, not a patient data repository. Clinical data referenced in QMS documents (such as CERs) is typically already anonymized or aggregated by the time it enters the QMS, because EU MDR and Good Clinical Practice require patient data protection at the source.

**Key Insight**: The fear of GDPR blocking QMS data sharing is largely unfounded. The overwhelming majority of the data Regla needs - document structures, process workflows, template architectures, regulatory compliance patterns, risk management frameworks - contains zero personal data.

### Recommendation

Structure the agreement with a **tiered data classification** approach:
- **Tier 1 (Unrestricted)**: All organizational, procedural, and technical QMS data. Share freely under NDA.
- **Tier 2 (Light Processing)**: Data with incidental personal data references. Apply simple pseudonymization before transfer.
- **Tier 3 (Controlled)**: Data with clinical/patient references. Apply anonymization or exclude from standard data access; use synthetic data generation for AI training on these patterns.

---

## 2. Controller, Processor, or Joint Controller: It Depends on Data Type

### Analysis Framework

The EDPB Opinion 28/2024 and CNIL's 2025 guidance on AI system development provide the definitive framework for determining roles in co-development scenarios.

### Role Determination by Activity

**For Tier 1 Data (Non-Personal Data): No GDPR Role Needed**

GDPR does not apply. Neither party is a controller or processor because there is no personal data processing. This is the majority of the data exchange.

**For Tier 2 Data (Incidental Personal Data): Regla as Independent Controller**

When Regla accesses QMS data that incidentally contains employee names or organizational personal data:
- **OptoCeutics** is the original controller of employee data
- **Regla** becomes an independent controller when it processes this data for its own purpose (platform development)
- This is NOT a processor relationship because Regla determines its own purposes and means of processing
- This is NOT joint controllership because the parties have distinct, independent purposes

The CNIL guidance on AI system providers explicitly addresses this: when a company provides data to an AI developer, and the AI developer uses that data for its own independent purpose (building a product), the AI developer is an independent controller, not a processor.

**For Tier 3 Data (Clinical/Patient Data): Avoid Entirely Through Design**

The cleanest approach is to ensure Regla never receives identifiable patient data. OptoCeutics anonymizes before sharing, or the parties use synthetic data generation. If truly anonymized, GDPR does not apply (Recital 26).

### Why Joint Controllership Should Be Avoided

Joint controllership under Article 26 GDPR would require:
- A joint controller agreement specifying respective responsibilities
- A contact point for data subjects
- Shared liability for GDPR compliance
- Complexity in exercising data subject rights

This is unnecessary overhead for a partnership where the personal data component is minimal. The agreement should be structured to make clear that each party independently determines its own processing purposes.

### Recommendation

- Draft the agreement so that OptoCeutics shares **non-personal QMS data** under NDA (no GDPR role)
- For any data containing personal data elements, OptoCeutics pseudonymizes before transfer
- Regla is an **independent controller** for any residual personal data it processes
- Include a brief **data access protocol** specifying that OptoCeutics is responsible for pseudonymization/anonymization before data leaves its systems
- Avoid joint controllership entirely through clean data separation

---

## 3. Lawful Basis: Mostly Irrelevant, But Covered

### For Non-Personal Data (Tier 1)

No lawful basis required. GDPR does not apply. This is a commercial data sharing arrangement governed by contract and confidentiality obligations.

### For Incidental Personal Data (Tier 2)

**Legitimate interest (Article 6(1)(f))** is the appropriate lawful basis for both parties:

**OptoCeutics' legitimate interest in sharing**: Co-developing a platform that will improve its QMS processes, reduce compliance burden, and provide free perpetual access to a valuable tool. The data shared is limited to incidental personal data (employee names in process documents), the impact on data subjects is minimal, and subjects would reasonably expect their employer to engage technology partners.

**Regla's legitimate interest in processing**: Developing an AI platform for medical device QMS automation. This is a clearly lawful commercial activity. The personal data processed is minimal and incidental (names in document metadata), and the processing is necessary for the legitimate commercial purpose.

The CNIL's June 2025 recommendations explicitly affirm that **commercial interests in AI development constitute legitimate interests** under GDPR, provided the processing is necessary and proportionate. Given that the personal data here is incidental rather than targeted, the balancing test is straightforward in favor of processing.

**Contract performance (Article 6(1)(b))** also applies for OptoCeutics' employees whose data appears in QMS documents - processing their names in quality records is necessary for OptoCeutics' performance of its employment contracts and quality management obligations.

### For Clinical/Patient Data (Tier 3)

If properly anonymized before sharing: no lawful basis needed (Recital 26 - anonymized data is not personal data).

If pseudonymized only: Article 9(2)(j) GDPR - processing necessary for scientific research purposes with appropriate safeguards - or Article 9(2)(i) - processing necessary for reasons of public interest in the area of public health. However, the better approach is to ensure anonymization so this question never arises.

### Recommendation

- The agreement should state that GDPR lawful basis is **not required** for the majority of shared QMS data (non-personal data)
- For incidental personal data, both parties rely on **legitimate interest** with a documented balancing assessment
- For clinical data, the default approach is **anonymization before sharing**, making lawful basis irrelevant
- Include a brief legitimate interest assessment (LIA) as an annex to the agreement for completeness

---

## 4. Data Processing Agreement: Required Only for Narrow Scope

### When Is a DPA Required?

A DPA under Article 28 GDPR is required only when one party acts as a processor for the other. As analyzed above:
- For non-personal data: No DPA needed
- For the recommended structure (independent controllership): No DPA needed
- A DPA would be required only if Regla were processing personal data on behalf of OptoCeutics (which it is not - Regla processes for its own purposes)

### What to Include Instead

Rather than a DPA, the cooperation agreement should include a **Data Access and Handling Schedule** that covers:

1. **Data classification** (Tier 1/2/3 as described above)
2. **Pseudonymization/anonymization responsibilities** (OptoCeutics before transfer)
3. **Permitted uses** (development, training, validation, productization)
4. **Security measures** (proportionate to data sensitivity)
5. **Retention and deletion** (what happens at termination)
6. **Incident notification** (mutual obligation to notify data breaches)
7. **Confirmation that each party is an independent controller** for any residual personal data

### Can It Be Embedded?

Yes. The Data Access and Handling Schedule should be an annex to the cooperation agreement, not a separate document. This keeps the deal structure simple (one agreement, one NDA embedded, one data schedule attached).

### Recommendation

- Do NOT include a formal Article 28 DPA (it would incorrectly characterize the relationship)
- Include a **Data Access and Handling Schedule** as an annex
- Keep it pragmatic: 2-3 pages maximum
- Focus on classification, responsibilities, and security rather than GDPR boilerplate

---

## 5. AI/ML Training Data: The EDPB Has Opened the Door

### The Current Regulatory Landscape

The EDPB Opinion 28/2024 (December 2024) is the most important regulatory development for AI training data under GDPR. Key holdings:

1. **AI models can be anonymous**: If it is very unlikely that individuals can be identified from the model, and personal data cannot be extracted through queries, the model itself is not personal data. Once data is embedded in model weights through training, it is typically transformed beyond identifiability.

2. **Legitimate interest can justify AI training**: The EDPB confirmed that legitimate interest under Article 6(1)(f) can serve as a lawful basis for processing personal data to develop AI models, subject to the standard three-part balancing test.

3. **Unlawful training does not necessarily taint the model**: Even if personal data was used unlawfully during training, the resulting model may still be lawfully deployed if it has been properly anonymized (though this is a case-by-case assessment).

### Application to Regla's Use Case

Regla's situation is particularly favorable because:

- The training data is **primarily non-personal** (QMS procedures, templates, risk analyses)
- Any personal data in the training data is **incidental** (names in document headers, not targeted collection of personal information)
- The AI model being developed processes **document structures and compliance patterns**, not personal data
- The model outputs are **new QMS documents**, not personal data about identifiable individuals

The risk of personal data extraction from a QMS automation model is negligible. Nobody will query a document generation model to extract the name of OptoCeutics' quality manager.

### Right to Erasure and Model Weights

The EDPB acknowledges the technical challenge of erasing personal data from trained models. For Regla's use case:

- If training data is properly pseudonymized before use, the model weights will not contain identifiable personal data
- The EDPB allows alternatives to retraining: output filtering, documentation of suppression logic
- Given the incidental nature of any personal data in QMS documents, the risk of identifiable data persisting in model weights is extremely low

### Recommendation

- **Pseudonymize all personal data before using it in AI training** (this is the practical safeguard that makes everything else easy)
- Document the training data pipeline including pseudonymization steps
- The agreement should grant Regla the right to use QMS data for AI model training, with the understanding that trained models are independent works that do not contain OptoCeutics' data in recoverable form
- Include a clause stating that Regla's AI models, once trained, are Regla's IP and do not constitute OptoCeutics' confidential information (even though they were trained on it)

---

## 6. Anonymization and Pseudonymization: Practical Standards

### What Level of De-Identification Is Needed?

**For the majority of QMS data**: None. It is not personal data.

**For Category B data (incidental personal data)**:
- **Pseudonymization is sufficient**: Replace names with role codes (e.g., "QA Manager", "Production Lead", "Auditor-01")
- This is simple find-and-replace in most cases
- Pseudonymized data remains personal data under GDPR, but the risk is minimal
- Full anonymization (irreversible) is not required for this level of data

**For Category C data (clinical/patient references)**:
- **Anonymization is required**: Remove all direct and indirect identifiers
- For CERs: clinical data is typically already reported in aggregate
- For vigilance reports: redact patient identifiers, HCP names, reporting institution details
- Statistical data (outcomes, adverse event rates) is inherently anonymous

### Practical Standard for Medtech Co-Development

The industry standard for medtech data sharing partnerships is:

1. **Automated pseudonymization**: Use scripts to replace personal identifiers with codes in document batches
2. **Tiered review**: Quality team reviews Category C data before sharing; Category B is automated
3. **Metadata stripping**: Remove document metadata (author fields, modification history) that may contain employee names
4. **Aggregate clinical data**: Share statistical summaries rather than patient-level data
5. **Living protocol**: Update the pseudonymization protocol as new data types are identified

### Recommendation

- Include a simple **Data Preparation Protocol** in the Data Access Schedule
- OptoCeutics is responsible for pseudonymization before sharing
- Regla should provide pseudonymization tools/scripts as part of the platform (this is itself a product feature)
- Set the standard at pseudonymization for Category B, anonymization for Category C
- Do not over-engineer: a simple find-and-replace protocol handles 95% of cases

---

## 7. Data Access Scope: Broad but Bounded

### The Tension

Regla needs comprehensive access to build a genuinely useful product. But OptoCeutics should not need to share everything, and defining scope too narrowly would hobble development.

### Recommended Scope Definition

**Included (Default Access)**:
- All QMS procedural documents (SOPs, work instructions, quality manuals)
- Document templates and structural hierarchies
- Risk management files and frameworks
- Regulatory submission structures and templates
- Process maps and workflow documentation
- Training records (pseudonymized)
- Internal audit frameworks and methodologies (pseudonymized findings)
- CAPA process documentation and anonymized case examples
- Document control metadata (version history, document relationships)

**Included (On-Request Access)**:
- Clinical evaluation reports (with clinical data anonymized)
- Post-market surveillance reports and summaries
- Specific regulatory submissions (de-identified)
- Complaint handling process documentation (anonymized cases)

**Excluded**:
- Raw patient-level clinical data
- Individual employee personnel files
- Financial data unrelated to QMS
- Legal privilege communications
- Active regulatory correspondence with notified bodies (unless OptoCeutics consents)

### Flexibility Mechanism

Rather than a rigid data catalog, use a **data access request protocol**:
1. Regla requests access to a data category with a stated development purpose
2. OptoCeutics reviews (max 10 business days response time)
3. OptoCeutics either provides access (with pseudonymization if needed) or declines with reason
4. Unreasonable refusal is a breach of the cooperation spirit (soft obligation)
5. Certain core categories (SOPs, templates, risk files) are pre-approved

### Recommendation

- Define broad categories of pre-approved data access (the Included Default list above)
- Create a lightweight request protocol for additional data
- Include a **cooperation obligation** requiring OptoCeutics to provide data reasonably necessary for platform development
- Avoid itemizing individual documents (too rigid, too burdensome to maintain)

---

## 8. Data Security: Proportionate, Not Aspirational

### What Is Proportionate for a Startup?

ISO 27001 or SOC 2 certification would be disproportionate for an early-stage startup. The GDPR requires security measures that are "appropriate to the risk" (Article 32), not best-in-class enterprise security.

### Recommended Security Baseline

**Technical Measures**:
- Encryption at rest and in transit (AES-256, TLS 1.2+)
- Access controls (role-based, principle of least privilege)
- Secure cloud infrastructure (Oracle Cloud Infrastructure with EU data residency)
- Regular backups with encryption
- Logging of data access events
- Multi-factor authentication for system access

**Organizational Measures**:
- Written information security policy
- Employee confidentiality obligations
- Incident response procedure
- Data access limited to personnel who need it for development
- Annual security review

**What NOT to Require**:
- ISO 27001 certification (aspiration, not requirement)
- SOC 2 Type II (expensive, premature for startup)
- Penetration testing by external firm (can be self-assessed initially)
- Dedicated CISO (Regla is ~5 people)

### Growth Path

The agreement should include a **security maturity clause**: Regla commits to implementing security measures proportionate to the sensitivity of data accessed and the scale of operations, with periodic review. As Regla grows and handles more client data, security measures will scale accordingly.

### Recommendation

- Specify concrete technical minimums (encryption, access control, MFA)
- Include organizational measures (policy, incident response, confidentiality)
- Add a proportionality clause acknowledging startup stage
- Include an annual security review obligation
- Avoid requiring specific certifications at this stage

---

## 9. EU MDR Data Retention: No Conflict

### OptoCeutics' Retention Obligations

Under EU MDR Article 10(8), manufacturers must keep technical documentation available for competent authorities:
- **10 years** after the last device is placed on the market (general rule)
- **15 years** for implantable devices

This covers all technical documentation, clinical evaluation reports, post-market surveillance data, and quality management records.

### Interaction with Regla's Data Access

There is **no conflict** between OptoCeutics' retention obligations and data sharing with Regla:

1. **Sharing is not deleting**: Providing Regla with copies of QMS data does not affect OptoCeutics' ability to retain originals
2. **Regla does not replace the QMS**: OptoCeutics maintains its own QMS; Regla's platform supplements it
3. **No regulatory risk from sharing**: EU MDR does not prohibit sharing QMS data with technology partners, provided confidentiality is maintained
4. **Retention applies to OptoCeutics**: Regla has no independent EU MDR retention obligation (Regla is not the device manufacturer)

### Agreement Provision

Include a clause clarifying that:
- Nothing in the cooperation agreement relieves OptoCeutics of its EU MDR retention obligations
- Regla's use of QMS data is independent of OptoCeutics' regulatory retention
- Upon termination, Regla's obligation to delete/return data does not affect OptoCeutics' retained copies

### Recommendation

- Address EU MDR retention in one or two sentences for clarity
- Confirm OptoCeutics retains full control of its regulatory documentation
- No complex provisions needed - this is a non-issue

---

## 10. Data Portability: Not a Concern

### GDPR Data Portability (Article 20)

The right to data portability applies only to personal data provided by the data subject, processed on the basis of consent or contract, and carried out by automated means.

QMS organizational data is not personal data, so Article 20 does not apply. Even for incidental personal data in QMS documents, the data subjects are OptoCeutics' employees - they have no portability right vis-a-vis Regla's platform.

### Commercial Data Portability

The more relevant question is commercial: when Regla builds features based on patterns learned from OptoCeutics' QMS, does OptoCeutics have any claim to those patterns?

The answer is no, provided the agreement clearly establishes:
- Regla owns all IP in the platform
- Patterns, insights, and generalizations derived from OptoCeutics' data are Regla's IP
- OptoCeutics' rights are limited to platform access, not to the underlying platform logic
- The distinction between confidential raw data (protected by NDA) and derived insights (Regla's IP)

### Recommendation

- Data portability under GDPR is not applicable
- Address commercial data rights in the IP section of the agreement
- Clearly distinguish between raw data (OptoCeutics', return/delete on termination) and derived works (Regla's IP, retained permanently)

---

## 11. Cross-Border Data Transfers: Manageable

### The Setup

Both Regla and OptoCeutics are Danish companies. If all data processing occurs within the EU/EEA, no transfer mechanism is needed.

### Cloud Infrastructure Consideration

Regla uses Oracle Cloud Infrastructure (OCI). Key points:

1. **OCI EU data residency**: Oracle offers EU-based data centers (Frankfurt, Amsterdam, Stockholm). If Regla uses an EU region, there is no cross-border transfer issue.

2. **Oracle's GDPR compliance**: OCI has completed EU Code of Conduct Level 2 assessment and offers Binding Corporate Rules for Processors (BCR-p) approved by EU DPAs.

3. **Sub-processor risk**: Oracle may use sub-processors that access data from outside the EU for support purposes. Oracle's DPA and BCR-p address this with Standard Contractual Clauses.

4. **AI model training**: If Regla uses cloud-based AI training services (e.g., calling Anthropic's API), the data sent for inference may leave the EU. Solution: use pseudonymized data for any cloud AI processing, and document the transfer mechanism.

### Practical Approach

- Use EU-based OCI regions for all data storage and processing
- Ensure Oracle's DPA covers any incidental sub-processor access from outside EU
- For AI training involving third-party APIs: pseudonymize all data before sending
- Document the data flow architecture in the Data Access Schedule

### Recommendation

- Include a data residency clause requiring EU storage of OptoCeutics' data
- Reference Oracle's GDPR compliance mechanisms (BCR-p, SCCs)
- Address AI processing separately: pseudonymized data for any non-EU processing
- Keep it simple - this is a solved problem for OCI

---

## 12. Creative Data Access Models: The Maximum Permissible Structure

### The Goal

Give Regla maximum data access and utility while maintaining GDPR compliance and protecting OptoCeutics' interests. Here are the creative approaches:

### Model 1: Tiered Access with Embedded Pseudonymization (Recommended)

This is the primary recommended model:

- **Tier 1**: Unrestricted access to non-personal QMS data. Full copy provided to Regla. Used freely for development, training, productization.
- **Tier 2**: Automated pseudonymization pipeline. OptoCeutics runs a Regla-provided script that strips personal identifiers before export. Regla receives pseudonymized data.
- **Tier 3**: Data clean room approach for sensitive clinical data. Regla's algorithms run on OptoCeutics' systems (or a shared secure environment), extracting patterns without accessing raw patient data.

**Why this works**: It is the simplest structure that addresses all GDPR concerns. No over-engineering, maximum data utility.

### Model 2: Synthetic Data Generation for Sensitive Categories

For Category C data (clinical/patient adjacent):
- OptoCeutics provides anonymized statistical profiles of their clinical data
- Regla uses these profiles to generate synthetic clinical datasets
- Synthetic data retains statistical properties needed for AI training without any personal data
- Regla's platform can be trained on synthetic clinical scenarios

**Advantage**: Completely eliminates GDPR concern for the most sensitive data category. Regla gets realistic training data; OptoCeutics shares no patient-level data.

### Model 3: On-Premises Development Environment (If Needed)

For maximum security during initial development:
- Regla developers work in a secure environment connected to OptoCeutics' QMS
- Data extraction follows the tiered protocol
- Once development patterns are established, move to standard data export

**When to use**: Only if OptoCeutics' management or notified body requires it. Not recommended as default - adds unnecessary friction.

### Model 4: Progressive Data Access

Start with the least sensitive data and expand:
1. **Month 1-2**: Document templates, SOPs, process maps (Tier 1 only)
2. **Month 3-4**: Add risk management files, audit frameworks (Tier 1 + Tier 2)
3. **Month 5+**: Add clinical evaluation frameworks, pseudonymized examples (all tiers)

**Advantage**: Builds trust incrementally. OptoCeutics sees responsible data handling before sharing more sensitive categories.

### Recommendation

Use **Model 1 (Tiered Access)** as the default, supplemented by **Model 2 (Synthetic Data)** for clinical data. Include **Model 4 (Progressive Access)** as an optional comfort mechanism if OptoCeutics prefers gradual rollout.

---

## 13. Audit Rights: Light Touch

### Should OptoCeutics Have Audit Rights?

Yes, but proportionate to the actual risk. The data shared is overwhelmingly non-personal organizational data. Full GDPR-style audit rights (on-site inspections, unlimited scope) would be disproportionate.

### Recommended Audit Framework

**Annual Self-Assessment Report**: Regla provides OptoCeutics with an annual written report confirming:
- Compliance with the data handling schedule
- Security measures in place
- Any incidents or breaches (should be zero for organizational QMS data)
- Data retention and deletion status

**Audit Right on Cause**: OptoCeutics may request a more detailed audit (up to on-site inspection) if:
- Regla reports a data security incident affecting OptoCeutics' data
- OptoCeutics has reasonable grounds to believe the agreement is being breached
- A regulatory authority requires it

**Scope Limitation**: Audit rights cover only data handling practices related to OptoCeutics' data, not Regla's entire business operations, source code, or other clients' data.

**Cost Allocation**: OptoCeutics bears audit costs unless the audit reveals material non-compliance, in which case Regla bears the cost.

### Recommendation

- Annual self-assessment report (low burden, builds trust)
- Audit on cause only (not routine on-site inspections)
- Scope limited to OptoCeutics' data handling
- Reasonable notice period (30 days for on-site)
- Cost allocation as described above

---

## Overall Recommendations: The Maximum Permissible Structure

### Agreement Architecture for Data Access

The cooperation agreement should include a **Data Access and Handling Schedule** (annex) with:

1. **Data Classification** (Tier 1/2/3)
2. **Pre-Approved Data Categories** (broad list of Tier 1 and Tier 2 data)
3. **Data Request Protocol** (for additional data beyond pre-approved)
4. **Pseudonymization Protocol** (OptoCeutics' responsibility, Regla provides tools)
5. **Permitted Uses** (development, training, validation, productization, benchmarking)
6. **Security Baseline** (proportionate technical and organizational measures)
7. **Retention and Termination** (return/delete raw data; retain trained models and derived works)
8. **Audit Provisions** (annual report, audit on cause)
9. **Incident Response** (mutual notification)
10. **EU MDR Acknowledgment** (one sentence confirming no impact on OptoCeutics' regulatory retention)

### What NOT to Include

- A formal DPA (wrong legal instrument for this relationship)
- Joint controller agreement (parties are independent controllers for minimal personal data)
- Excessive GDPR boilerplate (most data is not personal data)
- ISO 27001 or SOC 2 requirements (disproportionate)
- Complex data mapping exercises (simple classification suffices)

### The Boldest Defensible Position

The maximum permissible structure is one where:
- 90%+ of QMS data flows freely under NDA with zero GDPR friction
- Incidental personal data is handled with lightweight pseudonymization
- Clinical data is either anonymized or synthetically generated
- Regla retains all trained models and derived insights as its own IP regardless of termination
- Data access is broad by default, with exclusions being narrow and justified
- Security is real but proportionate to an early-stage startup
- Audit rights exist but are not burdensome

This structure is fully GDPR-compliant, commercially enabling, and practical for both parties.

---

## Sources and References

### Regulatory Sources
- EDPB Opinion 28/2024 on certain data protection aspects related to the processing of personal data in the context of AI models (December 2024)
- CNIL Recommendations on legitimate interest as legal basis for AI system development (June 2025)
- EU MDR 2017/745, particularly Articles 10(8) (retention), 83-86 (post-market surveillance)
- GDPR Articles 4(1), 6(1)(f), 9(2), 20, 26, 28, 32; Recital 26

### Danish Authority Guidance
- Datatilsynet AI in healthcare supervisory priorities for 2025
- Datatilsynet regulatory sandbox for AI and GDPR compliance guidance

### Industry Standards
- ISO 13485:2016 (Quality management systems for medical devices)
- Oracle Cloud Infrastructure EU Code of Conduct Level 2 compliance

### Technical References
- Data clean room architectures for healthcare data collaboration
- Synthetic data generation for GDPR-compliant AI training
- Federated learning approaches for medical device data

---

*This research report is produced by Regla's AI Legal Research System and should be reviewed by qualified legal counsel before being used to draft contractual provisions.*
