# Liability Limitations in Danish Cooperation Agreements

## Research Report for Regla ApS / OptoCeutics A/S Cooperation Agreement

**Date:** 2026-02-25
**Prepared for:** Emil Timmreck Pedersen, CEO, Regla ApS
**Subject:** Whether the cooperation agreement draft (v01) needs a liability limitation clause
**Governing Law:** Danish law (Aftaleloven, Erstatningsansvarsloven, general Danish contract law)

---

## 1. Executive Summary

The cooperation agreement draft is currently silent on liability. This research examines what Danish law implies in that silence, what the realistic risks are, and whether adding a liability clause would improve or complicate the agreement.

**Bottom-line recommendation:** Add a minimal liability clause (Option B or C). The Danish default rules create an open-ended liability exposure that is disproportionate to this no-money, good-faith cooperation. A two-to-three sentence clause eliminates ambiguity without undermining the agreement's lightweight spirit. This is not about distrust -- it is about preventing the one scenario where silence could hurt both parties.

---

## 2. Danish Legal Framework: What Happens When the Agreement is Silent

### 2.1 The Culpa Norm (Fault-Based Liability)

Under Danish law, the foundational liability principle is **culpa** (fault-based liability). The Chambers Commercial Contracts 2025 guide for Denmark states that "the general basis of liability is the culpa rule, which is the principal rule both within and outside contractual relationships." This means:

- A party is liable for harm caused **intentionally or negligently** (all forms of negligence)
- Three elements must be proven: (1) loss occurred, (2) negligent or intentional act, and (3) causal connection between the act and the loss
- When contracts lack explicit liability terms, courts apply an implied duty standard, including implied duties of honesty, disclosure, and care

**For this agreement:** If Regla negligently handles OptoCeutics' QMS data (e.g., a data leak through a misconfigured system), or if OptoCeutics' feedback leads Regla to build something that causes harm to a third party, the default culpa norm applies with no contractual cap or limitation.

### 2.2 No Statutory Cap on Liability

Danish law does not prescribe a general, statutory limitation on liability for specific categories of losses. Unlike some jurisdictions, there is no automatic cap. In principle, recoverable losses may include:

- **Direct losses** (direkte tab): Immediate, tangible costs flowing from the breach
- **Indirect/consequential losses** (indirekte tab): Including loss of profit, lost business opportunities, reputational harm

The Danish Sale of Goods Act (Kobeloven) distinguishes between direct and indirect loss with stricter standards for recovering indirect loss, but this distinction applies most directly to sale-of-goods relationships. For a cooperation agreement, the distinction is less clear-cut, and courts would likely apply general culpa principles.

### 2.3 The Adequacy Requirement (Adaekvans)

Danish law requires that damages be **foreseeable** (adaekvat) -- the loss must be a reasonably foreseeable consequence of the breach. This provides some natural limitation, but it is a judicial assessment made after the fact, not a contractual certainty.

### 2.4 Duty to Mitigate (Tabsbegraeningsplikt)

The injured party has a duty to mitigate its losses. Failure to mitigate can reduce or eliminate a damages claim. This provides another natural check, but again, it operates after the fact.

### 2.5 Section 36 of the Danish Contracts Act (Aftaleloven)

Section 36 allows courts to modify or set aside contractual terms that are unreasonable or contrary to good faith. However, the Danish Supreme Court maintains a **highly restrictive approach** when applying Section 36 to commercial B2B contracts. The Supreme Court has reasoned that agreements between commercial parties "must be assumed to rest on a comprehensive balancing, which is the result of the parties' considerations regarding business risks and economic conditions." In practice, courts are very reluctant to intervene in freely negotiated commercial agreements.

**Implication:** If a future dispute arises, a court would not easily rewrite the agreement to add liability protections that the parties chose not to include. The silence would be interpreted as a deliberate choice by two commercial parties.

### 2.6 Freedom of Contract

The overriding principle of Danish contract law is **freedom of contract** (aftalefrihed). Parties are free to structure their agreements as they choose, including deciding what to include or exclude. Importantly, exclusion and limitation clauses are generally valid, with two exceptions:

1. **Gross negligence (grov uagtsomhed) and intent (forsaet):** Liability for these cannot be excluded
2. **Personal injury:** Liability for personal injury cannot be excluded

### 2.7 Loyalitetspligt (Duty of Loyalty)

Danish law recognizes an implied duty of loyalty between contracting parties. In commercial cooperation contexts, this manifests as:

- Both parties must act loyally and in good faith
- Each party must promote the cooperation's interests and make reasonable efforts
- Each party must notify the other of relevant circumstances
- The obligation is mutual -- it applies to both parties equally

This duty exists regardless of whether the agreement mentions it. It adds an implicit behavioral standard but does not, by itself, create or limit financial liability.

---

## 3. Specific Risks in This Cooperation

### 3.1 Risk Profile Analysis

The cooperation involves specific risk vectors that differ from a typical commercial contract:

| Risk Vector | Who Bears It | Severity | Probability |
|---|---|---|---|
| **Confidentiality breach of QMS data** | Regla (data recipient) | HIGH | Low-Medium |
| **Platform malfunction affecting OptoCeutics operations** | Regla (platform provider) | MEDIUM | Low |
| **Regla incorporates OptoCeutics IP into platform incorrectly** | Regla | MEDIUM | Low |
| **OptoCeutics provides incorrect/outdated QMS data** | OptoCeutics | LOW-MEDIUM | Low |
| **Platform generates incorrect regulatory documentation** | Regla | HIGH (regulatory) | Low |
| **Data protection breach (GDPR)** | Both parties | HIGH | Low |
| **Cooperation fails, wasted resources** | Both parties | LOW | Medium |

### 3.2 The Asymmetric Risk Problem

The risk profile is **asymmetric**:

- **Regla** bears most of the active risk (building software, handling data, potential platform failures)
- **OptoCeutics** bears most of the passive risk (sharing sensitive QMS data, depending on platform for operations)
- **Regla** is a 3-person startup with approximately 100K EUR/year budget
- **OptoCeutics** is a 50-person company with substantially larger operations

If OptoCeutics suffered a significant loss traceable to Regla's negligence (e.g., a QMS data breach that triggers regulatory action), the damages could theoretically exceed Regla's entire annual budget many times over. Under Danish default rules, there is no cap.

### 3.3 The Confidentiality Clause Is Not a Liability Clause

The agreement already has a robust confidentiality section (Section 5). However, Section 5 defines **obligations** (what each party must do with confidential information) but does not address **consequences** (what happens if those obligations are breached). The confidentiality clause creates the duty; liability rules determine the remedy. Without a liability clause, the remedy is unlimited under Danish default law.

---

## 4. Does the No-Money Nature of the Agreement Matter?

### 4.1 Danish Law Does Not Require Consideration

Unlike common law jurisdictions, Danish contract law does **not** recognize the concept of consideration. Contracts are formed on the basis of offer and acceptance. The absence of monetary payment does not affect the validity or enforceability of the agreement.

### 4.2 Barter/In-Kind Arrangements Under Danish Law

Danish law assesses contracts through fairness and reciprocity standards rather than formal consideration. The fact that this is a barter arrangement (QMS access for platform access) does not reduce liability exposure. Both parties have contractual obligations, and breach of those obligations carries the same liability consequences as in a paid contract.

### 4.3 Proportionality Argument

While Danish law does not formally reduce liability for non-monetary agreements, the **adaekvans** (foreseeability) and Section 36 (reasonableness) doctrines could provide some proportionality protection. A court might be less inclined to award massive damages in a no-money cooperation than in a high-value commercial contract. However, this is uncertain and would depend on the specific circumstances.

---

## 5. Analysis of Options

### Option A: Keep the Agreement As-Is (No Liability Clause)

**Description:** Rely entirely on Danish default rules. Trust the relationship and the culpa norm.

**Advantages:**
- Maximum simplicity -- no additional text
- Consistent with the "coffee-readable" design principle
- Does not introduce legal concepts that might feel adversarial
- Danish default rules provide reasonable baseline protections (fault-based liability, foreseeability, duty to mitigate)
- Both parties are Danish commercial entities who understand the legal environment

**Disadvantages:**
- **Unlimited liability exposure** for both parties (especially problematic for Regla as a startup)
- **Indirect/consequential damages** are recoverable by default -- a data breach at Regla could expose it to OptoCeutics' full consequential losses
- **Ambiguity about remedies** for confidentiality breaches (Section 5 creates duties but says nothing about consequences)
- Danish courts would treat the silence as a **deliberate choice** by two commercial parties, not an oversight
- Creates **asymmetric risk**: Regla has more to lose because its entire business is at stake, while OptoCeutics' loss exposure is bounded by the value of the cooperation
- If the relationship sours, the absence of a liability clause could escalate disputes
- **No protection against indirect damages** that could dwarf the value of the cooperation itself

### Option B: Add a Minimal One-Sentence Liability Limitation

**Proposed text:**
> "Neither Party shall be liable to the other for indirect or consequential losses arising from this cooperation, and each Party's total liability under this Agreement shall not exceed [EUR 50,000 / the direct losses actually incurred]."

**Advantages:**
- Adds one sentence -- barely changes the agreement's length or feel
- Eliminates the most dangerous default rule (unlimited indirect/consequential damages)
- Provides a clear cap that protects Regla as a startup
- Standard practice in Danish commercial agreements -- would not raise eyebrows
- Leaves direct damages fully recoverable (parties remain accountable)
- Can be explained in 30 seconds: "we exclude indirect losses, there's a reasonable cap on direct losses"

**Disadvantages:**
- Introduces a financial figure that requires negotiation (what cap amount?)
- One sentence may be too compressed to be completely clear
- A cap that is too low might be challenged under Section 36 (though this is very unlikely between commercial parties)

### Option C: Add a Short Liability Section (2-3 Sentences)

**Proposed text (new Section 8.7 or separate Section 9):**
> "**Limitation of Liability.** Neither Party shall be liable to the other for any indirect or consequential loss, including but not limited to loss of profit, loss of data, or loss of goodwill, arising from or in connection with this cooperation. Each Party's total aggregate liability under this Agreement shall not exceed EUR [50,000]. Nothing in this Agreement excludes or limits liability for gross negligence, wilful misconduct, or breach of the confidentiality obligations in Section 5."

**Advantages:**
- Clear and comprehensive without being heavy
- Explicitly excludes indirect/consequential losses (the primary risk)
- Provides a financial cap for total liability
- Carves out gross negligence and wilful misconduct (legally required anyway under Danish law, but making it explicit shows good faith)
- Carves out confidentiality breaches (protecting OptoCeutics' most important interest)
- Still fits on a single page section -- consistent with lightweight design
- Follows Danish commercial practice exactly

**Disadvantages:**
- Three sentences is slightly heavier than Option B
- The confidentiality carve-out means liability for data breaches remains uncapped (which may concern Regla)
- Requires agreeing on a cap figure
- Introduces more defined terms (indirect loss, consequential loss) that could need interpretation

### Option D: Add a More Detailed Liability Section

**Proposed text (5-8 sentences covering caps, exclusions, time limitations, and indemnification):**
A full liability section covering: (i) exclusion of indirect losses, (ii) aggregate financial cap, (iii) carve-outs for gross negligence and intent, (iv) carve-out for confidentiality and IP breaches, (v) time limitation for bringing claims, (vi) mutual indemnification for third-party claims, (vii) force majeure.

**Advantages:**
- Most comprehensive protection
- Covers edge cases (force majeure, third-party claims, time bars)
- Standard in formal commercial agreements

**Disadvantages:**
- **Fundamentally inconsistent with the agreement's design principle** -- this is supposed to be a coffee-readable cooperation agreement, not a SaaS contract
- Could signal that Regla anticipates problems or doesn't trust the relationship
- Overkill for a no-money cooperation between existing business partners
- Would double the length of Section 8 (General Provisions)
- May trigger OptoCeutics' legal team to review and redline the entire agreement, turning a simple sign-off into a negotiation

---

## 6. Red Team Analysis

### 6.1 Red Teaming "No Liability Clause" (Option A)

**Scenario 1: QMS Data Breach**
Regla suffers a cybersecurity incident. OptoCeutics' QMS documentation -- including proprietary processes, supplier information, and product specifications -- is exposed. OptoCeutics faces regulatory scrutiny from its Notified Body. The Notified Body suspends OptoCeutics' CE marking pending investigation. OptoCeutics loses 3 months of sales (EUR 2M+), must conduct emergency remediation (EUR 200K), and suffers reputational damage.

Under Danish default rules, OptoCeutics could claim all of these as damages: direct costs (remediation) plus indirect losses (lost sales, reputational harm). With no liability cap, Regla -- a 3-person startup with 100K EUR annual budget -- faces a claim that could bankrupt the company. The culpa norm requires fault, so Regla would need to have been negligent, but a misconfigured cloud server or an employee mistake easily qualifies.

**Scenario 2: Platform Generates Incorrect Documentation**
OptoCeutics relies on Regla's platform to generate risk analysis documentation. The platform produces documentation with a systematic error. OptoCeutics submits the documentation to its Notified Body without catching the error. The Notified Body flags the issue, requiring OptoCeutics to recall and redo all affected documentation (months of work, regulatory delays).

Who is liable? The agreement does not address this. Under culpa principles, was Regla negligent in building the platform feature? Was OptoCeutics negligent in not reviewing the output? Without a liability clause, this ambiguity gets resolved in court.

**Scenario 3: Relationship Deteriorates**
The cooperation works well for 18 months. Then Regla pivots, deprioritizes OptoCeutics' specific needs, and platform quality declines. OptoCeutics terminates under Section 7.3(a) (material breach). OptoCeutics claims damages for the period of declining service plus costs of transitioning to an alternative solution. Under default rules, these damages are potentially uncapped.

**Assessment:** The "no liability clause" approach exposes Regla to existential risk in low-probability but high-severity scenarios. The natural protections (culpa, foreseeability, mitigation duty) help but provide no certainty. For a 100K EUR/year startup, even a 200K EUR claim could be devastating.

### 6.2 Red Teaming "Add Liability Clause" (Options B/C)

**Concern 1: Signals Distrust**
Adding a liability clause could make OptoCeutics wonder: "Why is Regla thinking about liability? Are they worried about something? Is this riskier than we thought?" In a good-faith cooperation between existing business partners, introducing legal protections might feel like Regla is hedging against failure.

**Counter-argument:** Liability clauses are standard in Danish commercial agreements. Any experienced business person would expect one. Its absence is more unusual than its presence. OptoCeutics' own contracts with its suppliers almost certainly include liability limitations. Not including one signals inexperience, not trust.

**Concern 2: Creates Awareness of Risks That Don't Exist**
By mentioning "indirect losses" and "consequential damages," the clause could draw attention to catastrophic scenarios that neither party has considered. It could make the agreement feel heavier and more adversarial.

**Counter-argument:** The risks exist whether or not they are mentioned. A liability clause does not create risks -- it manages them. A short clause (Option B or C) is no more alarming than the existing confidentiality section (Section 5), which is already six subsections long.

**Concern 3: Opens Negotiation**
Introducing a liability clause could trigger OptoCeutics to involve its lawyers, leading to counter-proposals, redlines, and delays. This contradicts the "lightweight" design principle.

**Counter-argument:** This risk is real but manageable. If the clause is presented as a mutual protection (both parties benefit from the cap), it should be uncontroversial. Option B (one sentence) or Option C (three sentences) are short enough that they are unlikely to trigger a full legal review. If OptoCeutics does push back, the negotiation itself would be valuable -- it would surface any hidden concerns early.

**Concern 4: A Low Cap Could Backfire**
If the cap is set too low (e.g., EUR 10,000), it could be seen as Regla trying to avoid accountability. This could actually damage trust more than no clause at all.

**Counter-argument:** Set the cap at a meaningful but proportionate level. EUR 50,000 (half of Regla's annual budget) would demonstrate seriousness while providing protection. Alternatively, tie the cap to direct losses actually incurred, which is self-adjusting.

**Concern 5: Confidentiality Carve-Out Creates Complexity**
Option C includes a carve-out for confidentiality breaches, meaning liability for data breaches remains uncapped. This is fair to OptoCeutics but potentially dangerous for Regla.

**Counter-argument:** This is the trade-off. OptoCeutics is sharing its most sensitive data. If Regla negligently leaks it, OptoCeutics should have full recourse. Regla's protection is in the culpa requirement (OptoCeutics must prove negligence) and foreseeability limitation. If Regla wants to cap confidentiality liability too, it should negotiate that explicitly.

### 6.3 Red Team Synthesis

| Factor | No Liability Clause | Add Liability Clause |
|---|---|---|
| Worst-case scenario | Existential risk to Regla | Slightly heavier agreement |
| Relationship impact | Neutral (until a problem arises) | Minimal (standard commercial practice) |
| Practical likelihood of problem | Low | N/A (preventive measure) |
| Cost of being wrong | Potentially company-ending | Minor drafting effort |
| Reversibility | Cannot add after signing | Can always waive limitations later |

The asymmetry is clear: the downside of not having a clause (existential risk) vastly outweighs the downside of having one (slightly longer agreement).

---

## 7. Recommendation

### Primary Recommendation: Option C (Short Liability Section)

Add a short liability section with three sentences. This is the right balance between the agreement's lightweight design principle and prudent legal protection.

**Recommended text (add as Section 8.7 or new Section 9):**

> **Limitation of Liability.** Neither Party shall be liable to the other for any indirect or consequential loss, including loss of profit, loss of data (other than data subject to Section 5), or loss of goodwill, arising from or in connection with this Agreement. Each Party's total aggregate liability under this Agreement (excluding liability for breach of Section 5) shall not exceed EUR 50,000. Nothing in this Agreement excludes or limits either Party's liability for gross negligence or wilful misconduct.

**Why this text:**
1. **Excludes indirect/consequential losses** -- eliminates the most dangerous default exposure
2. **Provides a EUR 50,000 cap** -- meaningful but proportionate for a 100K EUR/year startup
3. **Carves out confidentiality** -- protects OptoCeutics' core interest (its QMS data)
4. **Carves out gross negligence/intent** -- legally required under Danish law, but explicitly stating it shows good faith
5. **Three sentences** -- still coffee-readable
6. **Mutual** -- protects both parties equally, reinforcing the cooperative spirit

### Alternative Recommendation: Option B (One Sentence)

If even three sentences feel too heavy, use a single sentence:

> "Neither Party shall be liable to the other for indirect or consequential losses arising from this cooperation, and each Party's aggregate liability under this Agreement shall not exceed EUR 50,000."

This is the absolute minimum that provides meaningful protection.

### What NOT to Do

- **Do not choose Option A** (no clause). The asymmetric risk to Regla as a startup is too significant.
- **Do not choose Option D** (detailed section). It contradicts the agreement's design principle and is disproportionate to the cooperation's nature.

### How to Present This to OptoCeutics

Frame it as mutual protection, not as Regla hedging:

"We've added a standard mutual liability limitation -- it protects both of us equally. It just says we don't chase each other for indirect losses, and there's a reasonable cap on direct liability. It's three sentences. We kept the confidentiality obligations fully enforceable because we take your data seriously."

---

## 8. Sources and References

### Primary Legal Sources
- **Aftaleloven** (Danish Contracts Act), particularly Section 36 (reasonableness)
- **Erstatningsansvarsloven** (Danish Tort Liability Act)
- **Kobeloven** (Danish Sale of Goods Act) -- for the direct/indirect damages distinction by analogy

### Secondary Sources (Research Material)
- Chambers and Partners, [Commercial Contracts 2025 - Denmark](https://practiceguides.chambers.com/practice-guides/commercial-contracts-2025/denmark)
- Schjodt, [Limitation of Liability in Commercial Agreements](https://schjodt.com/news/limitation-of-liability-in-commercial-agreements)
- Schjodt, [Section 36 of Nordic Contract Acts: Impact on Commercial Agreements](https://schjodt.com/news/application-of-section-36-of-the-contract-acts-between-commercial-parties-in-the-nordics)
- ClearContract, [Culpa in Danish Contract Liability](https://www.clearcontract.dk/culpa-danish-contract-liability)
- Lexology, [In Brief: Limiting Contractual Liability in Denmark](https://www.lexology.com/library/detail.aspx?g=55f069ae-708b-45fb-a499-009d6664084d)
- Lexology, [Commercial Contracts in Denmark](https://www.lexology.com/library/detail.aspx?g=4c9e1b57-1e91-4add-a5c7-696e5a182cee)
- Kromann Reumert, [A Brief Guide to Set Up a Joint Venture in Denmark](https://kromannreumert.com/en/news/a-very-brief-guide-to-set-up-a-joint-venture-in-denmark)
- Carsted Rosenberg, [Danish Contract Law](https://www.carstedrosenberg.com/danish-contract-law)
- Baker Tilly Legal, [Entering into Commercial Contracts with Danish Partners](https://www.bakertillylegal.dk/en/insights/what-you-should-know-when-entering-into-a-commercial-contract-with-a-danish-business-partner)

### Key Danish Legal Principles Referenced
- **Culpa** (fault-based liability) -- default liability standard
- **Adaekvans** (foreseeability/adequacy) -- damages must be foreseeable
- **Tabsbegraeningsplikt** (duty to mitigate) -- injured party must mitigate
- **Aftalefrihed** (freedom of contract) -- parties can structure agreements freely
- **Loyalitetspligt** (duty of loyalty) -- implied good faith duty in cooperation
- **Grov uagtsomhed** (gross negligence) -- cannot be excluded contractually
- **Direkte tab / indirekte tab** (direct/indirect loss) -- distinction in damages

---

*This research report is prepared by the Regla Legal AI system for internal use. It is not formal legal advice. Final decisions should be validated with external counsel (Martin).*
