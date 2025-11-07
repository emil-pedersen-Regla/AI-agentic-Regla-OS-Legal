# Entity Documentation

## Purpose

This directory contains comprehensive information about legal entities relevant to Regla's operations. Currently focused on Regla ApS (the primary operating entity), this structure can be extended to include other entities as the company grows (subsidiaries, holding companies, joint ventures, etc.).

## Structure

```
entities/
└── regla_aps/                      # Regla ApS (Danish Anpartsselskab)
    ├── corporate_documents.md      # Formation docs, registration, basic info
    ├── ownership_structure.md      # Cap table, shareholders, vesting, rights
    └── governance.md               # Board, management, decision-making
```

## Document Overview

### regla_aps/corporate_documents.md

**Purpose**: Central repository for all corporate formation and registration information

**Contents**:
- Entity basics (name, type, jurisdiction, CVR number)
- Business information (focus, products, model)
- Founder information
- Articles of association summary
- Share capital structure
- Registration and filing history
- Bank and tax information
- Insurance policies
- External legal counsel
- Important dates and deadlines

**When to update**:
- Corporate structure changes
- Registration information changes (address, directors)
- Share capital changes
- New insurance policies or renewals
- Changes to external counsel
- At least annually

### regla_aps/ownership_structure.md

**Purpose**: Track ownership, cap table, and shareholder rights

**Contents**:
- Current cap table (shareholders, shares, percentages)
- Share classes and rights
- Vesting schedules (founder, employee, advisor)
- Equity pools (ESOP, advisor pool)
- Fully-diluted capitalization
- Shareholder rights (transfer restrictions, voting, economic)
- Ownership change history
- Share transfer log

**When to update**:
- Immediately after any share issuance, transfer, or repurchase
- Immediately after changes to shareholder rights
- Quarterly to reflect option vestings and exercises
- After investment rounds close
- After option grants or exercises

### regla_aps/governance.md

**Purpose**: Document governance structure and decision-making processes

**Contents**:
- Board of directors composition and responsibilities
- Board meeting procedures and frequency
- Reserved matters requiring special approval
- Shareholder meeting requirements (AGM, EGM)
- Shareholder voting rights and thresholds
- Management structure and authority limits
- Decision-making authority matrix
- Conflict of interest policy
- Corporate formalities and record-keeping
- Governance best practices

**When to update**:
- Board composition changes
- New reserved matters or approval thresholds
- Changes to management team
- After shareholder agreement amendments
- Following governance review (annually recommended)

## Usage Guidelines

### For Legal Analysis Tasks

When reviewing contracts or making legal recommendations, reference entity documentation to:
- Understand current ownership and control dynamics
- Verify authority of individuals to execute contracts
- Assess impact of proposed transactions on ownership/control
- Ensure compliance with shareholder agreement restrictions
- Evaluate governance implications of decisions

### For Contract Review

Check entity documentation when reviewing:
- **Investment agreements**: Verify against current cap table and rights
- **Customer contracts**: Ensure signatory has authority per governance docs
- **Vendor agreements**: Verify approval thresholds met
- **Employment agreements**: Check against equity pool availability
- **Any contract affecting ownership, control, or material operations**

### For Compliance Monitoring

Entity documentation informs compliance with:
- **Corporate filings**: Annual report deadlines, registration updates
- **Shareholder agreements**: Compliance with rights and restrictions
- **Board requirements**: Meeting frequency, quorum, reserved matters
- **Regulatory obligations**: Industry-specific requirements

### For External Counsel Coordination

Provide entity documentation to external counsel when:
- Seeking advice on corporate structure
- Preparing for investment rounds
- Reviewing shareholder disputes
- Planning reorganizations or transactions
- Updating corporate records

## Maintenance Responsibilities

### Primary Responsibility
**Legal Module** - Ensure entity documentation is accurate, complete, and up-to-date

### Coordination
- **Regla_Admin Module**: Cap table management software, financial data
- **CEO (Emil)**: Corporate decisions, board/shareholder meeting outcomes
- **External Counsel (Martin)**: Legal opinion on complex matters, transaction support

### Review Schedule
- **Monthly**: Quick review for any changes needed
- **Quarterly**: Comprehensive review, especially ownership_structure.md (vestings, options)
- **Annually**: Full review during annual report preparation, update governance best practices
- **Event-Driven**: Immediate updates after investments, share transfers, governance changes

## Confidentiality

**Sensitivity Level**: HIGH - Contains sensitive corporate and financial information

**Access Control**:
- Internal use only (Emil, Legal module, Regla_Admin module)
- Share with external counsel on need-to-know basis
- Do not commit financial details or sensitive terms to public repositories
- Store executed shareholder agreements separately in Legal/agreements/ (gitignored)

**Anonymization**:
- When creating examples or patterns for documentation, remove:
  - Specific ownership percentages
  - Financial terms (valuations, investment amounts)
  - Personal information about shareholders
  - Sensitive governance provisions

## Document Naming Conventions

Entity documentation files follow standard project conventions:
- **Descriptive names**: `corporate_documents.md`, `ownership_structure.md`, `governance.md`
- **Version tracking**: Update date in document header on each significant change
- **Update history**: Maintain update history section at bottom of each document

## Future Expansion

As Regla grows, this directory can expand to include:

### Additional Entities
```
entities/
├── regla_aps/                  # Original operating entity
├── regla_holding_bv/           # If holding company created
├── regla_us_inc/               # If US subsidiary created
└── regla_germany_gmbh/         # If German subsidiary created
```

### Additional Documentation Per Entity
- **compliance_tracking.md**: Entity-specific compliance obligations
- **contracts_register.md**: Major contracts entered by this entity
- **regulatory_filings.md**: Industry-specific regulatory submissions
- **tax_structure.md**: Tax residency, transfer pricing, international tax

### Cross-Entity Documentation
- **group_structure.md**: Corporate group diagram and relationships
- **intercompany_agreements.md**: Agreements between entities
- **transfer_pricing.md**: Intercompany pricing policies
- **consolidated_governance.md**: Group-wide governance framework

## Integration with Main Project

Entity documentation integrates with:

### Within Legal Module
- **docs/projects/**: Entity information informs contract reviews and analysis
- **agreements/**: Executed shareholder and corporate agreements reference entity docs
- **compliance/**: Corporate compliance tracking uses entity documentation
- **decisions/**: LDRs reference entity structure in decision-making

### Other Modules
- **OptoCeutics**: Customer contracts executed by Regla ApS
- **AI_Lab**: IP ownership depends on entity structure
- **Regla_Admin**: Financial management aligned with entity structure
- **OS**: Infrastructure contracts must be reviewed against authority limits

## Quick Reference

### Current Entities
- **Regla ApS**: Primary operating entity (Denmark)
  - Status: Operational
  - Jurisdiction: Denmark
  - Type: Anpartsselskab (private limited company)

### Key Information Locations
- **CVR Number**: entities/regla_aps/corporate_documents.md
- **Cap Table**: entities/regla_aps/ownership_structure.md
- **Board Composition**: entities/regla_aps/governance.md
- **Authority Limits**: entities/regla_aps/governance.md (Authority Matrix)
- **Vesting Schedules**: entities/regla_aps/ownership_structure.md

### Common Questions

**Q: Who can sign contracts for Regla ApS?**
A: Check governance.md → Decision-Making Authority → Authority Matrix

**Q: What approval is needed for a €50,000 contract?**
A: Check governance.md → Authority Matrix for contract approval thresholds

**Q: What are the founder vesting terms?**
A: Check ownership_structure.md → Vesting Schedules → Founder Vesting

**Q: Who are the current board members?**
A: Check governance.md → Board of Directors → Current Board Composition

**Q: When is the next annual general meeting?**
A: Check governance.md → Shareholder Meetings → Annual General Meeting

**Q: What is the current ownership breakdown?**
A: Check ownership_structure.md → Current Ownership → Cap Table Summary

## Version

- **Created**: 2025-11-07
- **Last Updated**: 2025-11-07
- **Status**: Initial version, ready for population

---

**Maintain accurate entity documentation - it's the foundation for all legal analysis and decision-making.**
