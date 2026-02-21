# Mutual Protection & Liability: Research Report

**Project**: OptoCeutics Co-Development Cooperation Agreement
**Research Stream**: D - Mutual Protection & Liability
**Date**: 2026-02-19
**Agent**: Mutual Protection & Liability Researcher

---

## Executive Summary

This report addresses how to structure mutual protection, liability, indemnification, termination, and dispute resolution between Regla ApS (5-person AI startup) and OptoCeutics (~50-person medical device company) for a co-development cooperation agreement under Danish law. The core design principle is **maximum protection with minimum complexity** -- achieving in 4-6 elegant clauses what mediocre agreements attempt in 40 pages.

The central insight: this is not a vendor-customer relationship. It is a **mutual investment partnership** where both parties are contributing time, knowledge, and resources without cash changing hands. Traditional SaaS liability frameworks (capped at 12 months of fees) do not apply because there are no fees. The liability architecture must be built from first principles around what each party actually risks.

---

## 1. Liability Cap Structure

### The Problem with Symmetric Caps

A symmetric liability cap (e.g., both parties capped at EUR 100,000) sounds fair but is structurally unfair. EUR 100,000 is existential for a 5-person startup and a rounding error for a 50-person company. Symmetry of number produces asymmetry of impact.

### The Problem with Fee-Based Caps

The standard SaaS approach -- capping liability at 12 months of fees paid -- produces a cap of zero here, since OptoCeutics pays nothing for platform access. This is unusable.

### Recommended Approach: Proportionate Contribution-Based Cap

Structure the cap around what each party actually stands to lose in the cooperation, not around a notional contract value.

**Recommended structure:**

- **General liability cap for each party**: EUR 50,000 -- equivalent to roughly one year's worth of dedicated development effort from a single contributor. This is meaningful enough to incentivize careful performance without being existential for the startup.
- **Enhanced cap for data-related breaches**: 2x the general cap (EUR 100,000). This recognizes that OptoCeutics' QMS data is their crown jewel and a breach has outsized consequences.
- **Uncapped liability** for fraud, willful misconduct, and breaches of the confidentiality/IP ownership clauses (see Section 5 below).

**Why this works:** The cap is low enough that Regla can survive a worst-case general liability scenario, high enough that both parties take their obligations seriously, and the tiered structure puts extra skin in the game on the data protection obligations that matter most to OptoCeutics.

**Alternative considered and rejected:** Revenue-share-based cap (e.g., cap grows as Regla's revenue grows). Too complex to administer and creates perverse incentives where OptoCeutics benefits from Regla's failure.

### Danish Law Context

Under Danish contract law, there are no statutory controls on financial caps to limit liability for breach of contract in B2B relationships. The principle of freedom of contract (aftalefrihed) governs. However, Section 36 of the Danish Contracts Act (Aftalelov) allows courts to adjust or set aside terms that are unfair or contrary to good faith. In practice, the threshold for setting aside a negotiated liability limitation between two professional parties is very high. The key requirement is that the clause must be clear, unambiguous, and genuinely negotiated (not buried in standard terms). A negotiated cooperation agreement between two companies easily meets this standard.

**Critical limitation under Danish law:** Liability exclusions and caps generally do not apply to liability caused by intent (forsaet) and, in most cases, gross negligence (grov uagtsomhed). This is a background principle of Danish law that applies even if the contract is silent on it. The agreement should make this explicit rather than leaving it to default law.

---

## 2. Consequential Damages

### Standard Practice vs. This Deal

Standard commercial contracts exclude consequential (indirect) damages -- lost profits, lost business opportunity, reputational harm, etc. This is normally sensible because it limits unpredictable exposure.

**However**, in a co-development cooperation where both parties are investing significant time and resources without immediate cash compensation, a blanket exclusion of consequential damages creates a troubling dynamic: if either party performs badly, the other party has invested months of work with no real remedy, since direct damages in a no-fee arrangement are minimal.

### Recommended Approach: Targeted Inclusion

Rather than a blanket exclusion or inclusion, use a **targeted approach**:

- **Exclude** consequential damages as the default for general performance issues.
- **Include** consequential damages (up to the enhanced cap) for two specific scenarios:
  1. **Breach of confidentiality obligations** -- If Regla leaks OptoCeutics' QMS data, the consequential damage to OptoCeutics is the real harm. Limiting them to direct damages only would mean they recover essentially nothing despite catastrophic loss.
  2. **Breach of IP ownership provisions** -- If OptoCeutics claims IP rights they do not have, Regla's consequential loss (inability to commercialize, investor concerns) is the real harm.
- **Always exclude** purely speculative damages (e.g., "we would have won a contract if your platform worked better").

**Why this is elegant:** It creates real accountability on the two issues that actually matter (data confidentiality and IP ownership) while preventing open-ended exposure on general performance complaints.

---

## 3. Indemnification

### Minimum Necessary Set

Indemnification means one party agrees to defend the other and pay for losses arising from specific third-party claims. The key question is: what third-party claims could realistically arise from this cooperation?

**Regla indemnifies OptoCeutics for:**
1. **Third-party IP infringement claims** arising from the platform itself (not from OptoCeutics' data fed into it). If Regla's software infringes someone else's patent or copyright, Regla should hold OptoCeutics harmless.
2. **Data breach claims by third parties** if the breach is caused by Regla's failure to comply with agreed security standards. If OptoCeutics' data is exposed because Regla had inadequate security, Regla bears the cost of third-party claims.

**OptoCeutics indemnifies Regla for:**
1. **Third-party IP infringement claims** arising from OptoCeutics' QMS data or materials provided to Regla. If the data OptoCeutics provides infringes third-party rights, OptoCeutics should hold Regla harmless.
2. **Regulatory non-compliance claims** if OptoCeutics uses platform output without the required human review and a regulatory body takes action. The platform generates draft documentation; OptoCeutics is responsible for validating and approving it.

**Not included (and why):**
- General indemnification for "any breach of this agreement" -- too broad, converts every contract breach into an indemnification claim, and is unnecessary given the liability cap structure.
- Indemnification for employee claims -- not relevant to this cooperation.
- Cross-indemnification for "any loss whatsoever" -- vague and unenforceable under Danish law's clarity requirements.

### Indemnification Procedure

Keep it to three conditions (standard but necessary):
1. Prompt written notice of the claim.
2. The indemnifying party gets to control the defense.
3. The indemnified party cooperates reasonably.

### Cap on Indemnification

Indemnification obligations should be **subject to the enhanced cap** (EUR 100,000), not uncapped. Rationale: uncapped indemnification is only as good as the indemnifying party's assets. Regla is a 5-person startup. An uncapped indemnification from Regla is effectively capped at Regla's total assets anyway, and the illusion of unlimited coverage gives OptoCeutics false comfort. Better to set a realistic cap that both parties can actually honor, supplemented by insurance requirements (see Section 6).

**Exception:** Indemnification for breaches caused by fraud or willful misconduct remains uncapped.

---

## 4. Warranty Provisions

### The Elegant Minimum

Warranties should be narrow, specific, and actually meaningful. Every warranty creates a potential breach, so only warrant what you can actually stand behind.

**Regla warrants:**
1. **Authority and capacity**: Regla has the right to enter this agreement and perform its obligations.
2. **Non-infringement**: The platform (excluding OptoCeutics-provided data) does not, to Regla's knowledge, infringe third-party IP rights.
3. **Reasonable care**: Regla will develop the platform using reasonable professional care and skill. (NOT that it will be error-free, NOT that it will meet specific performance targets, NOT that it will comply with EU MDR -- those are OptoCeutics' responsibility to verify.)
4. **Security standards**: Regla will implement and maintain reasonable technical and organizational security measures for data protection.

**OptoCeutics warrants:**
1. **Authority and capacity**: OptoCeutics has the right to enter this agreement and share its QMS data.
2. **Data rights**: OptoCeutics has all necessary rights, licenses, and permissions to provide its QMS data and materials for the purposes contemplated by this agreement, and such data does not infringe third-party rights.
3. **Data accuracy**: The QMS data and materials provided are accurate and complete to the best of OptoCeutics' knowledge. (This is critical -- if Regla builds on inaccurate data, the product is flawed and Regla needs recourse.)
4. **Regulatory status**: OptoCeutics is responsible for its own regulatory compliance and will not rely on platform output without appropriate professional review and validation.

**Explicitly NOT warranted (by either party):**
- Fitness for a particular purpose. The platform is being co-developed; neither party can warrant the outcome of a joint development effort.
- Uninterrupted or error-free operation. It is development-stage software.
- Compliance with any specific regulatory standard. The platform assists with compliance documentation; it does not certify compliance.

### Warranty Duration

Warranties of authority, capacity, and non-infringement: for the term of the agreement.
Warranty of data accuracy: at the time each data set is provided (a point-in-time warranty, not ongoing).

---

## 5. Limitation of Liability Exceptions (Carve-Outs)

The liability cap exists to provide predictability. But certain behaviors are so serious that capping them would undermine the entire agreement's integrity. The following should be **excluded from the general liability cap** (meaning liability is uncapped for these):

1. **Fraud or intentional misconduct** -- Standard under Danish law; caps generally do not apply to intentional wrongdoing regardless.
2. **Gross negligence** -- Consistent with Danish legal principles; explicitly stating this avoids ambiguity.
3. **Breach of confidentiality obligations regarding the other party's trade secrets** -- If Regla leaks OptoCeutics' QMS to competitors, or OptoCeutics leaks Regla's platform IP, the damage far exceeds any reasonable cap.
4. **Breach of IP ownership provisions** -- If OptoCeutics challenges Regla's IP ownership or if Regla misappropriates OptoCeutics' proprietary QMS methodology, this strikes at the foundation of the deal.

**Not excluded from cap (and why):**
- General data breaches (covered by enhanced cap, not uncapped). A data breach due to ordinary negligence should be subject to the enhanced cap. Only a breach due to gross negligence or intentional conduct should be uncapped.
- General performance failures. If the platform does not work well, the remedy is termination, not unlimited liability.
- Breach of warranty. Warranties operate within the cap structure.

### Drafting Note

The carve-out clause should be structured as: "The limitations set forth in Section [X] shall not apply to liability arising from: (a) fraud or willful misconduct; (b) gross negligence; (c) breach of Section [confidentiality]; or (d) breach of Section [IP ownership]." Clean, one sentence, four items.

---

## 6. Insurance Requirements

### Proportionate to Party Size

Mandating comprehensive insurance in a cooperation agreement between a startup and a medium company requires proportionality.

**Recommended:**

- **Regla**: Professional indemnity (errors & omissions) insurance with minimum coverage of EUR 250,000 and cyber liability insurance with minimum coverage of EUR 250,000. These are obtainable and affordable for a startup (typically EUR 2,000-5,000/year combined for a 5-person tech company).
- **OptoCeutics**: General commercial liability insurance (which they almost certainly already maintain as a medical device company).
- **Both parties**: Must maintain insurance for the duration of the agreement plus 12 months after termination (tail coverage).

**Why this matters:** Insurance fills the gap between the liability cap (EUR 50,000-100,000) and the realistic cost of a major incident (potentially much higher). It gives OptoCeutics comfort that Regla's indemnification obligations are backed by something beyond a startup's balance sheet, without requiring Regla to carry disproportionate insurance costs.

**Not recommended:** Mandating specific coverage amounts above EUR 250,000 for Regla. This would be disproportionate to the cooperation's value and could make the deal uneconomic for Regla.

---

## 7. Termination Rights

### For Cause

Either party may terminate immediately (or with 14 days' cure period for curable breaches) if:

1. **Material breach** that is not cured within 30 days of written notice.
2. **Insolvency or bankruptcy** of the other party (including filing for administration, appointment of receiver, or cessation of business).
3. **Breach of confidentiality or IP obligations** -- immediate termination right, no cure period. These are foundational obligations; once breached, trust is broken.
4. **Change of control** -- if either party is acquired by a competitor of the other party, the non-acquired party gets a termination right. (This protects Regla if OptoCeutics is acquired by a company hostile to Regla, and protects OptoCeutics if Regla is acquired by a direct competitor.)

### For Convenience

This is where the asymmetry needs careful thought:

- **OptoCeutics**: Can terminate for convenience with **90 days' written notice**. This gives Regla time to find alternative data sources and adjust development plans, but does not trap OptoCeutics in a relationship that is not working.
- **Regla**: Can terminate for convenience with **90 days' written notice**. Same reasoning applies.
- **Minimum cooperation period**: Consider a **12-month initial term** during which neither party can terminate for convenience. This protects both parties' investment in the initial development phase. After 12 months, for-convenience termination becomes available.

**Why 90 days:** Short enough to not feel like a trap, long enough to wind down data access, complete in-progress work, and transition gracefully.

### Wind-Down Period

Upon any termination, a **60-day wind-down period** applies during which:
- Regla completes any in-progress documentation tasks.
- Both parties cooperate to separate shared resources.
- Data return/deletion procedures are initiated.

---

## 8. Termination Consequences

This is the most nuanced area of the agreement because of the AI training dimension.

### What Survives Termination

1. **OptoCeutics' platform license**: The perpetual, royalty-free license to use the platform **survives termination**. This is the core of the deal -- OptoCeutics is investing time and data in exchange for permanent access. Revoking this on termination would make the cooperation worthless to them.
   - **Condition**: The surviving license covers the platform version existing at termination. It does not include future updates or development.
   - **Support**: No ongoing support obligation survives, unless separately agreed.

2. **Confidentiality obligations**: Survive for **5 years after termination**. Standard and appropriate.

3. **IP ownership provisions**: Survive indefinitely. IP ownership does not expire.

4. **Indemnification obligations**: Survive for **3 years after termination** for claims arising from events during the cooperation term.

5. **Liability cap and exclusions**: Survive to the extent they relate to surviving obligations.

### The AI Training Question

**This is the critical novel issue.** During the cooperation, Regla will use OptoCeutics' QMS data to develop, train, validate, and improve the platform. Some of this data will be incorporated into the platform's knowledge, model weights, or training datasets. Upon termination, you cannot simply "un-train" an AI model.

**Recommended approach:**

- **Distinguish between raw data and derived knowledge.** Raw QMS documents belong to OptoCeutics and must be returned or deleted within 60 days of termination. Regla provides a deletion certificate.
- **Derived knowledge retained.** The platform's learned patterns, model improvements, validation benchmarks, and generalized knowledge derived from OptoCeutics' data may be retained by Regla. This is analogous to a consultant who learns from a client's business -- the specific documents are returned, but the expertise gained cannot be unlearned.
- **Anonymization obligation.** Any retained derived data must be sufficiently anonymized that OptoCeutics' specific QMS content, trade secrets, or proprietary methodologies cannot be reconstructed or identified.
- **No reverse engineering.** Regla must not use retained knowledge to reverse-engineer or reconstruct OptoCeutics' specific QMS documentation.

**Why this works for both parties:**
- **OptoCeutics** is protected because their raw data is deleted, retained knowledge is anonymized, and reverse engineering is prohibited.
- **Regla** is protected because they can continue developing the platform without having to lobotomize their AI model.

**Draft the clause to be explicit:** "Upon termination, Regla shall delete all OptoCeutics Confidential Information in its original form within 60 days and provide written certification thereof. Regla may retain generalized, anonymized knowledge derived from the cooperation, provided that such retained knowledge does not enable identification or reconstruction of OptoCeutics' specific confidential information, trade secrets, or proprietary QMS content."

---

## 9. Force Majeure

### Worth Including?

Yes, but only as a lean, single-paragraph clause. Under Danish law, force majeure can be invoked as a reason to be exempt from liability even without an express contractual clause, provided it is not actively excluded. However, including an express clause provides clarity and avoids litigation over whether the default rule applies.

### Recommended Clause (Simplified)

A single paragraph covering:

1. **Definition**: Events beyond reasonable control, including but not limited to natural disasters, war, pandemic, government action, and fundamental regulatory changes that make performance impossible (not merely more difficult or expensive).
2. **Notification**: The affected party must notify the other party promptly and mitigate where possible.
3. **Suspension, not termination**: Obligations are suspended for the duration of the force majeure event, up to a maximum of **6 months**.
4. **Termination right**: If the force majeure event continues for more than 6 months, either party may terminate the agreement.

**What NOT to include:** Detailed enumeration of every conceivable event. Financial hardship. Changes in market conditions. Inability to hire staff. These are business risks, not force majeure.

**Regulatory change note:** A change in EU MDR requirements or AI Act obligations that fundamentally alters the viability of the co-development could qualify as force majeure if it makes performance legally impossible. A change that merely makes it more expensive or requires adjustment does not. This distinction should be implicit in the "impossible, not merely difficult" formulation.

---

## 10. Dispute Resolution

### Options Analysis

| Option | Pros | Cons | Cost |
|--------|------|------|------|
| **Danish courts** | Familiar, enforceable, precedent-based | Slow (12-24 months), public, unpredictable costs | Moderate |
| **Arbitration (DIA)** | Confidential, expert arbitrators, faster | High minimum cost, formal, less accessible for startup | High |
| **Mediation-first + arbitration** | Preserves relationship, cheaper initial step, confidential | Adds a step, may delay resolution if mediation fails | Low initial, high if escalates |
| **Mediation-first + courts** | Best of both worlds for domestic dispute | Courts are public if mediation fails | Low initial, moderate if escalates |

### Recommended: Mediation-First Escalation

For a cooperation between two Danish companies that want to preserve their relationship:

**Step 1: Good-faith negotiation** (30 days). Senior representatives of each party attempt to resolve the dispute directly.

**Step 2: Mediation** through the Danish Institute of Arbitration (Voldgiftsinstituttet). This is confidential, relatively inexpensive, and the DIA has explicit expertise in business-to-business disputes of all sizes.

**Step 3: If mediation fails within 60 days**, the dispute is resolved by the ordinary Danish courts (Copenhagen City Court as first instance).

**Why not arbitration as the final step?** Arbitration costs can be disproportionate for a startup. The DIA's simplified arbitration procedure helps, but for a cooperation agreement with a EUR 50,000-100,000 liability cap, full arbitration proceedings could cost more than the dispute is worth. Danish courts are competent, and since both parties are Danish, there is no enforcement concern.

**Governing law:** Danish law. Both parties are Danish-connected, the cooperation is performed in Denmark, and the data is processed in Denmark. There is no reason to choose any other governing law.

---

## 11. Proportionate Protection for Different-Sized Parties

### Structural Asymmetries That Protect Both Parties

The agreement should acknowledge the size difference without being patronizing about it. Several structural features naturally create proportionate protection:

**Insurance requirement** (Section 6): Requires Regla to carry professional indemnity insurance, which gives OptoCeutics confidence that Regla's obligations are backed by real coverage. Does not require Regla to carry insurance disproportionate to its size.

**Liability cap structure** (Section 1): The absolute cap is set at a level that is meaningful to both parties. EUR 50,000 hurts a startup and is noticeable to a medium company. This is more proportionate than a percentage-of-revenue cap, which would produce radically different numbers.

**Termination consequences** (Section 8): The perpetual license survives termination, which protects OptoCeutics' investment. The data deletion obligation protects OptoCeutics' trade secrets. The derived knowledge retention protects Regla's development investment.

**Dispute resolution** (Section 10): Mediation-first protects Regla from being overwhelmed by litigation costs. Court resolution (rather than arbitration) as the final step keeps costs proportionate.

### Asymmetric Obligations That Make Sense

- **Regla has higher data security obligations** -- because Regla is handling OptoCeutics' data, not the reverse.
- **OptoCeutics has higher data accuracy obligations** -- because OptoCeutics is providing the data Regla relies on.
- **Regla has a platform maintenance obligation during the cooperation** -- because the platform is Regla's contribution.
- **OptoCeutics has a data access obligation during the cooperation** -- because data access is OptoCeutics' contribution.

These asymmetries are not about party size; they are about party role. This is the right way to create different obligations -- based on what each party actually does, not on how many employees they have.

---

## 12. Creative Minimalism: The Four-Clause Architecture

### Philosophy

The best cooperation agreements in the tech industry follow a pattern: instead of trying to anticipate every possible scenario (which produces 40-page liability sections), they establish clear **principles** and **mechanisms** that can handle any scenario. The goal is to create a self-adjusting framework, not a comprehensive encyclopedia.

### The Proposed Four-Clause Architecture for Mutual Protection

**Clause 1: Liability Framework** (covers Sections 1, 2, and 5 above)
One clause that establishes: (a) the general liability cap, (b) the enhanced cap for data-related breaches, (c) exclusion of consequential damages as default with targeted inclusion for confidentiality and IP breaches, (d) the carve-outs for fraud, gross negligence, confidentiality breach, and IP breach. Everything in one place, internally consistent, about 150-200 words.

**Clause 2: Mutual Indemnification** (covers Sections 3 and 4 above)
One clause that establishes: (a) what each party indemnifies the other for (two items each), (b) indemnification procedure (three conditions), (c) indemnification cap (enhanced cap applies), (d) key warranties from each party. Approximately 200-250 words.

**Clause 3: Termination** (covers Sections 7 and 8 above)
One clause that establishes: (a) for-cause termination triggers, (b) for-convenience termination with notice periods, (c) minimum term, (d) what survives termination (license, NDA, IP, indemnification), (e) data return/deletion obligations and the AI training carve-out. Approximately 250-300 words.

**Clause 4: Dispute Resolution** (covers Sections 9 and 10 above)
One clause that establishes: (a) governing law, (b) good-faith negotiation, (c) mediation through DIA, (d) Danish courts as final forum, (e) force majeure (integrated as a sub-clause). Approximately 150-200 words.

**Total: approximately 750-950 words for the entire mutual protection section.** This is achievable and sufficient.

### What Makes This Work

- **Internal references instead of repetition.** The liability cap is defined once and referenced everywhere.
- **Principles over scenarios.** "Reasonable professional care" covers more ground than a 20-item list of specific performance standards.
- **Role-based obligations.** Each party's obligations flow from their role (technology developer vs. data provider), creating a natural and intuitive structure.
- **Escalation mechanisms over rigid rules.** The dispute resolution escalation (negotiate, mediate, litigate) handles everything from minor disagreements to fundamental disputes without needing separate procedures for each.

---

## Key Recommendations Summary

| Area | Recommendation | Rationale |
|------|---------------|-----------|
| **Liability cap** | EUR 50,000 general / EUR 100,000 data-related | Proportionate to cooperation value; meaningful to both parties |
| **Consequential damages** | Exclude generally; include for confidentiality + IP breaches | Targets real harm without open-ended exposure |
| **Indemnification** | Mutual, 2 items each, subject to enhanced cap | Covers realistic third-party claim scenarios only |
| **Warranties** | 4 per party, role-specific | Narrow but meaningful; each warranty is actionable |
| **Carve-outs** | Fraud, gross negligence, confidentiality breach, IP breach | Danish law defaults + agreement-critical behaviors |
| **Insurance** | PI + cyber (EUR 250K each) for Regla; general liability for OptoCeutics | Backstops the liability cap affordably |
| **Termination** | 12-month minimum, 90-day notice, for-cause triggers | Protects investment while allowing exit |
| **Post-termination** | License survives; raw data deleted; derived knowledge retained if anonymized | Balances both parties' legitimate interests |
| **Force majeure** | Single paragraph, suspension up to 6 months | Simple, sufficient, consistent with Danish law |
| **Dispute resolution** | Mediation-first through DIA, then Danish courts | Cost-proportionate, relationship-preserving |
| **Architecture** | 4 clauses, ~750-950 words total | Maximum protection, minimum complexity |

---

## References and Sources

- Danish Contracts Act (Aftalelov), particularly Section 36 (unfair terms)
- Chambers and Partners, Commercial Contracts 2025 - Denmark
- Lexology, "Limiting contractual liability in Denmark"
- Danish Institute of Arbitration (Voldgiftsinstituttet), Rules of Mediation and Simplified Arbitration
- American Bar Association, "SaaS Agreements: Key Contractual Provisions"
- Morgan Lewis, "Key Concepts in AI Contracting: Data Rights and Restrictions" (2025)
- Mazanti, "Force Majeure under Danish Law"
- Gorrissen Federspiel, "Force Majeure: Implications for Commercial Contracts"

---

*This report was produced as part of the parallel research phase for the OptoCeutics Cooperation Agreement project. It is intended for synthesis with the other four research streams (Danish cooperation law, NDA best practices, IP ownership, QMS data access/GDPR) to inform the agreement drafting phase.*
