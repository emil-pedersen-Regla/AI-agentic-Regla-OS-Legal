# Legal Decision Records (LDR) - Index

## Overview

This directory contains Lightweight Decision Records (LDR) documenting significant legal decisions affecting Regla ApS. LDRs provide transparency, auditability, and institutional memory for legal choices and their rationales.

**Format**: Follows main project LDR format (see main project decisions/)
**Purpose**: Document "why" for future reference, audit trail, compliance

## Active Decisions

### Corporate Structure
*Decisions about entity structure, jurisdiction, corporate form*

[No decisions yet - will be added as legal decisions are made]

### Contracts and Agreements
*Decisions about contract terms, negotiation positions, standard clauses*

[No decisions yet - will be added as contract decisions are made]

### Compliance Approach
*Decisions about how to comply with regulations, interpretation of requirements*

[No decisions yet - will be added as compliance decisions are made]

### Intellectual Property
*Decisions about IP ownership, protection strategies, licensing approaches*

[No decisions yet - will be added as IP decisions are made]

### Regulatory
*Decisions about regulatory strategies, classifications, submissions*

[No decisions yet - will be added as regulatory decisions are made]

## Superseded Decisions

*Decisions that have been replaced by later decisions*

[None yet]

---

## Decision Categories

Legal Decision Records are organized by category:

1. **Corporate Structure**: Entity selection, jurisdiction, corporate form, reorganizations
2. **Contracts and Agreements**: Standard terms, negotiation positions, contract templates
3. **Compliance Approach**: Regulatory compliance strategies, interpretations
4. **Intellectual Property**: IP ownership policies, protection strategies, licensing
5. **Regulatory**: Medical device classification, regulatory strategies, submissions

## When to Create an LDR

Create a Lightweight Decision Record when:

- **Selecting Legal Structures**: Choosing entity type, jurisdiction, holding structure
- **Establishing Policies**: IP ownership, data handling, contract standards
- **Major Contract Positions**: Negotiation stance on significant terms (e.g., liability cap amounts)
- **Compliance Approaches**: How to interpret and implement regulatory requirements
- **Risk Acceptance**: Deciding to accept certain legal risks with mitigation plan
- **Process Changes**: Significant changes to legal workflows or approval processes

**Do NOT create LDR for**:
- Routine contract reviews (use contract review documents instead)
- Simple legal research (use investigation or guide documents)
- Minor operational decisions
- Decisions without lasting implications

## LDR Template

Use this template for all Legal Decision Records:

```markdown
# LDR-YYYY-MM-DD-Short-Title

**Date**: YYYY-MM-DD
**Status**: Proposed | Approved | Implemented | Superseded
**Decision Maker**: Emil Timmreck Pedersen (CEO) | Board of Directors | [Other]
**Category**: Corporate Structure | Contracts | Compliance | IP | Regulatory

## Context

[Why is this decision needed? What problem does it solve? What are the circumstances?]

## Decision

[What was decided? Be specific and clear.]

## Rationale

[Why was this approach chosen? What are the benefits? What factors were considered?]

## Alternatives Considered

### Alternative 1: [Name]
- **Description**: [What is this alternative?]
- **Pros**: [Advantages]
- **Cons**: [Disadvantages]
- **Why Not Chosen**: [Reasoning]

### Alternative 2: [Name]
- **Description**: [What is this alternative?]
- **Pros**: [Advantages]
- **Cons**: [Disadvantages]
- **Why Not Chosen**: [Reasoning]

## Consequences

### Positive Consequences
- [Expected benefit 1]
- [Expected benefit 2]

### Negative Consequences / Risks
- [Risk or downside 1]
- [Risk or downside 2]

### Mitigations
- [How risks will be mitigated]

## Implementation

**Action Items**:
1. [Specific action 1]
2. [Specific action 2]

**Responsible**: [Who implements]
**Timeline**: [When to implement]
**Dependencies**: [What must happen first]

## Legal Review

**External Counsel**: Martin | [Other counsel]
**Date Reviewed**: YYYY-MM-DD
**Counsel Recommendation**: [Counsel's advice on this decision]
**Counsel Caveats**: [Any warnings or limitations noted by counsel]

## References

- [Related document 1]
- [Related document 2]
- [External guidance or regulation]
- [Prior LDR if superseding]

## Review Schedule

**Next Review**: YYYY-MM-DD
**Review Trigger**: [Event that should trigger review - e.g., "After Series A funding"]

## Update History

- **YYYY-MM-DD**: Decision proposed
- **YYYY-MM-DD**: Decision approved
- **YYYY-MM-DD**: Decision implemented
- **YYYY-MM-DD**: Decision reviewed/amended

---

**Decision Owner**: [Name]
**Last Updated**: YYYY-MM-DD
```

## LDR Naming Convention

**Format**: `LDR-YYYY-MM-DD-short-descriptive-title.md`

**Examples**:
- `LDR-2025-11-10-apslect-entity-structure.md`
- `LDR-2025-11-15-standard-liability-cap-customer-contracts.md`
- `LDR-2025-12-01-founder-vesting-acceleration-terms.md`
- `LDR-2026-01-15-gdpr-data-processing-agreement-approach.md`

**Guidelines**:
- Date is decision date (not LDR creation date if different)
- Use lowercase with hyphens
- Keep title short but descriptive (3-6 words)
- Be specific enough to understand decision from filename

## LDR Lifecycle

```
Proposed → Approved → Implemented → [Active] → [Superseded]
```

### Status Definitions

**Proposed**:
- Decision has been drafted and is under consideration
- Not yet approved
- May be revised based on feedback

**Approved**:
- Decision has been approved by appropriate decision maker (Emil, Board, etc.)
- Not yet implemented
- Implementation planned

**Implemented**:
- Decision has been put into effect
- Actions completed
- This is the "active" status for most decisions

**Superseded**:
- Decision has been replaced by a later decision
- No longer in effect
- Retained for historical record

## Decision Approval Authority

| Decision Type | Approval Required |
|---------------|-------------------|
| Corporate structure changes | Board of Directors + Shareholder approval |
| Contract standard terms (low risk) | CEO (Emil) |
| Contract standard terms (high risk) | CEO (Emil) + External counsel review |
| Major contract positions (>€50K impact) | CEO (Emil) + External counsel review |
| Compliance approaches | CEO (Emil) + External counsel review if complex |
| IP ownership policies | CEO (Emil) + External counsel review |
| Risk acceptance (material) | CEO (Emil) + Board if significant |
| Legal process changes | Legal module + CEO approval |

## LDR Review and Maintenance

### Review Schedule

**Annual Review**:
- Review all active LDRs annually
- Assess if decisions still appropriate
- Update status (Active → Superseded if needed)
- Document review in update history

**Event-Driven Review**:
- After major corporate events (funding, acquisition, etc.)
- When circumstances change significantly
- When external counsel recommends reconsideration
- When compliance requirements change

### Maintenance Responsibilities

**Legal Module**:
- Create LDRs for significant legal decisions
- Maintain index (this file)
- Conduct annual reviews
- Update status as decisions are superseded

**Emil (CEO)**:
- Approve LDRs requiring CEO authority
- Participate in reviews
- Flag when decisions need reconsideration

**External Counsel**:
- Review proposed LDRs when consulted
- Advise on legal implications
- Recommend decision reviews when law changes

## Integration with Main Project

Legal LDRs integrate with main project decision records:

**Cross-References**:
- Link to main project LDRs when legal decisions implement broader business decisions
- Reference legal LDRs from main project when business decisions have legal implications

**Coordination**:
- Coordinate with OS layer decision records (main project decisions/)
- Legal decisions support business objectives

**Example**:
- Main project LDR: "Expand to EU market"
- Legal LDR: "Establish German subsidiary (GmbH) for EU operations"

## Templates and Examples

### Example LDR: Liability Cap in Customer Contracts

```markdown
# LDR-2025-11-20-customer-contract-liability-cap

**Date**: 2025-11-20
**Status**: Proposed
**Decision Maker**: Emil Timmreck Pedersen (CEO)
**Category**: Contracts

## Context

Regla needs a standard liability cap for customer contracts. Without a cap, unlimited liability exposes company to catastrophic risk. With a cap too low, customers may resist. Need to balance protection with marketability.

## Decision

Standard liability cap: 12 months of fees paid by customer
- Applies to direct damages only
- Excludes: IP indemnity, confidentiality breach, willful misconduct
- Can be negotiated higher for large customers (>€100K annual contract value)

## Rationale

- 12 months is market standard for B2B SaaS
- Covers typical damages without unlimited exposure
- Protects company while acceptable to most customers
- Exclusions protect critical interests (IP, confidentiality)

## Alternatives Considered

### Alternative 1: Lower cap (6 months)
- **Pros**: Greater protection for Regla
- **Cons**: May lose deals, not market standard
- **Why Not Chosen**: Too protective, hurts sales

### Alternative 2: Higher cap (24 months)
- **Pros**: More attractive to customers
- **Cons**: Increases exposure, not necessary to win deals
- **Why Not Chosen**: Insufficient protection for risk

### Alternative 3: Fixed amount (e.g., €50,000)
- **Pros**: Predictable exposure
- **Cons**: Unfair for small customers, too low for large customers
- **Why Not Chosen**: Doesn't scale with customer size

## Consequences

### Positive
- Clear, consistent approach to liability negotiation
- Market-standard terms acceptable to most customers
- Manageable financial risk for company

### Negative / Risks
- Some customers may push for higher cap
- Still exposed to 12 months of fees (could be significant for large customers)

### Mitigations
- Insurance (E&O policy) to cover beyond cap
- Higher approval threshold for customers with >€100K contracts
- Quality controls to minimize likelihood of damages

## Implementation

**Actions**:
1. Update customer contract template with 12-month liability cap
2. Brief sales team on rationale and negotiation guidelines
3. Secure E&O insurance policy
4. Document exceptions requiring CEO approval

**Responsible**: Legal module + Sales lead
**Timeline**: Before next customer contract
**Dependencies**: E&O insurance policy in place

## Legal Review

**External Counsel**: Martin
**Date Reviewed**: 2025-11-20
**Counsel Recommendation**: Approved. 12 months is reasonable and market standard.
**Counsel Caveats**: Ensure E&O insurance in place. Consider higher cap for very large customers.

## References

- Customer contract template: docs/templates/Customer_Contract_Template_v01.md
- Market research: docs/investigations/SaaS_Liability_Cap_Market_Research_20251120_v01.md
- E&O insurance policy: [To be added]

## Review Schedule

**Next Review**: 2026-11-20 (annual)
**Review Trigger**: After first customer dispute involving damages

## Update History

- **2025-11-20**: Decision proposed and approved
- **2025-11-20**: Template updated, sales briefed
- **2025-11-20**: Implemented

---

**Decision Owner**: Emil Timmreck Pedersen
**Last Updated**: 2025-11-20
```

## Quick Actions

### Create New LDR
1. Copy template above
2. Fill in all sections thoroughly
3. Save to Legal/decisions/ with proper naming (LDR-YYYY-MM-DD-title.md)
4. Add entry to this index under appropriate category
5. Get approval from appropriate decision maker
6. Implement and update status

### Review Existing LDR
1. Open LDR file
2. Assess if still appropriate given current circumstances
3. Check if any consequences have changed
4. Update status if superseded
5. Document review in update history
6. Update this index if status changed

### Supersede LDR
1. Create new LDR documenting updated decision
2. Reference old LDR in new LDR
3. Update old LDR status to "Superseded"
4. Add superseding LDR reference to old LDR
5. Move old LDR entry to "Superseded" section in this index

## Notes

**First Decision**:
When creating the first legal LDR, consider documenting the foundational decision of establishing the Legal module itself:
- **LDR-2025-11-07-establish-legal-module.md**: Decision to create AI-powered internal legal department
  - Context: Regla needs legal capability for contract review, compliance
  - Decision: Create Legal module using Claude Code
  - Rationale: Cost-effective, scalable, 24/7 availability
  - Alternative: Hire in-house counsel (too expensive at this stage)
  - Alternative: Rely solely on external counsel (too slow and expensive)

---

**Maintain this index as the single source of truth for all legal decisions.**

**Last Updated**: 2025-11-07
**Status**: Active
