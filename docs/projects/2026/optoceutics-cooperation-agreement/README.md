# OptoCeutics Co-Development Cooperation Agreement

## Project Overview

Regla ApS (3-person AI startup) and OptoCeutics (~50-person medical device company) are entering a co-development partnership. This project covers the research, drafting, and finalization of a **Cooperation Agreement** with embedded NDA.

**Design principle**: As simple as possible. Both companies share the view that European regulation is overly complex. This agreement reflects that mindset - lean, practical, readable by non-lawyers.

## Parties

| Party | Description | Role |
|-------|-------------|------|
| **Regla ApS** | Danish AI startup (~3 people, ~100K EUR/year budget) automating compliance documentation for medical device manufacturers | Technology developer, IP owner |
| **OptoCeutics** | ~50-person Danish medical device company (existing Regla client) | Domain partner, QMS/data provider |

## Deal Structure

- **OptoCeutics gets**: Free platform access (duration depends on cooperation length and circumstances - see agreement Section 7.4)
- **Regla gets**: Access to OptoCeutics' QMS and data for platform development
- **IP**: Regla retains all IP. OptoCeutics keeps their own QMS/data.
- **Confidentiality**: Mutual NDA embedded in the agreement

## Co-Development Scope

1. QMS documentation automation
2. Risk analysis and post-market surveillance documentation
3. Full regulatory strategy (longer-term)

## Project Deliverables

| Document | Location | Status |
|----------|----------|--------|
| Cooperation Agreement (draft v01) | `cooperation-agreement-draft-v01.md` | Complete |
| Contract Rationale | `analysis/contract-rationale.md` | Complete |
| Status Tracker | `status.md` | Living document |

## Research (Background Reference)

Five research reports were produced to inform the agreement drafting. These are reference material - the actual agreement is intentionally much simpler than the research suggested.

| Topic | Location |
|-------|----------|
| Danish cooperation agreement law | `research/danish-cooperation-law.md` |
| NDA best practices (medtech/SaaS) | `research/nda-best-practices.md` |
| IP ownership structures | `research/ip-ownership-structures.md` |
| Mutual protection & liability | `research/mutual-protection-liability.md` |
| QMS data access & GDPR | `research/qms-data-access-gdpr.md` |

## Project Phases

1. **Research** - Complete (2026-02-19)
2. **Drafting** - Complete (2026-02-19)
3. **Meeting with OptoCeutics** - Scheduled (next week)
4. **Negotiation & Revision** - Pending
5. **Signing** - Pending

## Agent Protocol

- All subagents run in foreground (never background) for this project
- Each research/analysis agent produces a full report in the appropriate subfolder
- Each agent returns an XML summary (600-800 tokens) to the orchestrating agent
- XML format is at the discretion of each agent

## Key Contact

- **Regla**: Emil Timmreck Pedersen (CEO/Founder)

## Date Created
2026-02-19
