# Red Team Review: Consultancy Agreement v03

**Date:** 2026-02-26
**Reviewer:** Independent Legal Review Agent
**Client:** Regla ApS
**Subject:** Consultancy Agreement between Regla ApS and OptoCeutics A/S (draft v03)
**Classification:** Pre-meeting strategic review -- time-sensitive

---

## 1. Executive Summary

The v03 agreement is a well-crafted, intentionally minimal consultancy contract. It achieves its design goal: a document that looks like a standard Danish konsulentaftale, is short enough that Marcus can sign without triggering internal legal review at OptoCeutics, and that reinforces Regla's IP position. The consultancy framing is the correct strategic choice under Danish copyright law.

However, the agreement's simplicity creates specific vulnerabilities. This review identifies **4 critical gaps, 5 significant risks, and 6 areas where the agreement is adequate or strong**. The critical gaps are areas where silence in the contract produces outcomes that harm Regla under Danish default law. The significant risks are areas where the agreement's current language is functional but could be exploited or misinterpreted in an adversarial scenario.

**Overall assessment:** The agreement is approximately 80% of where it needs to be. The remaining 20% can be addressed with targeted additions of approximately 3-5 sentences total, preserving the ~1.5 page format.

---

## 2. Methodology

This review was conducted from five adversarial perspectives:

1. **OptoCeutics' aggressive future counsel** -- How would a hostile lawyer exploit ambiguities on behalf of OptoCeutics?
2. **OptoCeutics' acquirer** -- What happens if a competitor of Regla acquires OptoCeutics?
3. **Regla's insolvency administrator** -- What survives if Regla goes bankrupt?
4. **A Danish court applying substance-over-form** -- Would a court look through the consultancy label?
5. **SKAT (Danish tax authority)** -- VAT and transfer pricing implications.

Each clause was tested against these five perspectives.

---

## 3. What the Agreement Gets Right

Before identifying problems, it is important to acknowledge what works well. These are areas where no changes are recommended.

### 3.1 Consultancy Framing (Strong)

The consultancy framing is legally sound. Under the Danish Copyright Act, a consultant retains copyright in their work by default. The agreement reinforces this default rather than deviating from it. The language in Section 1.1 ("independent contractor," "independently and at its own discretion") correctly establishes the consultancy relationship. This is the single most important structural decision in the agreement, and it is correct.

### 3.2 IP Ownership Clause (Strong)

Section 2.1 is clean and absolute: Regla owns all IP in the Platform, including improvements developed "during or as a result of this engagement." The phrase "as a result of" is important -- it captures IP that arises from feedback, co-working sessions, or insights gained through the engagement, not just work performed during formal consulting hours. This is well-drafted.

### 3.3 Liability Cap with Carve-Outs (Adequate)

Section 4 follows the recommendation from the liability research: EUR 50,000 general cap, indirect/consequential loss exclusion, carve-outs for gross negligence, wilful misconduct, and confidentiality breaches. This is proportionate for a zero-fee consultancy between a startup and a medium-sized company. The confidentiality carve-out appropriately gives teeth to the NDA.

### 3.4 Termination with Survival (Adequate)

Section 5.3 correctly states that Sections 2 (IP), 3 (Confidentiality), and 4 (Liability) survive termination. This is the minimum necessary survival set.

### 3.5 Governing Law and Jurisdiction (Strong)

Danish law, Copenhagen City Court. Both parties are Danish. No reason for any other choice. Courts over arbitration is correct for the size of the parties.

### 3.6 No-Cash Compensation Acknowledgment (Adequate)

Section 1.3 explicitly states no cash payment and that each party bears its own costs. This avoids ambiguity about fee expectations and is consistent with the design principle of transparency about the deal structure.

---

## 4. Critical Gaps

These are issues where the agreement's silence produces outcomes harmful to Regla under Danish default law, or where a missing provision creates an exploitable vulnerability.

### 4.1 CRITICAL: Source Code License Survives Termination -- But With What Scope?

**The problem:** Section 2.2 grants OptoCeutics a license to use Platform source code for internal purposes and in their own products. Section 5.3 says Section 2 survives termination. This means the source code license survives indefinitely.

**The gap:** The license as currently drafted grants access to source code for use "in OptoCeutics' own products and services." This license survives termination. But the agreement does not define:

- **Which version of the source code is licensed post-termination.** Does OptoCeutics get the source code as it existed at termination, or does Regla have an ongoing obligation to provide updated source code indefinitely? The silence is ambiguous.
- **Whether OptoCeutics can modify the source code.** The license says they can "use" it. Under Danish copyright law, "use" of source code arguably includes the right to make necessary modifications for the permitted purpose (internal use and own products). But can they create derivative works? The agreement is silent.
- **How "in OptoCeutics' own products and services" interacts with an acquisition.** If OptoCeutics is acquired by a competitor of Regla, the acquirer's products become "OptoCeutics' own products" by operation of corporate merger. The source code license would extend to the acquirer's product line.

**Adversarial scenario:** OptoCeutics is acquired by a large compliance software company. That company argues that all its products are now "OptoCeutics' own products" and uses Regla's source code across its entire product portfolio. The license has no change-of-control provision limiting this.

**Recommendation:** Add one sentence to Section 2.2: "The license granted in this Section 2.2 covers the Platform source code as made available to OptoCeutics during the term of this Agreement. In the event of a change of control of OptoCeutics, the license shall not extend beyond the scope of OptoCeutics' business as conducted at the time of the change of control."

**Severity:** CRITICAL -- This is an existential risk if OptoCeutics is acquired by a competitor.

### 4.2 CRITICAL: No Definition of "Platform"

**The problem:** The Background section describes the Platform in general terms ("AI-powered electronic Quality Management System... incorporating automated documentation generation, clinical and regulatory data analysis, and regulatory strategy support"). This description is both broad and vague.

**The gap:** OptoCeutics has its own internal platform that performs some automated compliance functions. The README explicitly warns about this overlap. If a dispute arises about whether specific functionality falls within Regla's Platform or OptoCeutics' own independent development, the current definition provides no clear boundary.

**Adversarial scenario:** Regla develops a novel regulatory pathway analysis feature. OptoCeutics independently develops a similar feature for its own internal use. Regla claims OptoCeutics copied from the Platform source code. OptoCeutics claims it was their own independent development, entirely outside the Platform scope. Without a precise Platform definition, both arguments have merit.

**The deeper problem:** The broad Platform definition could be read as claiming IP ownership over functionality that OptoCeutics developed independently. Section 2.1 says Regla owns all IP "in the Platform, including any improvements, features, or functionality developed during or as a result of this engagement." If "the Platform" encompasses all regulatory AI functionality, this clause sweeps very broadly.

**Recommendation:** This is difficult to fix without adding complexity. The minimum viable fix is to add a sentence to the Background clarifying that "the Platform" refers specifically to Regla's proprietary codebase and does not include tools, software, or processes independently developed by OptoCeutics. Something like: "For the avoidance of doubt, the Platform does not include any software, tools, or processes independently developed by OptoCeutics."

**Severity:** CRITICAL -- Without this, the IP clause creates a potential claim over OptoCeutics' own independent development, which would be both unfair and likely unenforceable, but would still create expensive litigation risk.

### 4.3 CRITICAL: No Data Ownership / Return Provision

**The problem:** The agreement grants Regla access to OptoCeutics' QMS environment (implied by the consultancy scope -- Regla needs QMS data to provide consulting services). But the agreement says nothing about:

- Who owns the data Regla accesses
- What Regla can do with insights derived from the data
- What happens to the data upon termination
- Whether Regla must return or destroy OptoCeutics' data after the engagement ends

**Why this matters for Regla:** Without an explicit data ownership clause, the default under Danish law is that OptoCeutics retains ownership of its data (which is correct and desired). But the lack of any provision about derived insights creates risk for Regla. If Regla uses generalized patterns learned from OptoCeutics' QMS to improve its platform for other customers, OptoCeutics could argue that this use exceeds what the consultancy authorized, particularly after termination.

**Why this matters for OptoCeutics:** OptoCeutics has no contractual assurance that Regla will delete their QMS data after the engagement ends. The confidentiality clause (Section 3) protects against disclosure but does not mandate deletion.

**Adversarial scenario:** The engagement terminates. OptoCeutics demands Regla delete all copies of QMS data. Regla has trained AI models on this data. The agreement says nothing about whether model weights containing patterns from OptoCeutics' data constitute "copies" that must be deleted. Litigation ensues.

**Recommendation:** Add one sentence acknowledging that OptoCeutics retains ownership of its QMS data and that upon termination, Regla shall return or destroy copies of OptoCeutics' data in its original form. This is a standard provision in consultancy agreements and would not raise eyebrows. Example: "OptoCeutics retains all rights in its QMS data. Upon termination, Regla shall, at OptoCeutics' request, return or destroy all copies of OptoCeutics' confidential data in its original form and confirm such return or destruction in writing."

**Severity:** CRITICAL -- Both parties are exposed. This is the most likely source of a post-termination dispute.

### 4.4 CRITICAL: "Competes with the Platform" is Undefined

**The problem:** Section 2.2 prohibits OptoCeutics from using the source code to "develop, market, or offer to third parties any product or service that competes with the Platform." The term "competes with the Platform" is not defined.

**The gap:** What constitutes a competing product? OptoCeutics already has its own internal compliance automation. If OptoCeutics uses its own technology (not Regla's source code) to build a product that happens to have overlapping functionality with Regla's Platform, is that "competing"? If OptoCeutics licenses its own separately-developed QMS tools to a third party, and those tools overlap with some Platform features, has OptoCeutics violated the restriction?

**The core issue:** The restriction is meant to be IP-based (do not use our code to build a competitor), not market-based (do not compete with us at all). But the language "any product or service that competes with the Platform" reads as market-based when applied to independently developed OptoCeutics technology.

**Adversarial scenario:** OptoCeutics uses its own independently developed technology to offer QMS automation to a third party. Regla argues this "competes with the Platform" and demands OptoCeutics stop. OptoCeutics argues they never used Regla's source code for this product. The dispute hinges on the undefined term "competes."

**Recommendation:** Clarify that the restriction applies specifically to use of the source code, not to OptoCeutics' independent business activities. The restriction already says "use the source code to develop, market, or offer" -- but the phrase "that competes with the Platform" could be read as a standalone condition. Tightening the language would help. Example revision: "...nor use the source code, in whole or in part, in the development of any product or service offered to third parties that replicates or is substantially based on the Platform's functionality."

**Severity:** CRITICAL -- The current language could be misread as a blanket non-compete on OptoCeutics' business, which would be disproportionate, likely unenforceable under Danish law, and damaging to the relationship if raised.

---

## 5. Significant Risks

These are issues where the agreement functions but creates vulnerabilities that could be exploited or that produce unintended consequences in specific scenarios.

### 5.1 Recharacterization Risk: Consultancy vs. Co-Development

**The risk:** Danish courts apply a substance-over-form principle (realitetsgrundsaetning). If the operational reality looks like co-development (joint decision-making on features, shared roadmap, OptoCeutics engineers contributing to the Platform), a court could recharacterize the agreement as a cooperation, potentially implying joint IP ownership.

**Current mitigation in the agreement:** The consultancy language is correct. Section 1.1 establishes independence. Section 1.2 avoids mutual commitments.

**Gap in mitigation:** The agreement does not address operational conduct. If Regla and OptoCeutics operate like co-development partners in practice (which is the likely reality), the contractual language will be tested.

**Recommendation:** This cannot be fully fixed in the contract. Regla should maintain operational discipline: Regla decides what to build, OptoCeutics provides feedback as a client. Do not create joint Jira boards, shared product roadmaps, or co-authored design documents. The README already notes this concern. The operational implementation is more important than any contract clause.

**Severity:** MEDIUM -- Low probability (would require a dispute), but high impact if realized (joint IP ownership claim).

### 5.2 Three-Year Confidentiality Survival May Be Too Short

**The risk:** Section 3.3 states confidentiality obligations survive for three years post-termination. Source code remains valuable long after three years. Trade secrets have no expiration date under the Danish Trade Secrets Act.

**The concern:** After three years, OptoCeutics would no longer have a contractual obligation to keep Regla's source code confidential. While the Trade Secrets Act provides independent statutory protection (as long as the code qualifies as a trade secret), the contractual protection is more certain and easier to enforce.

**Comparison:** The research recommended a dual-track approach: 5 years for general confidential information, perpetual for trade secrets. The agreement uses a flat 3 years for everything.

**Recommendation:** Consider extending to 5 years, or adding a sentence specifying that obligations regarding trade secrets (specifically the source code) survive for as long as they qualify as trade secrets under applicable law. This is standard language and would not add significant complexity.

**Severity:** MEDIUM -- The statutory trade secret protection provides a backstop, but the shorter contractual term weakens enforceability.

### 5.3 No Warranty Disclaimer

**The risk:** The agreement is silent on warranties. Under Danish law, this means the default implied warranties apply. In a consultancy context, this includes an implied duty to perform services with reasonable professional care and skill (the culpa norm). But it could also be read as implying that the Platform is fit for OptoCeutics' purposes.

**The concern:** If OptoCeutics relies on Platform-generated documentation for regulatory submissions and the documentation contains errors, OptoCeutics could argue that Regla breached an implied warranty of fitness. The liability cap (Section 4) limits exposure, but the confidentiality carve-out could be invoked if the error involved confidential data.

**Recommendation:** Add a brief disclaimer to Section 1 or Section 4: "The Platform and services are provided 'as is.' Regla does not warrant that the Platform will be error-free or suitable for any specific regulatory purpose. OptoCeutics is responsible for reviewing and validating all output before use." This is standard in technology consultancy agreements and protects Regla from implied fitness claims.

**Severity:** MEDIUM -- The liability cap provides protection, but a warranty disclaimer would close this gap cleanly.

### 5.4 Sublicensing to OptoCeutics' Subsidiaries/Affiliates

**The risk:** Section 2.2 says the license is "non-transferable" and prohibits sublicensing. But it does not address whether OptoCeutics' subsidiaries or affiliates can use the source code.

**The concern:** If OptoCeutics has (or creates) subsidiaries, those entities are legally separate from OptoCeutics A/S. Under the current license, only OptoCeutics A/S is authorized to use the source code. A subsidiary using it would technically violate the license. Alternatively, OptoCeutics could argue that "internal purposes" includes intra-group use.

**Recommendation:** Low priority. This is standard license ambiguity that can be addressed if it becomes relevant. If OptoCeutics raises it, the simplest answer is: "The license is to OptoCeutics A/S. Subsidiaries would need separate authorization."

**Severity:** LOW-MEDIUM -- Unlikely to be an issue in the near term given OptoCeutics' current structure.

### 5.5 No Force Majeure

**The risk:** The agreement is silent on force majeure. Under Danish law, force majeure can be invoked as a defense to non-performance even without a contract clause, so the practical risk is low. However, silence means the threshold and consequences are determined by courts rather than by the parties.

**Recommendation:** Given the design principle of simplicity, omitting force majeure is defensible. Danish default law provides adequate protection. No change recommended unless OptoCeutics raises it.

**Severity:** LOW -- Danish default law covers this adequately.

---

## 6. Clause-by-Clause Analysis

### Background Section

| Element | Assessment | Notes |
|---------|-----------|-------|
| Regla description | Adequate | Correctly identifies Platform scope |
| OptoCeutics description | Adequate | Correctly frames as client engaging consultant |
| Consultancy framing | Strong | Language supports the intended characterization |
| Platform definition | **Weak** | See Critical Gap 4.2 -- too broad, no exclusion for OptoCeutics' own tools |

### Section 1: Services

| Clause | Assessment | Notes |
|--------|-----------|-------|
| 1.1 Independent contractor | Strong | Correct language for consultancy framing |
| 1.2 Flexible scope | Adequate | Avoids mutual commitments, supports consultancy framing |
| 1.3 No cash payment | Adequate | Transparent, satisfies reciprocity expectation |

### Section 2: Intellectual Property

| Clause | Assessment | Notes |
|--------|-----------|-------|
| 2.1 Regla owns all Platform IP | Strong | Clean, absolute, correct scope |
| 2.2 Source code license | **Needs work** | See Critical Gaps 4.1 and 4.4 -- scope post-termination unclear, "competes" undefined, no change-of-control provision |

### Section 3: Confidentiality

| Clause | Assessment | Notes |
|--------|-----------|-------|
| 3.1 Mutual obligation | Adequate | Broad definition with specific examples |
| 3.2 Standard exclusions | Strong | All four standard exclusions present |
| 3.3 Three-year survival | **Needs consideration** | See Significant Risk 5.2 -- may be too short for trade secrets |

### Section 4: Liability

| Clause | Assessment | Notes |
|--------|-----------|-------|
| 4.1 Indirect loss exclusion | Strong | Standard, well-drafted |
| 4.2 EUR 50,000 cap with carve-outs | Adequate | Proportionate, correct carve-outs |

### Section 5: Term and Termination

| Clause | Assessment | Notes |
|--------|-----------|-------|
| 5.1 Indefinite term, 3-month notice | Adequate | Standard consultancy terms |
| 5.2 Material breach termination | Strong | 30-day cure period, insolvency trigger |
| 5.3 Survival clause | Adequate | Correct sections survive (2, 3, 4) |

### Section 6: General

| Clause | Assessment | Notes |
|--------|-----------|-------|
| 6.1 Danish law, Copenhagen courts | Strong | Correct for two Danish parties |
| 6.2 Written amendments, entire agreement | Strong | Standard, well-drafted |

---

## 7. Adversarial Perspective Testing

### 7.1 OptoCeutics' Aggressive Future Counsel

If the relationship deteriorates and OptoCeutics hires aggressive counsel, the most likely attack vectors are:

1. **Claim joint IP ownership based on co-development substance.** Argue that the consultancy label is a fiction and that OptoCeutics' contributions (QMS data, domain expertise, feedback) give rise to joint ownership under Danish copyright law.
   - **Defense strength:** MEDIUM. The consultancy framing is the legal default, but substance-over-form is a real doctrine.

2. **Argue the source code license is broader than intended.** Push the boundaries of "internal purposes" and "own products and services" to cover activities Regla did not contemplate.
   - **Defense strength:** WEAK without the recommended clarifications.

3. **Challenge the non-compete as an unenforceable restraint of trade.** Argue that "competes with the Platform" is so vague as to be a blanket non-compete, which is disproportionate under Danish law.
   - **Defense strength:** WEAK. The current language is genuinely ambiguous.

### 7.2 OptoCeutics' Acquirer

If OptoCeutics is acquired by a Regla competitor:

1. **Source code access flows to the acquirer** through the non-transferable license (which transfers by operation of law in a share sale, since OptoCeutics A/S continues to exist as an entity).
2. **The "own products" scope expands** to include the acquirer's product portfolio.
3. **The non-compete restriction becomes harder to enforce** because the acquirer may already compete with Regla independently.

**This is the most dangerous scenario the agreement fails to address.**

### 7.3 Regla's Insolvency Administrator

If Regla goes bankrupt:

1. **The source code license is a surviving obligation** (Section 5.3 makes Section 2 survive).
2. **An insolvency administrator may argue the license is an executory contract** that can be rejected under Danish insolvency law.
3. **Without source code escrow, OptoCeutics loses access** if Regla ceases to exist.

**Risk level:** Low probability, but the agreement provides no protection for OptoCeutics in this scenario. This could become a negotiation point if OptoCeutics raises concerns about Regla's startup status.

### 7.4 A Danish Court Applying Substance-Over-Form

A Danish court would consider:

1. **Does Regla actually operate independently?** If yes, the consultancy framing holds.
2. **Does OptoCeutics have any decision-making authority over the Platform?** If yes, co-development argument strengthens.
3. **Is the "no cash" arrangement genuinely a consultancy, or is it barter?** The court may view it as a barter arrangement regardless of the label.
4. **Does the agreement as a whole reflect a consultancy or a partnership?** The absence of client obligations (what OptoCeutics must provide) actually supports the consultancy framing -- it looks like Regla serves OptoCeutics, not the other way around.

**Assessment:** The agreement would likely survive a substance-over-form challenge if Regla maintains operational independence. The risk is in the operational reality, not the contract language.

### 7.5 SKAT (Tax Authority)

1. **Barter VAT risk:** SKAT may treat the arrangement as a barter -- Regla provides consulting services, OptoCeutics provides QMS access. Both supplies could be subject to 25% VAT on their market value. Net effect is zero if both parties are VAT-registered (they likely are), but failure to report is a compliance risk.
2. **The consultancy framing does not avoid the VAT issue.** The framing affects IP treatment but not VAT treatment.
3. **Mitigation in the agreement:** Section 1.3 describes the arrangement as "without separate cash payment" and "each Party bears its own costs." This is helpful but does not eliminate the barter characterization.

**Recommendation:** This is a tax advice issue, not a contract drafting issue. Both parties should consult their accountants about VAT treatment. No contract changes needed, but Regla should be aware of the exposure.

---

## 8. Priority-Ranked Recommendations

### Must-Do Before Meeting (4 items, ~3-5 sentences of additional text)

| Priority | Issue | Fix | Impact on Length |
|----------|-------|-----|-----------------|
| 1 | Change-of-control on source code license (4.1) | Add one sentence to Section 2.2 | +1 sentence |
| 2 | "Competes with the Platform" clarification (4.4) | Revise existing language in Section 2.2 | Net zero (revision, not addition) |
| 3 | Platform definition exclusion (4.2) | Add one sentence to Background | +1 sentence |
| 4 | Data return/destruction (4.3) | Add one sentence to Section 5 (termination consequences) | +1 sentence |

### Should-Do If Space Permits (2 items)

| Priority | Issue | Fix | Impact on Length |
|----------|-------|-----|-----------------|
| 5 | Warranty disclaimer (5.3) | Add one sentence to Section 1 or Section 4 | +1 sentence |
| 6 | Trade secret survival duration (5.2) | Modify Section 3.3 to add trade secret perpetual carve-out | +1 clause |

### Do Not Do (complexity not worth the protection)

- Indemnification provisions
- Insurance requirements
- Force majeure clause
- Detailed data handling framework
- AI-specific source code restrictions
- Audit rights
- Background IP schedules

These would individually be valuable, but collectively they would transform the agreement from ~1.5 pages to ~4 pages, violating the core design principle. The items in the "Must-Do" list achieve approximately 80% of the protective value for 10% of the added complexity.

---

## 9. Specific Redline Suggestions

### Section 2.2 (Revised)

**Current:**
> Regla grants OptoCeutics a non-exclusive, non-transferable license to use the Platform source code for OptoCeutics' own internal purposes and in OptoCeutics' own products and services. OptoCeutics shall not distribute, sublicense, or otherwise make the source code available to third parties, nor use the source code to develop, market, or offer to third parties any product or service that competes with the Platform.

**Proposed:**
> Regla grants OptoCeutics a non-exclusive, non-transferable license to use the Platform source code **as provided during the term of this Agreement** for OptoCeutics' own internal purposes and in OptoCeutics' own products and services. OptoCeutics shall not distribute, sublicense, or otherwise make the source code available to third parties, nor use the source code**, in whole or in part, in the development of** any product or service **offered to third parties that replicates the Platform's core functionality**. **In the event of a change of control of OptoCeutics, the license shall not extend beyond the scope of OptoCeutics' business as conducted at the time of the change of control.**

### Background Section (Addition)

Add after the Platform description:
> **For the avoidance of doubt, the Platform does not include any software, tools, or processes independently developed by OptoCeutics.**

### Section 5.3 (Addition)

After the current survival clause, add:
> **Upon termination, Regla shall, at OptoCeutics' request, return or destroy all copies of OptoCeutics' confidential data in its original form and confirm such action in writing.**

---

## 10. Overall Risk Assessment

| Risk Category | Count | Aggregate Severity |
|---------------|-------|--------------------|
| Critical gaps | 4 | HIGH -- any could produce adverse outcomes in a dispute |
| Significant risks | 5 | MEDIUM -- manageable, mostly covered by Danish default law |
| Agreement strengths | 6 | Agreement is fundamentally sound |

**Bottom line for today's meeting:** The agreement is good but not ready for signature. The four critical gaps should be addressed before signing. The fixes are minimal -- approximately 3-5 additional sentences -- and preserve the agreement's intentional simplicity. If OptoCeutics wants to sign today, at minimum the change-of-control provision and the "competes with" clarification must be included. The data return provision and Platform definition exclusion can be added in a follow-up revision if necessary, but should be raised in the meeting.

---

*This review was prepared for Regla ApS. It identifies risks from both parties' perspectives but is written to serve Regla's strategic interests. It does not constitute legal advice. Final agreement should be reviewed by qualified Danish counsel before execution.*
