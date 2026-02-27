# OptoCeutics Cooperation Agreement - Status Tracker

> **Living document** - Updated continuously as the project progresses.

## Current Phase: Draft v03 Complete - Meeting Today

**Started**: 2026-02-19
**Status**: Draft v03 complete (2026-02-26). Streamlined to match standard Danish konsulentaftale format based on template research. ~1.5 pages. Meeting with OptoCeutics today (2026-02-26).

### Recalibration Note (2026-02-19)

Initial research agents produced overly complex recommendations (liability caps, breach penalties, four-tier systems, novel legal concepts). Founder feedback: Regla is a 3-person startup with ~100K EUR/year budget. Both parties consider EU regulation excessive. The agreement must be:
- **Audit-proof**: When OptoCeutics' Notified Body audits them, the agreement shows a legitimate cooperation exists
- **IP-clear**: Regla owns the IP, period
- **Confidential**: Basic mutual NDA, nothing fancy
- **Simple**: Both CEOs can read it over coffee

Everything else from the research is useful background knowledge but should NOT inflate the agreement.

## Open Questions

- [ ] Agreement language: English or Danish?
- [ ] OptoCeutics contact person / signatory
- [ ] Is there an existing NDA in place from the client relationship?
- [x] Governing law: Danish law (both parties Danish)
- [x] Dispute resolution: Danish courts (keep it simple)

## Decisions Made

| Date | Decision | Rationale |
|------|----------|-----------|
| 2026-02-19 | Agreement type: Cooperation Agreement (not JV, not license) | Simplest structure; no entity creation, no registration, pure contract |
| 2026-02-19 | NDA embedded in cooperation agreement (not separate) | Reduces document count, permits use scope directly references cooperation terms |
| 2026-02-19 | IP fully owned by Regla with perpetual license to OptoCeutics | Regla needs to commercialize; OptoCeutics gets free access |
| 2026-02-19 | Design principle: Maximum simplicity | No overly complex structures; push boundaries but keep it lean |
| 2026-02-19 | Single document approach: 3-5 pages total | Lean agreement readable by non-lawyers |
| 2026-02-19 | **RECALIBRATION**: Drop all complex protections | No breach penalties, no liability matrices, no insurance requirements, no escrow. 3-person startup with 100K budget. |
| 2026-02-19 | Audit-readiness is primary driver | Agreement must look clean and legitimate when OptoCeutics' Notified Body sees it |
| 2026-02-19 | Regla is 3 people, not 50 | Agreement complexity must match company size and resources |
| 2026-02-19 | Frame as "contribution model" not "joint development" | Avoids partnership characterization, simplifies IP, reduces governance |
| 2026-02-19 | "Perpetual Platform Access Right" not "license" | Contractual service access right avoids IP licensing complications |
| 2026-02-19 | Include "negative partnership" clause | Prevents court recharacterization as I/S (unlimited liability) |
| 2026-02-19 | Regla as independent controller (not processor/joint controller) | Avoids DPA requirements; supported by CNIL 2025 guidance |
| 2026-02-19 | Role-based asymmetry (not size-based) | Obligations flow from what each party does, not from headcount |
| 2026-02-25 | Platform access scoped to Background definition (Section 3.1) | Prevents free access extending to unrelated future products Regla may develop independently; ties access to the medtech regulatory platform described in the cooperation |
| 2026-02-25 | Post-termination access also scoped (Section 7.4a) | Consistent with Section 3.1 scoping; 10-year access applies to the cooperation platform, not separate products |
| 2026-02-25 | Fair-use qualifier added to post-termination access (Section 7.4a) | Prevents potential abuse of free access (e.g., excessive compute-heavy usage); "reasonable usage consistent with OptoCeutics' own business needs" |
| 2026-02-25 | Added mutual liability limitation section (new Section 8) | Danish law applies unlimited fault-based liability by default when silent; EUR 50,000 aggregate cap protects both parties proportionate to startup scale; excludes indirect/consequential losses; carves out confidentiality breaches and gross negligence/wilful misconduct |
| 2026-02-25 | Liability cap set at EUR 50,000 | Meaningful protection without being existential for a 100K EUR/year startup; research confirmed no-money nature does not reduce liability under Danish law |
| 2026-02-25 | Confidentiality breaches excluded from liability cap | Ensures NDA teeth remain intact; both parties' confidential information (QMS data, platform IP) deserves uncapped protection |
| 2026-02-25 | IP assignment clause (Section 4.3) kept as-is | Clean assignment is simpler and appropriate for aligned interests; don't preemptively soften own draft |
| 2026-02-25 | Developer resource NOT included in cooperation agreement | Would change deal nature, trigger VAT barter risk, and reduce flexibility; Section 1.2 allows separate written arrangements; recommend side letter if agreed verbally |
| 2026-02-26 | **MAJOR RESTRUCTURING**: Cooperation → Consultancy agreement | Marcus (OptoCeutics) feedback: contract too long, needs to "go under the radar" internally. Consultancy framing actually strengthens Regla's IP position (Danish copyright law defaults IP to consultant). |
| 2026-02-26 | Agreement reduced from 5+ pages to ~2 pages | Marcus requirement. Removed tiered post-termination access (Section 7.4), detailed data handling, IP assignment clause. Replaced with source code license. |
| 2026-02-26 | Source code license granted to OptoCeutics | OptoCeutics gets non-exclusive, non-transferable license for internal use including their own products. Cannot distribute to third parties. License survives termination but revokes on breach. |
| 2026-02-26 | IP assignment clause (old 4.3) REMOVED | Marcus bound by own employment constraints, cannot sign IP assignment. Not needed under consultancy framing - Regla owns what Regla builds by default under Danish copyright law. |
| 2026-02-26 | Use restrictions replace non-compete | IP-based restriction ("don't use our code for third-party products") instead of market-based non-compete ("don't compete in E-QMS"). OptoCeutics free to build own products with own code. 24 months post-termination. |
| 2026-02-26 | OptoCeutics can use source code in own products (non-competing) | Generous grant - costs Regla nothing, builds loyalty. Restricted only from third-party distribution. |
| 2026-02-26 | AI rewriting protection added | Explicit clause prohibiting use of AI tools on source code for creating third-party software. Trade secret acknowledgment added. Based on research: copyright insufficient for AI rewrites, trade secret law protects the process. |
| 2026-02-26 | Confidentiality expanded to cover concepts/architecture | Protects against non-literal copying and AI-assisted reimplementation. Source code acknowledged as trade secret. |
| 2026-02-26 | 10-year post-termination access REMOVED | Replaced by source code license which survives termination. Simpler, shorter, gives OptoCeutics equivalent protection. |
| 2026-02-26 | Platform description: "proprietary AI-powered E-QMS" | More specific than v01 to avoid overlap with OptoCeutics' own internal platform. Covers documentation automation, clinical/regulatory data analysis, regulatory strategy. |
| 2026-02-26 | **v03**: Streamlined to standard konsulentaftale format | Research of 15+ Danish consultancy templates showed v02 had non-standard elements (Use Restrictions section, Trade Secrets Act reference, audit carve-out, explicit no-cash statement). All removed or absorbed. |
| 2026-02-26 | Use Restrictions section removed (was v02 Section 3) | Most non-standard element. Made agreement look like software license. Protection preserved via source code license terms in IP section ("does not include right to distribute or make derived works available to third parties"). |
| 2026-02-26 | AI rewriting clause removed (was v02 Section 3.2) | Sent bad signal. Protection preserved via "derived works" language in source code license and confidentiality covering architecture/concepts. |
| 2026-02-26 | Background C (no-cash explanation) removed | Not standard in consultancy agreements. Deal structure is implicit. |
| 2026-02-26 | "No partnership" replaced with "independent contractor" | Danish practice: "selvstændig erhvervsdrivende" not Anglo-American negative partnership clause. |
| 2026-02-26 | Client obligations section removed | Not standard in consultancy. Made it look like two-way cooperation, not client-consultant. |
| 2026-02-26 | Trade Secrets Act reference removed | Too legally sophisticated for simple konsulentaftale. Trade secret protection still applies by operation of law. |
| 2026-02-26 | Agreement reduced to 6 sections, ~1.5 pages | Matches standard Danish SME konsulentaftale structure. Indistinguishable from routine consultancy contracts. |

## Research Status

| Topic | Agent | Status | Report |
|-------|-------|--------|--------|
| Danish cooperation agreement law | A | Complete | `research/danish-cooperation-law.md` |
| NDA best practices (medtech/SaaS) | B | Complete | `research/nda-best-practices.md` |
| IP ownership structures | C | Complete | `research/ip-ownership-structures.md` |
| Mutual protection & liability | D | Complete | `research/mutual-protection-liability.md` |
| QMS data access & GDPR | E | Complete | `research/qms-data-access-gdpr.md` |
| Liability in Danish cooperation agreements | F | Complete | `research/liability-in-danish-cooperation-agreements.md` |
| Consultancy framing viability (Danish law) | G | Complete | `research/consultancy-framing-research.md` |
| AI code rewriting IP risks | H | Complete | `research/ai-code-rewriting-ip-risks.md` |

---

## Synthesized Findings

### 1. Agreement Architecture (from Agent A)

**Structure**: Single cooperation agreement (~8-15 pages), no separate documents.

**Legal basis**: Danish Aftaleloven (freedom of contract). No specific statute for cooperation agreements. No formality requirements (no registration, written form not legally required but obviously advisable). Electronic signatures valid.

**Critical framing**: "Contribution model" - each party makes one-directional contributions. NOT "joint development" which implies shared ownership. Include explicit "negative partnership" clause stating the agreement does NOT create an I/S, partnership, or agency.

**Implied duty**: Danish law implies loyalitetspligt (loyalty obligation) in cooperation agreements - parties must act in each other's legitimate interests within cooperation scope.

**Governing law**: Danish law, CISG excluded. Dispute resolution: mediation through DIA, then Danish courts (Copenhagen City Court).

**VAT risk**: Barter transaction characterization possible (each side's contribution treated as taxable supply with 25% VAT). Structure contributions as "grants of access" rather than "services". **Tax advisor should review before signing.**

### 2. NDA Architecture (from Agent B)

**Structure**: Embedded as self-contained Article with independent survival clause.

**Definition**: Broad catch-all ("all information disclosed in connection with this Agreement") plus non-exhaustive carve-in list. NO marking requirement (impractical in daily co-development).

**Duration**: Dual-track: 5 years for general confidential information, perpetual for trade secrets.

**Key innovation - "Identifiable form" qualifier**: Regla may use OptoCeutics data to develop generalized platform features, provided no Confidential Information is disclosed to third parties in identifiable form. This single concept makes the entire co-development commercially viable.

**Return/destroy - four-tier system**:
1. Raw data: strict return/destroy within 30 days
2. Backups: encrypted, destroyed in ordinary rotation
3. AI models: need not be destroyed if they cannot extract source data; perpetual confidentiality
4. Derived works: not subject to return/destroy if they don't contain identifiable information

**Novel concept - "Derived Intelligence"**: Patterns/capabilities in AI models developed using Confidential Information but not containing it in identifiable form. Owned by Regla, not subject to return, subject to ongoing confidentiality.

**Residuals clause**: Scoped to human unaided memory only (trade secrets excluded). AI model retention handled separately.

**Medtech carve-outs**: Regulatory audit access for Notified Bodies, safety reporting override, Notified Body disclosure (existence of platform, not details).

**Breach remedies**: Contractual penalty ~DKK 500,000 per material breach + graduated response with 48-hour notification and cure for inadvertent breaches.

### 3. IP Architecture (from Agent C)

**Four-Layer Model**:
- **Background IP**: Each party retains. Documented in Background IP Schedule at signing.
- **Foreground IP**: All co-created IP vests in Regla automatically (CLA-style assignment). Covers specific expressions only, NOT OptoCeutics' underlying knowledge/methods.
- **Sideground IP**: Created during cooperation but outside scope - belongs to creating party.
- **Postground IP**: Future improvements belong to creating party.

**License-back to OptoCeutics**: Perpetual, irrevocable, royalty-free, non-exclusive. Key features:
- Irrevocable covenant (survives termination, even breach)
- Extends to all updates, improvements, future versions
- Most Favored Licensee clause
- Full feature parity guarantee
- Change-of-control transfer (limited to pre-acquisition business scope)

**Data vs. IP distinction (three tiers)**:
1. Raw QMS Data: OptoCeutics owns, licensed to Regla for development only
2. Abstracted Insights: Regla owns (once generalized past "identifiability" boundary)
3. Platform-Generated Outputs: Full Regla ownership

**Creative structures**:
- 12-month customization exclusivity window before features enter general platform
- "Founding Partner" model with Product Advisory Board seat, priority beta access
- Source code escrow (insolvency protection, EUR 500-2000/year)
- Contribution Acknowledgment Register (private evidence for boundary disputes)

**Insolvency protection**: License structured as fully-performed covenant (not executory contract) to survive bankruptcy administrator rejection. Plus escrow and step-in rights.

### 4. Mutual Protection Architecture (from Agent D)

**Core insight**: Standard SaaS liability frameworks produce a cap of ZERO because no money changes hands. Must build from first principles.

**Liability caps**:
- General: EUR 50,000 (meaningful to startup without being existential)
- Enhanced: EUR 100,000 for data-related breaches
- Uncapped: fraud, willful misconduct, gross negligence, confidentiality/IP breach

**Consequential damages**: Excluded by default. Included (up to enhanced cap) for confidentiality and IP breaches only.

**Indemnification**:
- Regla: third-party IP infringement from platform; data breach from Regla's security failures
- OptoCeutics: third-party IP claims from QMS data; regulatory claims from unreviewed platform output

**Warranties**:
- Regla: authority, non-infringement (to knowledge), reasonable professional care, security standards
- OptoCeutics: authority, data rights, data accuracy (at time of provision), regulatory responsibility
- Excluded: fitness for purpose, error-free operation, regulatory compliance certification

**Insurance**: Regla - PI EUR 250K + cyber EUR 250K (EUR 2-5K/year). OptoCeutics - existing commercial liability.

**Termination**: Material breach (30-day cure), insolvency (immediate), confidentiality/IP breach (immediate, no cure), convenience (90 days notice after 12-month minimum).

**Surviving obligations**: Platform access (frozen version), confidentiality (5 years), IP ownership (indefinite), indemnification (3 years).

**Dispute resolution**: Negotiation (30 days) → Mediation via DIA (60 days) → Danish courts.

**Elegance target**: Four clauses, ~750-950 words total for the entire mutual protection section.

### 5. Data Access & GDPR Architecture (from Agent E)

**Headline finding**: 90-95% of QMS data is non-personal organizational data. GDPR does NOT apply to the majority. GDPR is not a barrier.

**Three-tier classification**:
1. Tier 1 (90-95%): Non-personal QMS data. GDPR irrelevant. Flows freely under NDA.
2. Tier 2 (5-8%): Incidental personal data (employee names in headers). Simple pseudonymization.
3. Tier 3 (1-3%): Clinical references. Anonymize before sharing or use synthetic data.

**Controller status**: Regla as INDEPENDENT CONTROLLER (not processor, not joint controller). Avoids DPA requirements. Supported by CNIL 2025 guidance on AI developer qualification.

**Lawful basis** (for the small personal data portion): Legitimate interest (Art 6(1)(f)). CNIL June 2025 confirms commercial AI development qualifies.

**Agreement mechanism**: Data Access and Handling Schedule as annex (2-3 pages). NOT a formal Article 28 DPA.

**AI training**: EDPB Opinion 28/2024 favorable - trained models can be considered anonymous; legitimate interest justifies AI training; trained models are independent works = Regla's IP.

**Security**: Proportionate measures (encryption, access control, MFA, incident response). NOT ISO 27001 or SOC 2 certification. Security maturity clause that scales with growth.

**Progressive data access**: Start with templates/SOPs, then risk files, then clinical frameworks. Builds trust naturally.

---

## Key Tensions to Resolve

| Tension | Agent A | Agent D | Resolution |
|---------|---------|---------|------------|
| Termination notice | 6 months | 90 days after 12-month minimum | Lean toward 90 days (Agent D) - more startup-friendly, 12-month minimum protects cooperation |
| Dispute resolution | Mediation then arbitration (DIA) | Mediation then courts | Courts (Agent D) - arbitration costs disproportionate for startup |

| Tension | Agent B | Agent D | Resolution |
|---------|---------|---------|------------|
| NDA breach penalty (DKK 500K) vs. general cap (EUR 50K) | Contractual penalty | Liability cap | NDA penalty sits OUTSIDE general cap (it's a liquidated damages clause, not a liability claim) |

## Cross-Stream Synergies

- **"Derived Intelligence" (Agent B)** aligns perfectly with **"Abstracted Insights" (Agent C)** and **"trained model independence" (Agent E)** - use consistent terminology in agreement
- **"Contribution model" framing (Agent A)** directly supports **clean IP assignment (Agent C)** - not a partnership, just one-directional contributions
- **"Identifiable form" qualifier (Agent B)** is the same concept as **"generalization boundary test" (Agent C)** - unify into one definition
- **All agents converge on single-document approach**: 8-15 pages covering everything

## Proposed Agreement Structure

Based on synthesis of all five research streams:

1. **Recitals** (0.5 page) - Parties, background, purpose, "Founding Partner" framing
2. **Definitions** (0.5-1 page) - Confidential Information, Background IP, Foreground IP, Derived Intelligence, Platform, QMS Data
3. **Cooperation Scope & Contributions** (1-1.5 pages) - What each party contributes, phases, governance
4. **Intellectual Property** (1-1.5 pages) - Four-layer model, assignment, license-back, Background IP Schedule
5. **Confidentiality** (1-1.5 pages) - Embedded NDA, dual-track duration, four-tier return/destroy, residuals
6. **Data Access & Handling** (1 page) - Three-tier classification, pseudonymization, security, GDPR compliance
7. **Mutual Protections** (1 page) - Liability caps, indemnification, warranties, insurance
8. **Term & Termination** (0.5-1 page) - Duration, termination rights, surviving obligations
9. **Dispute Resolution** (0.5 page) - Negotiation → Mediation → Courts
10. **General Provisions** (0.5 page) - Negative partnership, amendments, notices, entire agreement
11. **Schedules** - A: Background IP, B: Data Access Classification, C: Platform Access Right

**Estimated total: 10-13 pages**

## Timeline

- **2026-02-19**: Project initiated, all 5 research streams completed, synthesis done, draft v01 completed
- **2026-02-25**: Internal review session. Added platform scope clarification, fair-use qualifier, mutual liability section. Liability research (Agent F) completed. Draft v01 revised.
- **2026-02-26**: Review with Marcus (OptoCeutics). Major restructuring: cooperation → consultancy agreement. Consultancy framing research (Agent G) and AI rewriting risk research (Agent H) completed. Draft v02 created.
- **2026-02-26**: Meeting with OptoCeutics (today)
- **Next**: Negotiation & revision based on meeting feedback

## Blockers

- [ ] VAT barter characterization risk - needs tax advisor review before finalizing
- [ ] Agreement language decision (English vs Danish)

## Notes

- Agreement should be proposal from Regla to OptoCeutics (we are proposing)
- OptoCeutics is an existing client (~50 persons, medical device company)
- Keep everything as simple as practically possible
- Be creative in structuring - think top-tier lawyer, not conservative boilerplate
- All spawned agents run in foreground (not background) for this project
