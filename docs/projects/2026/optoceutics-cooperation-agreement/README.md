# OptoCeutics Consultancy Agreement

## Project Overview

Regla ApS (3-person AI startup) and OptoCeutics A/S (~50-person medical device company) are formalizing their working relationship. This project covers the research, drafting, and finalization of a **Consultancy Agreement** that governs how the two companies work together.

## Spirit of the Agreement

This is a good-faith deal between two Danish companies that already work together. Both parties benefit, and neither is trying to exploit the other.

**Regla is the primary beneficiary.** Regla gets access to OptoCeutics' QMS environment, domain expertise, and real-world feedback from a 50-person medtech company. This is invaluable for building and validating the Platform. Without a partner like OptoCeutics, Regla would be building in isolation.

**OptoCeutics benefits significantly too.** They get a free AI-powered E-QMS platform, including source code access for their own internal use and in their own products. If they bought this on the market, it would cost tens of thousands of euros per year.

**The agreement should be fair to both parties.** We want OptoCeutics to feel this is generous. We want them to succeed. Their success validates our platform and makes it better. At the same time, Regla needs basic protections: IP ownership, confidentiality, and assurance that our source code won't be used to build a competing product.

**The agreement must be simple.** OptoCeutics' signatory (Marcus) needs something that looks like a standard Danish consultancy contract - short, standard, nothing unusual. Both parties share the view that European regulation is overly complex. This agreement reflects that mindset.

## Design Principles

1. **Looks like a standard Danish konsulentaftale** - 6 sections, ~1.5 pages, nothing that would raise eyebrows
2. **Consultancy framing** - Regla provides consulting services as an independent contractor. This is the legal framing, even though both parties understand it's co-development in spirit
3. **Regla owns all IP** - Non-negotiable. Under Danish copyright law, a consultant retains IP by default, so this is the legal default reinforced by contract
4. **Source code license replaces platform access** - OptoCeutics gets source code for internal use and in their own products. Simpler and more valuable than tiered platform access
5. **Protection through IP restriction, not market restriction** - OptoCeutics can do whatever they want as a business. They just can't use Regla's code to build a competing product for third parties. Their own code, their own products: completely unrestricted.
6. **No cash changes hands** - Regla's consideration is IP retention and QMS access. OptoCeutics' consideration is platform/source code access.

## Parties

| Party | Description | Role in Agreement |
|-------|-------------|-------------------|
| **Regla ApS** (CVR 45462013) | Danish AI startup (~3 people, ~100K EUR/year) building an AI-powered E-QMS | Consultant, IP owner |
| **OptoCeutics A/S** (CVR 39769689) | ~50-person Danish medical device company, existing Regla client | Client, source code licensee |

## Deal Structure

- **Regla provides**: Consulting services (QMS automation, regulatory documentation, regulatory strategy) using its proprietary Platform
- **OptoCeutics provides**: Access to QMS environment, domain expertise, practical feedback (not contractually specified - handled as normal client-consultant interaction)
- **OptoCeutics gets**: Free platform access + source code license for internal use and own products
- **Regla gets**: All IP ownership, QMS domain access for platform development
- **IP**: Regla owns everything in the Platform. OptoCeutics owns their QMS/data.
- **Source code restriction**: OptoCeutics cannot distribute the source code to third parties or use it to build a competing product for third parties
- **Confidentiality**: Mutual, embedded in the agreement, 3-year survival
- **Liability**: EUR 50,000 cap, uncapped for confidentiality breaches
- **Termination**: 3 months notice, either side. IP/confidentiality/liability survive.

## What the Platform Is

Regla's Platform is a proprietary AI-powered electronic Quality Management System (E-QMS) for medical device manufacturers. It covers three areas:

1. **Automated documentation generation** - QMS documents (SOPs, work instructions, quality records), clinical evaluation plans and reports, risk analysis, post-market surveillance
2. **Clinical and regulatory data analysis** - Searching clinical studies (PubMed, OpenFDA, clinicaltrials.gov), equivalent device analysis, data synthesis across regulatory sources
3. **Regulatory strategy support** - Regulatory pathway analysis, device classification, wellness/medical device categorization, strategy recommendations

The vision is a complete E-QMS for the age of AI agents - not just document generation, but an intelligence layer for regulatory decision-making.

## Key Decisions and Their Rationale

| Decision | Why |
|----------|-----|
| Consultancy, not cooperation agreement | Marcus (OptoCeutics) needs something standard that goes under the radar internally. Consultancy framing actually strengthens Regla's IP position under Danish copyright law. |
| Source code license instead of 10-year platform access | Simpler (removes most complex section of v01). More valuable for OptoCeutics. Source code license survives termination. |
| No IP assignment clause | Marcus is bound by his own employment constraints and cannot sign IP assignment. Not needed under consultancy - Regla owns what it builds by default. |
| IP-based restriction, not market non-compete | OptoCeutics has its own AI platform that touches regulatory areas. A market non-compete would restrict their own business. IP-based restriction only limits use of Regla's code, not OptoCeutics' own development. |
| No explicit AI rewriting clause | Sends a bad signal ("we think you'll steal our code"). Protection exists through: confidentiality covering architecture/concepts, trade secret law protecting the process, and general source code distribution restriction. |
| No client obligations section | Not standard in consultancy agreements. Listing what OptoCeutics must provide made it look like a two-way cooperation, not a consultancy. |
| Compensation acknowledged as "no cash payment" | Standard konsulentaftaler always address compensation. One sentence avoids the gap without over-explaining. |
| EUR 50,000 liability cap | Danish law applies unlimited liability by default. EUR 50,000 is proportionate for a startup. Confidentiality breaches are uncapped to give NDA teeth. |

## Important Context for Reviewers

- **OptoCeutics has its own internal platform** that does some automated compliance. The agreement's Platform description must be specific enough to avoid overlap with OptoCeutics' own products.
- **Marcus (OptoCeutics signatory) has employment constraints** that prevent him from signing IP assignment clauses. The consultancy framing avoids this issue entirely.
- **Both parties are Danish.** Danish law governs. Danish copyright law defaults IP to the consultant. Danish trade secret law protects source code even without explicit contract clauses.
- **This is a real relationship, not adversarial.** Both parties want the deal to work. The protections are minimum necessary, not maximum possible.
- **The agreement went through 3 drafts**: v01 (cooperation, 5+ pages), v02 (consultancy, 2 pages), v03 (streamlined consultancy, 1.5 pages). Each iteration simplified based on feedback.

## Project Deliverables

| Document | Location | Status |
|----------|----------|--------|
| Consultancy Agreement (draft v03) | `consultancy-agreement-draft-v03.md` | **Current** |
| Consultancy Agreement (draft v02) | `consultancy-agreement-draft-v02.md` | Superseded by v03 |
| Cooperation Agreement (draft v01) | `cooperation-agreement-draft-v01.md` | Superseded by v02 |
| Contract Rationale | `analysis/contract-rationale.md` | Complete (based on v01) |
| Status Tracker | `status.md` | Living document |

## Research (Background Reference)

Eight research reports were produced to inform the agreement drafting. These are reference material - the actual agreement is intentionally much simpler than the research suggested.

| Topic | Agent | Location |
|-------|-------|----------|
| Danish cooperation agreement law | A | `research/danish-cooperation-law.md` |
| NDA best practices (medtech/SaaS) | B | `research/nda-best-practices.md` |
| IP ownership structures | C | `research/ip-ownership-structures.md` |
| Mutual protection & liability | D | `research/mutual-protection-liability.md` |
| QMS data access & GDPR | E | `research/qms-data-access-gdpr.md` |
| Liability in Danish cooperation agreements | F | `research/liability-in-danish-cooperation-agreements.md` |
| Consultancy framing viability (Danish law) | G | `research/consultancy-framing-research.md` |
| AI code rewriting IP risks | H | `research/ai-code-rewriting-ip-risks.md` |
| Danish consultancy agreement templates | I | `research/danish-consultancy-agreement-templates.md` |

## Project Phases

1. **Research** - Complete (2026-02-19)
2. **Drafting v01** (Cooperation Agreement) - Complete (2026-02-19)
3. **Internal Review & v01 Revision** - Complete (2026-02-25)
4. **OptoCeutics Feedback** - Complete (2026-02-26, Marcus review)
5. **Restructuring to Consultancy** - Complete (2026-02-26, v02 and v03)
6. **Meeting with OptoCeutics** - Today (2026-02-26)
7. **Negotiation & Revision** - Pending
8. **Signing** - Pending

## Agent Protocol

- Each research/analysis agent produces a full report in the appropriate subfolder
- Each agent returns an XML summary (600-800 tokens) to the orchestrating agent
- XML format is at the discretion of each agent

## Key Contact

- **Regla**: Emil Timmreck Pedersen (CEO/Founder)

## Date Created
2026-02-19
**Last Updated**: 2026-02-26
