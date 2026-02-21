# IP Ownership Structures for Regla-OptoCeutics Co-Development Agreement

**Type**: research
**Date**: 2026-02-19
**Author**: IP Research Agent (Opus 4.6)
**Status**: Complete
**Jurisdiction**: Denmark / EU

---

## 1. Executive Summary

This report analyzes how to structure IP ownership in a co-development cooperation agreement where Regla ApS retains all intellectual property while OptoCeutics receives perpetual free access to the resulting platform. The analysis covers Danish copyright law, EU directives, creative structuring options borrowed from open-source and platform economics, and concrete clause recommendations.

The central finding is that a **Contributor License Agreement (CLA) hybrid model** -- adapted from open-source practice into a commercial co-development context -- delivers the cleanest IP allocation. OptoCeutics assigns all foreground IP to Regla via a lightweight CLA mechanism embedded in the cooperation agreement, while retaining full ownership of their background IP. In return, OptoCeutics receives a license that is not merely perpetual and royalty-free, but structured as an **irrevocable covenant** with source code escrow protection -- making their access rights practically indestructible even in insolvency scenarios.

---

## 2. The Four-Layer IP Architecture

The most elegant solution is to decompose the IP landscape into four distinct layers, each governed by its own clear rule. This avoids the ambiguity of a single catch-all IP clause.

### Layer 1: Background IP (Pre-Existing)

**Definition**: All IP, know-how, data, processes, and materials each party owns before the cooperation begins, or develops independently outside the cooperation scope.

**Rule**: Each party retains full ownership. No transfer, no license (except as needed for cooperation performance).

**Regla's Background IP**:
- Platform architecture, codebase, AI models, algorithms
- Prompt engineering techniques, validation frameworks
- Existing knowledge bases and regulatory templates

**OptoCeutics' Background IP**:
- QMS documentation, processes, and procedures
- Internal SOPs, risk management frameworks
- Clinical data, post-market surveillance data
- Proprietary manufacturing and quality processes
- Company-specific regulatory strategies

**Critical protection mechanism**: The agreement must include a **Background IP Schedule** -- a concrete list (or at minimum, categorical descriptions) of each party's pre-existing IP. This prevents future disputes about what existed before vs. what was created during the cooperation. Under Danish law, the burden of proof for pre-existence falls on the party claiming it, so documentation at the outset is essential.

**Recommended clause language**:

> "Background IP" means all Intellectual Property Rights owned by or licensed to a Party (a) prior to the Effective Date, or (b) created or acquired by a Party independently of the Cooperation during the Term. Each Party's Background IP is and shall remain the exclusive property of that Party. Nothing in this Agreement shall be construed as transferring, assigning, or granting any ownership rights in Background IP to the other Party, except for the limited licenses expressly granted herein.

### Layer 2: Foreground IP (Co-Created)

**Definition**: All new IP created as a result of, or in connection with, the cooperation activities.

**Rule**: All foreground IP vests in Regla. Period.

This is where the CLA hybrid model proves its value. Rather than trying to parse joint ownership (which under Danish law creates a messy situation where neither party can exploit without the other's consent), the agreement should use an **automatic assignment with license-back** structure.

**Why automatic assignment beats joint ownership under Danish law**:

Under the Danish Copyright Act (Ophavsretsloven), joint ownership of copyright requires that each co-author's contribution be inseparable from the whole. Joint owners cannot independently exploit the work without the other's consent. This would be commercially disastrous for Regla -- every sale to a new customer would theoretically require OptoCeutics' blessing. Joint ownership is a trap, not a compromise.

**The CLA hybrid mechanism**:

OptoCeutics agrees that any contribution they make to the platform -- feedback, feature suggestions, process descriptions, workflow requirements, test results, validation data -- that becomes incorporated into the platform constitutes a "Contribution" subject to automatic IP assignment to Regla.

But here is the creative twist borrowed from sophisticated open-source CLAs: the assignment is **not** of OptoCeutics' underlying knowledge. It is only of the specific expression as incorporated into Regla's platform. OptoCeutics retains the right to use their own knowledge, processes, and methods in any way they see fit -- including sharing them with Regla's competitors.

**Recommended clause language**:

> All Foreground IP arising from or in connection with the Cooperation shall vest in and be the exclusive property of Regla from the moment of creation. To the extent that any Foreground IP does not automatically vest in Regla by operation of law, OptoCeutics hereby irrevocably assigns to Regla all right, title, and interest in and to such Foreground IP, including all Intellectual Property Rights therein, and agrees to execute any documents reasonably necessary to perfect such assignment.
>
> For the avoidance of doubt: (a) the assignment of Foreground IP does not transfer any Background IP of OptoCeutics; (b) OptoCeutics retains the unrestricted right to use, disclose, and exploit its own knowledge, processes, methods, and know-how, regardless of whether such knowledge was also contributed to or reflected in the Cooperation; and (c) the obligation to assign Foreground IP extends only to the specific expressions, implementations, and embodiments incorporated into or developed for the Platform, not to the underlying ideas, concepts, or general methodologies of OptoCeutics.

### Layer 3: Sideground IP (Incidental Creations)

**Definition**: IP created by either party during the cooperation period but outside the defined cooperation scope, yet potentially related to it.

**Rule**: Belongs to the creating party. No automatic assignment.

This layer is often overlooked, but it matters. If OptoCeutics develops a new internal QMS process during the cooperation period that is inspired by (but not part of) the co-development work, that sideground IP belongs entirely to OptoCeutics. Conversely, if Regla develops a new AI technique during the cooperation that was not part of the defined scope, that belongs to Regla.

The EU Horizon 2020 framework's treatment of sideground provides a well-tested model here: sideground is the creating party's property, with no automatic access rights for the other party unless specifically agreed.

### Layer 4: Postground IP (Future Improvements)

**Definition**: Improvements, derivatives, and enhancements to foreground IP created after the cooperation ends or beyond the cooperation scope.

**Rule**: Belongs to the creating party (in practice, Regla, since they own the platform).

This is the "improvements and derivatives" question. The answer should be unambiguous: all improvements to the platform, including those inspired by OptoCeutics' earlier feedback, belong to Regla. The license-back to OptoCeutics covers the platform "as improved" (see Section 3), so OptoCeutics benefits from improvements without needing to own them.

**Anti-grant-back provision**: The agreement should explicitly state that OptoCeutics has NO obligation to assign improvements they make independently to their own processes, even if those improvements were inspired by using the Regla platform. This is the reciprocal fairness that makes the deal work.

---

## 3. The License-Back: Making OptoCeutics' Access Indestructible

The license back to OptoCeutics is not just compensation -- it is the commercial consideration that makes the entire IP assignment enforceable. Under Danish contract law (Aftaleloven), a promise without consideration can be challenged. The license-back provides the mutuality.

### Recommended License Structure

**Type**: Perpetual, irrevocable, royalty-free, non-exclusive, non-transferable (with limited transferability exceptions)

**Scope**: Use of the Platform for OptoCeutics' own internal business purposes, including all updates, improvements, and new versions made available during and after the cooperation period.

**Key attributes**:

1. **Perpetual**: No expiration date. Survives termination of the cooperation agreement.

2. **Irrevocable**: Cannot be revoked by Regla under any circumstances, including breach of the cooperation agreement (the license survives independently). This is critical -- an "irrevocable" license that can be terminated for breach is not truly irrevocable.

3. **Royalty-free**: No fees, ever. This should be stated as applying to the current platform and all future versions.

4. **Non-exclusive**: Regla can license to anyone. This is essential for Regla's business model.

5. **Non-transferable with acquisition carve-out**: The license is personal to OptoCeutics but follows OptoCeutics in a change-of-control event (acquisition, merger). This protects OptoCeutics from losing access if they are acquired. However, the license does NOT extend to the acquirer's other portfolio companies -- only to the business that was OptoCeutics at the time of acquisition.

### Creative Enhancement: The "Most Favored Licensee" Clause

Here is an unusual but powerful provision: OptoCeutics receives a "most favored licensee" commitment. Regla warrants that OptoCeutics will always receive access to the platform on terms no less favorable than those offered to any other licensee. If Regla ever offers a better deal to someone else (e.g., additional features, better SLA), OptoCeutics automatically gets the same.

This transforms OptoCeutics from "getting free access" to "getting the best access" -- a meaningful psychological and commercial distinction that makes the deal far more attractive to OptoCeutics without costing Regla anything significant (since OptoCeutics is already paying nothing).

### Creative Enhancement: Platform Feature Parity Guarantee

Instead of a vague "access to the platform" license, guarantee that OptoCeutics will always have access to the full feature set of the platform, not a stripped-down version. This prevents future temptation to create "premium" tiers that exclude OptoCeutics.

**Recommended clause language**:

> Regla hereby grants to OptoCeutics a perpetual, irrevocable, royalty-free, non-exclusive license to use the Platform, including all Foreground IP incorporated therein, for OptoCeutics' own internal business purposes (the "License"). The License:
> (a) is not terminable by Regla for any reason;
> (b) survives expiration or termination of this Agreement, regardless of the reason for termination;
> (c) extends to all updates, improvements, and new versions of the Platform;
> (d) includes access to all features and functionalities available to any other Platform licensee;
> (e) transfers to any successor entity of OptoCeutics in a change of control event, provided that the License shall not extend beyond the scope of OptoCeutics' business as conducted at the time of the change of control.

---

## 4. Moral Rights Under Danish Law

### The Problem

Under the Danish Copyright Act Section 3, the author of a work has inalienable moral rights, specifically:
- **Attribution right** (droit de paternite): The right to be identified as the author
- **Integrity right** (droit au respect): The right to object to derogatory treatment of the work

These moral rights **cannot be waived generally** under Danish law -- they can only be waived for "uses limited in nature and extent." This creates a theoretical problem: if an OptoCeutics employee contributes creative material that ends up in Regla's platform, that employee retains moral rights even after IP assignment.

### The Solution

In practice, this issue is minimal for software and SaaS platforms for several reasons:

1. **EU Software Directive (2009/24/EC)**: Computer programs created by employees in the course of their duties vest economic rights in the employer exclusively. Denmark has implemented this. OptoCeutics' employees' contributions to the cooperation are made in the course of their duties for OptoCeutics, so the economic rights vest in OptoCeutics, who then assigns them to Regla.

2. **Nature of contributions**: OptoCeutics' contributions are primarily functional (QMS requirements, process descriptions, feedback) rather than artistic. Danish moral rights attach most strongly to artistic and literary works. Functional contributions to software have minimal moral rights exposure.

3. **Practical waiver**: While a blanket waiver of moral rights is invalid, a specific waiver for the defined cooperation outputs is enforceable. The agreement should include a clause where OptoCeutics (and through their employment agreements, their employees) waives moral rights specifically in relation to contributions incorporated into the Platform, to the extent permitted by law.

**Recommended clause language**:

> To the extent permitted by applicable law, including Section 3 of the Danish Copyright Act, OptoCeutics waives, and shall procure that its employees and contractors waive, any moral rights in Contributions incorporated into the Platform, specifically including the right of attribution and the right to object to modification, in relation to the Platform and any derivative works thereof. OptoCeutics acknowledges that the Contributions will be integrated into a collective work (the Platform) in which individual attribution is not practical.

---

## 5. Data vs. IP: The Critical Distinction

### Why This Matters

OptoCeutics' QMS data is the most commercially sensitive element of the cooperation. It is NOT intellectual property in the traditional sense (no creative authorship), but it may be protected under:

1. **EU Database Directive (96/9/EC) sui generis right**: If OptoCeutics has made a substantial investment in obtaining, verifying, or presenting the data, they may have sui generis database rights
2. **Trade secret protection**: Under the EU Trade Secrets Directive (2016/943) and Danish implementation
3. **Contractual protection**: The NDA/confidentiality provisions of the agreement itself
4. **EU Data Act (Regulation 2023/2854)**: Applicable from September 2025, creating new data access rights

### The Recommended Data Framework

Create a clear three-tier data classification:

**Tier 1: Raw QMS Data** (OptoCeutics retains all rights)
- Actual QMS documents, SOPs, work instructions
- Clinical data, post-market surveillance data
- Product-specific regulatory files
- **Treatment**: Licensed to Regla for development and training purposes ONLY. Must be returned or destroyed at cooperation termination. Cannot be shared with third parties. Cannot be used to directly benefit competitors.

**Tier 2: Abstracted Insights** (Becomes part of Regla's platform knowledge)
- Generalized patterns derived from QMS data (e.g., "medical device companies typically structure QMS sections like X")
- Industry best practices extracted from data
- Regulatory requirement patterns
- **Treatment**: These abstract insights, once sufficiently generalized and anonymized to not reveal OptoCeutics-specific information, become part of Regla's platform IP. This is analogous to how a consultant gains expertise from each client engagement.

**Tier 3: Platform-Generated Outputs** (New IP owned by Regla)
- AI model weights and parameters trained on data
- Template structures and documentation frameworks
- Automated workflows and validation logic
- **Treatment**: Full Regla ownership as foreground IP.

**The "Generalization Boundary"**: The key to making this work is defining a clear test for when Tier 1 data becomes Tier 2 abstracted insight. The recommended test: information that has been (a) de-identified so it does not reveal OptoCeutics-specific processes, products, or strategies, AND (b) combined with information from at least one other source such that OptoCeutics' specific contribution is not separately identifiable.

**Recommended clause language**:

> OptoCeutics grants Regla a non-exclusive, non-transferable license to access and use OptoCeutics' QMS Data solely for the purpose of developing, training, and validating the Platform during the Cooperation Term (the "Data License"). The Data License:
> (a) does not transfer any ownership rights in the QMS Data to Regla;
> (b) prohibits Regla from sharing unmodified QMS Data with any third party;
> (c) permits Regla to derive generalized, anonymized, and aggregated insights from the QMS Data, provided that such insights do not reveal OptoCeutics-specific information, processes, or strategies;
> (d) shall terminate upon expiration or termination of this Agreement, at which point Regla shall return or destroy all copies of the QMS Data, provided that Regla may retain (i) generalized insights already incorporated into the Platform and (ii) backup copies required by law, subject to continuing confidentiality obligations.

### EU Data Act Considerations

The EU Data Act (applicable since September 2025) creates obligations for data holders to share data generated by connected products and related services. While this primarily affects IoT and connected device data, medical device companies should be aware that:

- Data generated by medical devices must generally be made accessible to users
- Sui generis database rights cannot be used to prevent data access under the Data Act
- However, trade secrets remain protected, and manufacturers have a veto right where data sharing could cause serious economic harm

For the Regla-OptoCeutics cooperation, the Data Act reinforces the approach of separating data access rights from IP ownership. OptoCeutics' QMS data is not "connected product data" in the Data Act sense, so the Act's mandatory sharing obligations do not directly apply. But the Act's philosophy of separating data access from ownership aligns with the Tier 1/2/3 framework above.

---

## 6. Non-Compete and Exclusivity: The Customization Shield

### The Problem

OptoCeutics' most legitimate concern: "Will Regla take the specific customizations we helped build and hand them directly to our competitors?"

### The Creative Solution: Customization Exclusivity Window

Instead of a broad non-compete (which would cripple Regla's business model), offer a **Customization Exclusivity Window**:

- Any feature, template, or workflow specifically built FOR OptoCeutics during the cooperation receives a 12-month exclusivity window before it can be offered to competitors in OptoCeutics' specific market segment
- General platform features (built for everyone) are excluded from this exclusivity
- After 12 months, the customization becomes part of the general platform

This is borrowed from enterprise SaaS contracts where large customers negotiate "development sprints" and receive temporary exclusivity on the resulting features.

**Why this works for both parties**:
- OptoCeutics gets a genuine competitive advantage: they always have features 12 months before competitors
- Regla retains full IP ownership and can eventually offer features to everyone
- The exclusivity is narrow (specific customizations, not the entire platform) and time-limited

**Recommended clause language**:

> Any Platform functionality specifically developed at OptoCeutics' request and based on OptoCeutics-specific requirements (a "Custom Feature") shall be subject to an exclusivity period of twelve (12) months from the date such Custom Feature is first made available to OptoCeutics (the "Exclusivity Window"). During the Exclusivity Window, Regla shall not offer the Custom Feature to any third party operating in OptoCeutics' primary market segment. After expiration of the Exclusivity Window, Regla may incorporate the Custom Feature into the general Platform offering without restriction. For the avoidance of doubt, general Platform features developed based on industry-wide needs are not Custom Features, even if OptoCeutics provided input or feedback on such features.

---

## 7. Exit Scenarios: Bulletproofing the Structure

### Scenario A: Regla is Acquired

**Risk**: Acquirer may not honor the license or may try to charge OptoCeutics.

**Protection**:
- The license is structured as an irrevocable covenant running with the IP, not a personal commitment of Regla's management
- Include an explicit "successor and assigns" clause binding any acquirer
- Add a source code escrow provision (see below) as ultimate backstop

### Scenario B: OptoCeutics is Acquired

**Risk**: OptoCeutics' acquirer might try to extend the free license beyond OptoCeutics' business.

**Protection**:
- License follows OptoCeutics' business but is limited to the business scope as it existed at the time of the change of control
- New parent company / affiliates / other portfolio companies do NOT inherit the license
- The acquirer gets no right to sublicense

### Scenario C: Cooperation Terminates

**Risk**: Unclear what happens to the license and data.

**Protection**:
- License survives termination (it is irrevocable and perpetual -- termination of the cooperation agreement does not affect the license)
- Data license terminates: Regla returns/destroys raw QMS data, but retains generalized platform insights
- Both parties retain their background IP unchanged

### Scenario D: Regla Goes Bankrupt/Insolvent

**Risk**: Under Danish insolvency law (Konkursloven), an insolvency administrator (kurator) may reject executory contracts. If the license is deemed an executory contract, the administrator could potentially terminate it.

**This is the hardest scenario and requires the most creative solution.**

**Protection mechanisms (layered)**:

1. **Structure the license as fully performed (executed), not executory**: If OptoCeutics' obligations under the license are fully performed (they have already made their contributions), the license is arguably not executory, and the administrator cannot reject it. The agreement should frame the license as granted in consideration of contributions already made, not as an ongoing exchange.

2. **Source code escrow**: Regla deposits source code with a neutral escrow agent. Release triggers include: (a) Regla's insolvency, (b) cessation of platform operations, (c) material breach of the license. This gives OptoCeutics the ability to self-host if Regla disappears.

3. **License characterized as a covenant running with the IP**: Under Danish law, characterizing the license as a servitude or encumbrance on the IP (rather than a personal contractual right) strengthens its survivability in insolvency. Include language stating the license is an encumbrance on the Foreground IP that any transferee takes subject to.

4. **Step-in rights**: If Regla enters insolvency proceedings, OptoCeutics has the right to step in and assume hosting/maintenance obligations for the platform (at its own cost) to ensure continuity.

**Recommended clause language**:

> The License granted under Section [X] constitutes an irrevocable encumbrance on the Foreground IP and shall be binding on Regla's successors, assigns, transferees, and any insolvency administrator or equivalent. The Parties acknowledge that the License is granted in consideration of OptoCeutics' Contributions already made or to be made under this Agreement, and is not conditional upon the continued performance of the Cooperation. In the event of Regla's insolvency, dissolution, or cessation of Platform operations, OptoCeutics shall have the right to access the escrowed source code under the Source Code Escrow Agreement and to operate the Platform for its own internal use.

---

## 8. Creative Structures: Beyond Standard Practice

### 8.1 The "Founding Partner" Model

Instead of framing OptoCeutics as a "licensee who gave up IP," frame them as a "Founding Development Partner" with named recognition. This is borrowed from the venture capital concept of "anchor investors" and gaming industry "founders editions."

**Concrete benefits**:
- OptoCeutics is listed as a "Founding Development Partner" on Regla's website and marketing materials (with OptoCeutics' consent)
- OptoCeutics receives priority access to beta features and new releases
- OptoCeutics has a standing seat on a "Product Advisory Board" (non-binding, consultative)
- OptoCeutics receives annual platform usage reports and roadmap previews

**Why this matters for IP**: It reframes the narrative from "OptoCeutics gave away their IP contributions" to "OptoCeutics co-founded the platform and has a permanent privileged relationship." This makes the IP assignment psychologically easier to accept and commercially more valuable.

### 8.2 The "Open Core" Inspiration

Borrowed from the open-source business model: OptoCeutics' contributions (generalized insights, not raw data) could be designated as part of a "community knowledge layer" that benefits all users, while Regla's proprietary algorithms, AI models, and platform code remain proprietary.

This reframes OptoCeutics' contribution as going into a "shared knowledge" layer rather than directly into Regla's proprietary stack. It is more palatable to contribute to a shared industry resource than to a competitor's product.

**Implementation**: Regla could eventually open-source certain knowledge bases or regulatory templates (derived from OptoCeutics' input among other sources) while keeping the AI engine proprietary. This does not require any IP concession -- Regla would still own everything -- but it changes the narrative.

### 8.3 The "Reverse Royalty" Model

Rather than OptoCeutics receiving a percentage of revenue (which creates complexity and audit rights), Regla commits to investing a defined percentage of platform revenue back into platform development. This ensures OptoCeutics' free platform keeps improving.

**Example**: Regla commits that at least 40% of gross platform revenue will be reinvested in R&D and platform development during the first 5 years. This is not a legal obligation to OptoCeutics per se, but a covenant that assures OptoCeutics the platform will not be abandoned after Regla finds paying customers.

### 8.4 Contribution Acknowledgment Register

Maintain a private, confidential register of all specific contributions made by OptoCeutics. This serves multiple purposes:
- Evidence for background IP vs. foreground IP disputes
- Documentation for the "generalization boundary" test
- Historical record if the relationship sours
- Proof of consideration for the IP assignment

---

## 9. Enforceability Under Danish Law

### Contract Formation

Danish contract law (Aftaleloven) requires offer, acceptance, and consideration. The cooperation agreement satisfies all three: Regla offers free platform access and development partnership; OptoCeutics accepts and provides data access, domain expertise, and testing. The IP assignment is part of the overall exchange.

### IP Assignment Validity

Under Danish copyright law, copyright can be assigned by written agreement. The Copyright Act does not require registration of assignments (Denmark has no copyright register). However, for maximum enforceability:
- Use clear, present-tense assignment language ("hereby assigns" rather than "shall assign")
- Include a "further assurances" clause requiring execution of any additional documents
- Maintain the Contribution Acknowledgment Register as evidence

### Choice of Law

The agreement should specify Danish law as governing law and the Copenhagen City Court (or Danish Arbitration Institute) as the dispute resolution forum. Both parties are Danish-connected, and Danish law is favorable to the intended structure.

### Anti-Competitive Considerations

Under EU competition law, IP assignment clauses in co-development agreements can raise concerns if they create an unreasonable restriction on competition. However, the structure here is defensible:
- OptoCeutics voluntarily enters the agreement with clear consideration (free platform access)
- OptoCeutics retains all background IP and can compete freely
- The arrangement does not prevent OptoCeutics from using other platforms or developing their own tools
- The Customization Exclusivity Window is narrow and time-limited

---

## 10. Implementation Recommendations

### Priority Actions

1. **Draft the Four-Layer IP Schedule** before negotiation begins -- it frames the discussion and demonstrates sophistication

2. **Prepare the Background IP Schedule** -- even a high-level categorical listing gives OptoCeutics comfort that their existing IP is protected

3. **Establish the Source Code Escrow** early -- it is Regla's strongest goodwill gesture and costs very little (approximately EUR 500-2,000/year for a standard escrow service)

4. **Use the "Founding Partner" framing** from the first conversation -- it changes the negotiation dynamic from adversarial to collaborative

5. **Keep the agreement under 15 pages** -- complexity is the enemy of execution. The four-layer architecture is inherently simple to explain despite its sophistication

### Clause Priority (Must-Have vs. Nice-to-Have)

**Must-Have**:
- Four-layer IP classification (Background, Foreground, Sideground, Postground)
- Clean foreground IP assignment to Regla
- Perpetual irrevocable royalty-free license to OptoCeutics
- Background IP protection for both parties
- Data access vs. IP ownership distinction
- Insolvency survival provisions

**Nice-to-Have (but strongly recommended)**:
- Source code escrow
- Customization Exclusivity Window
- Most Favored Licensee clause
- Founding Partner recognition
- Contribution Acknowledgment Register
- Product Advisory Board seat

---

## 11. Risk Matrix

| Risk | Likelihood | Impact | Mitigation |
|------|-----------|--------|------------|
| OptoCeutics claims joint ownership of platform | Low | Critical | Clear automatic assignment + CLA structure |
| Foreground/background IP boundary dispute | Medium | High | Background IP Schedule + Contribution Register |
| OptoCeutics employee asserts moral rights | Very Low | Low | Specific waiver clause + employment obligation |
| License termination in Regla insolvency | Low | Critical | Irrevocable covenant + escrow + step-in rights |
| Acquirer of Regla does not honor license | Low | High | Successor/assign binding + encumbrance language |
| OptoCeutics competitor claims data leak | Low | High | Three-tier data framework + strict Tier 1 controls |
| Antitrust challenge to IP assignment | Very Low | Medium | Voluntary agreement with clear consideration |
| OptoCeutics acquired, acquirer claims license extends | Medium | Medium | Change-of-control scope limitation |

---

## 12. Sources and References

- Danish Copyright Act (Ophavsretsloven), LBK nr 1144 af 23/10/2014 (consolidated)
- EU Software Directive 2009/24/EC
- EU Database Directive 96/9/EC
- EU Trade Secrets Directive 2016/943
- EU Data Act, Regulation 2023/2854
- Danish Contracts Act (Aftaleloven)
- Danish Insolvency Act (Konkursloven)
- AIPPI Resolution Q241 (IP Licensing and Insolvency)
- EU Horizon 2020 Framework -- Background/Foreground IP definitions
- Contributor License Agreement patterns (Apache CLA, Google CLA, W3C CLA)
- ICLG Copyright Laws and Regulations Report 2026 Denmark
- Taylor Wessing, "IP Licences and Insolvency" (2020)
- Baker McKenzie, "IP License Agreements in Insolvency Survey" (2020)

---

*Report generated 2026-02-19. This research report is for internal strategic use by Regla ApS and does not constitute legal advice. Final agreement should be reviewed by licensed Danish counsel.*
