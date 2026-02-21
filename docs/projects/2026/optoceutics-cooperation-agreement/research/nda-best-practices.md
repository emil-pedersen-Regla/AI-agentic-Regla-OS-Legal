# NDA Best Practices for Medtech/SaaS Co-Development

**Research Report -- Regla ApS / OptoCeutics Cooperation Agreement**
**Date**: 2026-02-19
**Scope**: Confidentiality and data protection structuring for an AI/SaaS startup co-developing with a medical device company
**Jurisdiction**: Danish law (both parties Danish-connected)

---

## 1. Embedded vs. Standalone NDA: The Structural Question

### Recommendation: Embed, but with a Survival Spine

Embedding the NDA inside the cooperation agreement is the right call for this deal. Here is why -- and where most people get it wrong.

**Advantages of embedding:**
- One document, one signature, one governing law clause, one dispute resolution mechanism. No risk of conflicting terms between a standalone NDA and the cooperation agreement.
- Eliminates the "which document prevails" problem that plagues dual-document structures. In a co-development where the confidentiality obligations are deeply intertwined with the IP, data access, and license terms, separation creates ambiguity.
- Simpler for a 50-person medtech company. OptoCeutics does not have a legal department parsing multiple interrelated agreements.
- Reduces negotiation overhead. One round of negotiation, not two.

**The risk everyone warns about (and why it does not apply here):**
The standard objection is that embedded NDAs die with the agreement. If the cooperation terminates, so does confidentiality. This is a real risk -- but the solution is a properly drafted survival clause, not a separate document. The confidentiality section must explicitly state that it survives termination or expiration of the cooperation agreement for a defined period. This is a two-sentence fix, not a structural problem.

**The elegant structure:**
- The cooperation agreement contains a dedicated Article (e.g., Article 7: Confidentiality) with its own internal structure: definitions, obligations, exclusions, duration, remedies.
- The survival clause in the termination section explicitly lists the confidentiality article as surviving.
- The confidentiality article cross-references the permitted use definitions in the cooperation scope, creating tight alignment between "what you can do with the data" and "what you must keep secret."

This is superior to a standalone NDA because the permitted use scope can directly reference the cooperation terms rather than trying to describe them abstractly.

### What a Mediocre Lawyer Misses

Most embedded NDAs are afterthoughts -- three generic paragraphs buried in the boilerplate. The key is to treat the confidentiality article as a self-contained module within the agreement: internally complete, externally connected. It should read as though it could be extracted and enforced independently, while benefiting from the context of the surrounding agreement.

---

## 2. Defining "Confidential Information": The Smartest Simple Definition

### Recommendation: Broad Catch-All + Specific Carve-Ins + Standard Exclusions

There are three schools of thought on defining confidential information: (1) everything is confidential unless excluded, (2) only specifically marked information is confidential, (3) a hybrid with categories.

For this deal, option (1) with specific carve-ins is optimal. Here is the structure:

**The core definition (one sentence):**
"Confidential Information means all information, whether written, oral, electronic, or visual, disclosed by or on behalf of one Party to the other Party in connection with this Agreement or the cooperation contemplated herein."

**The carve-in list (non-exhaustive, for avoidance of doubt):**
This includes, without limitation:
- (a) Platform technology, AI models, algorithms, source code, and development roadmap (Regla)
- (b) Quality Management System data, procedures, templates, and work instructions (OptoCeutics)
- (c) Business strategy, pricing, financial information, and customer data (both)
- (d) Product data, clinical data, and regulatory submissions (OptoCeutics)
- (e) Trade secrets of either Party

**Why this is better than a marking requirement:**
Marking requirements ("information is only confidential if stamped CONFIDENTIAL") are a trap in co-development. Engineers share things verbally in workshops. Data flows through APIs. QMS documents are accessed in real-time systems. A marking requirement creates a loophole the size of a barn door. The disclosing party forgets to mark one critical document, and it loses protection.

The carve-in list eliminates ambiguity for the most sensitive categories without requiring the parties to maintain a marking discipline they will inevitably fail to follow.

### The Oral Disclosure Problem

Standard NDAs require oral disclosures to be confirmed in writing within 30 days. This is impractical in a co-development where daily interactions generate confidential exchanges. Instead, use a blanket presumption: all information exchanged in connection with the cooperation is confidential, subject to the standard exclusions. This is aggressive but honest about how co-developments actually work.

---

## 3. Duration: The Dual-Track Approach

### Recommendation: Hybrid Duration -- 5 Years General / Perpetual for Trade Secrets

The standard approach is a single fixed term (3-5 years). This is inadequate for two reasons:

1. **Trade secrets deserve perpetual protection.** Under the EU Trade Secrets Directive (implemented in Denmark via the Danish Trade Secrets Act / Lov om forretningshemmeligheder), trade secrets retain legal protection as long as they meet the statutory criteria. An NDA with a 5-year cap on trade secret obligations could be read as extinguishing that protection after 5 years -- a catastrophic result. Recent case law in the US (where much AI IP litigation occurs) has confirmed that NDA expiration can vitiate trade secret protection.

2. **Ordinary confidential information does not need perpetual protection.** Business strategy from 2026 is irrelevant by 2031. Pricing data becomes stale. Perpetual obligations for all information are unreasonable and potentially unenforceable.

**The dual-track structure:**

- **Trade secrets**: Obligations survive for as long as the information qualifies as a trade secret under applicable law. No fixed expiration.
- **All other Confidential Information**: Obligations survive for 5 years from the date of disclosure, or 3 years after termination of the Agreement, whichever is longer.

This structure is defensible, fair to both parties, and avoids the trap of a single duration that is either too short for secrets or too long for stale information. It also aligns with the Danish Trade Secrets Act, which provides independent statutory protection but is strengthened by contractual obligations that explicitly acknowledge the perpetual nature of trade secret protection.

### The Creative Edge

Add a "declassification" mechanism: either party may notify the other that specific information is no longer considered Confidential Information (e.g., because it has been published, or because the business strategy has changed). This gives both parties an escape valve for information that has lost its sensitivity, reducing the burden of perpetual obligations without requiring formal amendment.

---

## 4. Exclusions: Standard + Two Non-Standard Additions

### Standard Exclusions (Must Include)

Every NDA excludes these categories. Omitting them creates enforceability risk:

1. **Public domain**: Information that is or becomes publicly available through no fault of the receiving party.
2. **Prior knowledge**: Information already known to the receiving party before disclosure (with burden of proof on the receiving party via contemporaneous records).
3. **Independent development**: Information independently developed by the receiving party without use of or reference to the disclosing party's Confidential Information.
4. **Third-party disclosure**: Information received from a third party who is not bound by confidentiality obligations to the disclosing party.
5. **Legal compulsion**: Information required to be disclosed by law, regulation, or court order (with prior notice to the disclosing party where legally permitted).

### Non-Standard Exclusion #1: Regulatory Disclosure Carve-Out

This is medtech-specific and critical. OptoCeutics may need to disclose QMS-related information to Notified Bodies, the Danish Medicines Agency (Laegemiddelstyrelsen), or EU competent authorities during audits, inspections, or regulatory submissions. Regla may need to disclose platform-related information if its software is ever classified as a medical device or SaMD.

The exclusion should permit disclosure to regulatory authorities to the extent required by applicable medical device regulations (EU MDR 2017/745, ISO 13485) without triggering a breach. This is not the same as the generic "legal compulsion" exclusion -- it specifically covers the proactive regulatory disclosure obligations that medtech companies face.

### Non-Standard Exclusion #2: Aggregated/Anonymized Data

Regla will inevitably want to use insights derived from OptoCeutics' QMS data to improve its platform for other customers. The clean way to handle this is an explicit exclusion for aggregated, de-identified, or anonymized data that cannot reasonably be re-identified to OptoCeutics or any individual. This is distinct from the residuals clause (discussed in Section 8) and provides a clear, auditable basis for using derived insights.

---

## 5. Permitted Use: The Hardest Clause in This Agreement

### The Core Tension

Regla is using OptoCeutics' confidential QMS data to build a product it will sell to OptoCeutics' competitors. This is the single most sensitive aspect of the NDA. If the permitted use clause is too narrow, Regla cannot build its product. If it is too broad, OptoCeutics has no meaningful protection.

### Recommendation: Purpose-Limited Use with Platform Abstraction

**The structure:**

"Each Party shall use the other Party's Confidential Information solely for the purposes of performing its obligations and exercising its rights under this Agreement (the 'Permitted Purpose')."

This is then operationalized through a specific carve-out for Regla:

"For the avoidance of doubt, the Permitted Purpose includes Regla's use of OptoCeutics' Confidential Information to develop, improve, train, validate, and test the Platform, including the creation of generalized Platform features, templates, and AI models, provided that:
(a) no Confidential Information of OptoCeutics is disclosed to third parties in identifiable form;
(b) the Platform does not reproduce, display, or output OptoCeutics' Confidential Information to other users in identifiable form; and
(c) any AI models trained using OptoCeutics' Confidential Information do not enable extraction or reconstruction of such Confidential Information."

### Why This Works

This gives Regla the operational freedom to build its product while giving OptoCeutics three concrete, verifiable protections:
1. No identifiable disclosure to third parties (competitors cannot see OptoCeutics' specific QMS).
2. No identifiable output (the platform does not spit out OptoCeutics' documents to other users).
3. No extraction from AI models (the model learns patterns, but cannot be reverse-engineered to reveal OptoCeutics' data).

The word "identifiable" is doing heavy lifting here. It permits Regla to create generalized templates, workflows, and AI capabilities informed by OptoCeutics' data, while preventing the specific data from leaking. This is the abstraction layer that makes the entire co-development commercially viable.

### The Non-Compete Alternative (Rejected)

Some lawyers would suggest restricting Regla from selling to OptoCeutics' direct competitors. This is a terrible idea. It destroys Regla's business model (the entire point is to sell to the medtech industry) and is likely unenforceable under Danish competition law for being disproportionate. The permitted use structure above achieves the same protection through data abstraction rather than market restriction.

---

## 6. Return/Destruction of Information: The AI Problem

### Why Traditional "Return or Destroy" Fails

Traditional NDAs require the receiving party to return or destroy all copies of Confidential Information upon termination. This was designed for a world of paper files and USB drives. It breaks completely in three scenarios present in this deal:

1. **AI model training**: When QMS data trains an AI model, the data is transformed into model weights and parameters. The original data is not "stored" in any retrievable sense -- it has been mathematically transformed. You cannot "return" what no longer exists in its original form, and you cannot "destroy" model weights without destroying the entire model.

2. **Automated backups**: Both parties will have automated cloud backup systems. Selectively purging specific files from encrypted backup archives is technically impractical and sometimes impossible.

3. **Derived works**: Regla will create platform features, templates, and algorithms informed by OptoCeutics' data. These are not copies of the Confidential Information, but they were created using it.

### Recommendation: Tiered Return/Destruction with AI Carve-Out

**Tier 1 -- Raw Data (strict obligation):**
All copies of OptoCeutics' raw QMS documents, data exports, and unprocessed data files must be returned or destroyed within 30 days of termination. Certification of destruction required.

**Tier 2 -- Backup exception:**
Copies retained in automated backup systems or disaster recovery archives need not be actively purged, provided they remain encrypted, are not actively accessed, and are destroyed in the ordinary course of backup rotation. Confidentiality obligations continue to apply.

**Tier 3 -- AI Model Carve-Out (the creative solution):**
AI models trained using OptoCeutics' Confidential Information need not be destroyed, provided that: (a) the models do not enable extraction or reconstruction of OptoCeutics' Confidential Information in identifiable form; (b) Regla's confidentiality and non-disclosure obligations with respect to OptoCeutics' Confidential Information continue to apply to such models in perpetuity; and (c) Regla does not further train such models on OptoCeutics' Confidential Information after termination.

**Tier 4 -- Derived works:**
Platform features, templates, algorithms, and other works derived from but not containing OptoCeutics' Confidential Information in identifiable form are not subject to return or destruction obligations, but are subject to the ongoing confidentiality obligations regarding the underlying Confidential Information.

### Why This is State of the Art

This tiered approach acknowledges the technical reality of AI systems while preserving meaningful protection. The key innovation is separating the obligation (confidentiality continues) from the remedy (you do not have to destroy what cannot technically be destroyed). Most NDAs still use binary "return or destroy" language that is either unenforceable or would require destroying Regla's entire platform -- neither outcome serves either party.

---

## 7. Medtech-Specific Considerations

### QMS Data is Not Ordinary Business Information

Quality Management System data in the medical device industry occupies a unique position. It is simultaneously:
- **Trade secret**: Proprietary processes, work instructions, and quality procedures represent significant competitive advantage.
- **Regulated content**: Required by ISO 13485 and EU MDR. Notified Bodies audit it. Competent authorities can demand access.
- **Patient-safety-adjacent**: While QMS data is not patient data per se, it directly affects the safety and performance of medical devices. Errors in QMS documentation can lead to patient harm.

### Specific NDA Implications

**1. Regulatory audit access:**
The NDA must not prevent OptoCeutics from sharing QMS information with Notified Bodies, competent authorities, or auditors. A blanket confidentiality obligation without a regulatory carve-out could put OptoCeutics in the impossible position of choosing between NDA compliance and regulatory compliance. Regulatory compliance wins every time, so the NDA should explicitly accommodate it.

**2. Post-market surveillance data:**
If Regla's platform processes post-market surveillance data or vigilance reports, this data may contain information about device malfunctions, adverse events, or safety concerns. The NDA should address Regla's obligations if it becomes aware of safety-relevant information through the cooperation -- specifically, that confidentiality obligations do not override regulatory reporting obligations.

**3. Notified Body audit scope:**
During ISO 13485 or EU MDR audits, Notified Bodies may inquire about tools and software used in QMS management. OptoCeutics should be permitted to disclose the existence and general nature of the Regla platform (that they use an AI tool for QMS documentation) without disclosing Regla's proprietary details (algorithms, pricing, etc.). This requires a calibrated disclosure permission, not a blanket carve-out.

**4. Clinical data handling:**
If OptoCeutics shares clinical evaluation data, post-market clinical follow-up data, or other clinical data, GDPR and the Clinical Trials Regulation may impose additional obligations. The NDA should cross-reference the data access terms elsewhere in the agreement and should not create a parallel confidentiality regime for data that is already governed by data protection law.

---

## 8. The Residuals Clause: Aggressive but Necessary for Regla

### What It Is

A residuals clause permits the receiving party to freely use ideas, concepts, know-how, and techniques retained in the unaided memory of its personnel after exposure to confidential information. In traditional NDAs, this addresses the practical reality that people cannot selectively erase memories.

### Why Regla Needs It

Regla's engineers and product designers will spend months deeply embedded in OptoCeutics' QMS processes. They will develop intuitions about how medical device companies manage quality, what pain points exist, what workflows are efficient. This general knowledge is essential for building a product that serves the entire industry. Without a residuals clause, Regla's own employees become toxic -- every product decision could be challenged as derived from OptoCeutics' Confidential Information.

### Why OptoCeutics Will Resist It

From OptoCeutics' perspective, a broad residuals clause could effectively nullify the NDA. If Regla's engineers can freely use "everything they remember," what exactly is the NDA protecting?

### The Creative Solution: Scoped Residuals with Guardrails

Draft the residuals clause with five specific constraints:

1. **Unaided memory only**: No notes, no recordings, no deliberate memorization exercises. The knowledge must be genuinely retained in human memory without intentional effort to memorize.

2. **General knowledge only**: The residuals right applies to general concepts, methodologies, know-how, and techniques -- not to specific documents, data, formulas, customer lists, pricing, or trade secrets.

3. **No IP license**: The residuals clause does not grant any license under OptoCeutics' patents, copyrights, or other intellectual property rights. Knowing how something works does not give you the right to copy it.

4. **Personnel limitation**: Applies only to Regla employees and contractors who were directly involved in the cooperation, not to the entire organization.

5. **Exclusion of trade secrets**: Trade secrets are explicitly excluded from the residuals clause. This is the critical constraint that makes the clause palatable to OptoCeutics while still useful to Regla. General QMS methodology knowledge is usable; OptoCeutics' specific proprietary processes are not.

### The AI Twist

Here is where this gets genuinely novel: does the "residuals" concept apply to AI models? If a model is trained on OptoCeutics' data and the training data is subsequently deleted, the model's "learned knowledge" is analogous to an engineer's residual memory. The model retains patterns and capabilities derived from the data without retaining the data itself.

The recommended approach is to keep the residuals clause strictly limited to human memory and address AI model retention separately in the return/destruction provisions (Section 6 above). Conflating the two creates unnecessary legal ambiguity. Human residuals have decades of legal precedent. AI model residuals are uncharted territory and deserve their own bespoke treatment.

---

## 9. Breach Remedies: What Actually Works Under Danish Law

### The Standard Toolkit

**1. Injunctive relief (fogedforbud / forelobigt forbud):**
Under Danish law, interim injunctions are available through the Danish Maritime and Commercial High Court (So- og Handelsretten) or ordinary district courts via Part 40 of the Danish Administration of Justice Act (Retsplejeloven). The threshold requires the claimant to demonstrate: (a) a prima facie case of breach, (b) urgency (risk of irreparable harm if relief is delayed), and (c) proportionality.

For confidentiality breaches, injunctive relief is generally available because damages are inherently difficult to quantify -- once a secret is disclosed, monetary compensation cannot undo the disclosure. The agreement should include a clause acknowledging that breach of confidentiality may cause irreparable harm for which monetary damages would be an inadequate remedy, and that the disclosing party is entitled to seek injunctive or other equitable relief.

**2. Damages (erstatning):**
Standard contractual damages under Danish law follow the principle of full compensation (fuldstaendig erstatning). The claimant must prove: (a) breach, (b) loss, (c) causation, and (d) adequacy. For confidentiality breaches, quantifying loss is notoriously difficult. The agreement can help by specifying minimum damages or agreed valuation methods.

**3. Contractual penalty (konventionalbod):**
Danish law permits contractual penalty clauses, which are enforceable subject to the reasonableness standard in the Danish Contracts Act (Aftalelovens) Section 36 (the general reasonableness clause). A well-calibrated penalty clause avoids the proof-of-loss problem inherent in confidentiality breaches.

### Recommendation: Layered Remedies

**Layer 1 -- Injunctive relief acknowledgment:**
Both parties acknowledge that breach may cause irreparable harm and consent to the jurisdiction of Danish courts for injunctive relief. This does not create the right (courts decide) but establishes the factual premise and avoids the receiving party arguing that damages would be adequate.

**Layer 2 -- Contractual penalty for material breach:**
Include a penalty of a fixed amount (e.g., DKK 500,000 / approximately EUR 67,000) for each material breach of the confidentiality obligations, payable without proof of actual loss. This amount should be calibrated to be meaningful but not so high as to trigger Section 36 reasonableness review.

**Layer 3 -- Additional damages:**
The contractual penalty does not limit either party's right to claim additional damages to the extent actual losses exceed the penalty amount.

**Layer 4 -- Audit rights:**
Each party has the right to conduct a reasonable audit (or appoint an independent third party to audit) the other party's compliance with the confidentiality obligations, upon reasonable notice and no more than once per calendar year. This is unusual in NDAs but powerful in co-development agreements where data access is ongoing.

### The Creative Edge: Graduated Response

Rather than a binary "breach / no breach" framework, include a notification and cure mechanism for inadvertent breaches. If a party discovers it has inadvertently disclosed Confidential Information (e.g., an employee accidentally included OptoCeutics data in a presentation), it must notify the other party within 48 hours and take all reasonable steps to mitigate the breach. Inadvertent breaches that are timely notified and effectively mitigated do not trigger the contractual penalty (though injunctive relief and damages remain available). This encourages transparency over concealment and is particularly important in an AI context where data leakage may be technical and unintentional.

---

## 10. AI/ML-Specific NDA Challenges: State of the Art

### The Fundamental Problem

Traditional NDA concepts assume information exists as discrete, identifiable units that can be copied, disclosed, returned, or destroyed. AI/ML breaks every one of these assumptions:

- **Copying**: Training an AI model on data is not "copying" in the traditional sense. The data is transformed into mathematical parameters.
- **Disclosure**: When an AI model generates output informed by training data, is that "disclosure" of the training data? If a model trained on OptoCeutics' QMS data generates a generic QMS template for another customer, has OptoCeutics' data been "disclosed"?
- **Return/Destruction**: As discussed in Section 6, you cannot return or destroy information that has been transformed into model weights.
- **Identification**: It is often technically impossible to determine whether a specific piece of training data influenced a specific model output.

### Current Best Practice: The Three-Layer Framework

Based on emerging practice and the latest guidance, the state of the art for AI/ML confidentiality involves three interlocking layers:

**Layer 1 -- Input Controls (what goes into the AI):**
- Explicit consent for which categories of Confidential Information may be used for AI training.
- Prohibition on using Confidential Information in third-party AI services (public LLMs, cloud AI APIs) without the disclosing party's written consent.
- Technical controls: data must be processed in secure environments with access controls.
- Logging: maintain records of which data was used for training which models.

**Layer 2 -- Output Controls (what comes out of the AI):**
- The AI platform must not output, display, or transmit Confidential Information in identifiable form to unauthorized persons.
- Output filtering: technical measures to prevent the model from reproducing or reconstructing identifiable Confidential Information.
- Regular testing: periodic evaluation that models do not leak training data (membership inference attacks, data extraction attempts).

**Layer 3 -- Lifecycle Controls (what happens over time):**
- Model versioning: track which models were trained on which data.
- Retraining obligations: if OptoCeutics requests deletion, Regla should be prepared to retrain models without OptoCeutics' data (acknowledging this may be commercially impractical and should be a last resort).
- Successor models: new model versions that are not trained on OptoCeutics' data supersede older versions, reducing the data footprint over time.

### The Contractual Innovation

The most creative structuring option is to define a new concept: "Derived Intelligence." This is distinct from both Confidential Information and from independently developed information. Derived Intelligence means the patterns, capabilities, weightings, and parameters of AI models that were developed using Confidential Information but that do not contain, reproduce, or enable extraction of the Confidential Information in identifiable form.

Derived Intelligence is:
- Not subject to return/destruction obligations
- Subject to ongoing confidentiality obligations regarding the source data
- Owned by Regla (consistent with the IP ownership structure)
- Not transferable to third parties without the platform (i.e., Regla cannot sell the raw model weights to a competitor)

This concept is not yet standard in any jurisdiction, but it accurately describes the technical reality and provides a contractual framework that both parties can work with.

---

## Summary of Recommendations

| Topic | Recommendation | Aggressiveness |
|-------|---------------|----------------|
| Structure | Embed NDA in cooperation agreement with survival spine | Moderate |
| Definition | Broad catch-all + specific carve-ins, no marking requirement | Moderate-Aggressive |
| Duration | 5 years general / perpetual for trade secrets | Moderate |
| Exclusions | Standard 5 + regulatory carve-out + anonymized data | Moderate |
| Permitted use | Purpose-limited with platform abstraction layer | Aggressive-Creative |
| Return/destroy | Four-tier system with AI model carve-out | Aggressive-Creative |
| Medtech-specific | Regulatory audit carve-outs, safety reporting override | Moderate |
| Residuals | Scoped to human memory with 5 guardrails, trade secrets excluded | Aggressive |
| Remedies | Layered: injunction + penalty + damages + audit rights | Moderate-Aggressive |
| AI/ML | Three-layer framework (input/output/lifecycle) + Derived Intelligence concept | Cutting-Edge |

---

## Key Sources and References

- [AI Clauses in NDAs: Protecting Confidentiality Without Killing Collaboration](https://www.avantialaw.com/news/ai-clauses-in-ndas-protecting-confidentiality-without-killing-collaboration)
- [7 AI-Specific Confidentiality Clauses](https://contractnerds.com/7-ai-specific-confidentiality-clauses/)
- [Keep it Confidential: NDAs in the AI Era (Lexology)](https://www.lexology.com/library/detail.aspx?g=ce7f1325-bfb1-47fd-a7c9-45c6d644736f)
- [Steal this NDA template to protect your data from AI training](https://blog.stackaware.com/p/nda-legal-agreement-ai-unintended-training)
- [What You Need to Know About Residual Information Clauses in NDAs](https://www.howtocontract.com/nda/residual-information-clause)
- [Beware Residuals Clauses when Disclosing Confidential Information](https://www.theiaengine.com/article/beware-residuals-clauses-when-disclosing-confidential-information/)
- [Residuals Clause - NDA Clause Library](https://terms.law/NDA/clause-library/residuals-clause.html)
- [Incorporating AI Training Language in Confidentiality Provisions](https://www.outsidegc.com/blog/incorporating-ai-training-language-in-confidentiality-provisions)
- [Non-Disclosure Agreements 2.0: AI Provisions (Roth Jackson)](https://www.rothjackson.com/blog/2025/12/non-disclosure-agreements-2-0-why-its-crucial-to-include-ai-provisions-in-your-non-disclosure-agreements/)
- [Common NDA Clauses to Include (2026 Guide)](https://www.pactly.com/blog/common-nda-clauses-to-include)
- [Danish Trade Secrets Act (WIPO Lex)](https://wipolex-res.wipo.int/edocs/lexdocs/laws/en/dk/dk230en.html)
- [Danish Marketing Practices Act (WIPO Lex)](https://www.wipo.int/wipolex/en/legislation/details/19554)
- [Injunctive Relief - NDA Clause Library](https://www.terms.law/NDA/clause-library/injunctive-relief.html)
- [NDA Law: Enforceability, Confidentiality, and Remedies](https://legalclarity.org/nda-law-enforceability-confidentiality-and-remedies/)
- [NDA Duration and Surviving Obligations](https://www.everynda.com/blog/duration-clauses-non-disclosure/)
- [How to Define Confidential Information in NDA](https://www.legalgps.com/nda/blog/how-to-define-confidential-information-in-nda)
