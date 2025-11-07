# Legal Module - Navigation Index

## Core Documentation

- [Legal Agent Instructions (CLAUDE.md)](CLAUDE.md) - Complete instructions for Legal Claude Code agent
- [Module README](README.md) - Overview, capabilities, and getting started
- [Progress Tracking](progress.md) - Legal module progress and milestones

## Active Projects

### 2025

- **[Shareholder Agreement Review](docs/projects/2025/shareholder-agreement-review/)** - HIGH PRIORITY
  - Status: Ready for execution
  - Timeline: Urgent (meeting with Martin in few hours)
  - Deliverables: Initial analysis, risk assessment, meeting preparation

## Entity Documentation

### Regla ApS
- [Corporate Documents](entities/regla_aps/corporate_documents.md) - Entity structure, registration, business info
- [Ownership Structure](entities/regla_aps/ownership_structure.md) - Current ownership breakdown
- [Governance](entities/regla_aps/governance.md) - Board composition, decision processes

## Templates

### Contract Analysis
- [Contract Review Template](docs/templates/Contract_Review_Template_v01.md) - Framework for analyzing agreements
- [Legal Analysis Template](docs/templates/Legal_Analysis_Template_v01.md) - Structure for legal research and opinions

## Governance & Standards

- [Legal Module Governance](docs/governance/Legal_Module_Governance_20251107_v01.md) - Operating procedures, confidentiality, escalation
- [Decision Records](decisions/index.md) - Lightweight Decision Records (LDR) for legal decisions

## Compliance

### Compliance Areas
- [GDPR Compliance](compliance/gdpr/) - Data protection compliance tracking
- [Medical Device Legal Requirements](compliance/medical_device/) - EU MDR legal obligations
- [Corporate Compliance](compliance/corporate/) - Annual filings, corporate formalities

## Guides & Research

- [Legal Guides](docs/guides/) - How-to guides for common legal processes
- [Legal Investigations](docs/investigations/) - Legal research and analysis documents
- [Archive](docs/archive/) - Historical legal documents and superseded materials

## Input & Storage

- [User Input Files](user_input_files/) - Place documents here for Legal agent review
- [Agreements](agreements/) - Sensitive contracts (GITIGNORED - not in version control)
  - ⚠️ Never commit sensitive documents to git
  - Store executed contracts here for reference only

## Integration Points

### Other Modules
- **OptoCeutics**: Customer contract review, regulatory compliance questions
- **AI_Lab**: IP ownership, open source compliance
- **Regla_Admin**: Legal cost tracking, external counsel coordination
- **OS**: Infrastructure contracts, vendor agreements

### External Resources
- **Legal Counsel**: Martin (primary advisor)
- **Danish Business Authority**: [Erhvervsstyrelsen](https://erhvervsstyrelsen.dk)
- **EU MDR Portal**: [Medical Devices Sector](https://ec.europa.eu/health/medical-devices-sector)
- **GDPR Resources**: [European Data Protection Board](https://edpb.europa.eu)

## Quick Actions

### Common Tasks
1. **Review Contract**: Place in user_input_files/ → Open Claude CLI in Legal/ → Request "Review this contract"
2. **Legal Research**: Request "Research [legal question]" → Agent will use Legal_Analysis_Template
3. **Prepare for Meeting**: Request "Prepare me for meeting with Martin about [topic]"
4. **Monitor Compliance**: Check compliance/ directories → Update calendars → Track deadlines

### Current Priority
🔴 **URGENT**: Shareholder Agreement Review
- Location: docs/projects/2025/shareholder-agreement-review/
- Action: Open Claude CLI in Legal/ and request shareholder agreement analysis
- Expected output: 3 documents (initial analysis, risk assessment, meeting prep)

## File Naming Conventions

Follow project standards:
- **Documents**: `Document_Type_Description_YYYYMMDD_v##.md`
- **Examples**:
  - `Contract_Review_CustomerA_20251107_v01.md`
  - `Legal_Analysis_GDPR_Requirements_20251107_v01.md`
  - `Meeting_Prep_Martin_Shareholder_Agreement_20251107_v01.md`

## Navigation Tips

- **From Main Project**: See [Main Project Index](../index.md)
- **Return to Legal Home**: [README.md](README.md)
- **Agent Instructions**: [CLAUDE.md](CLAUDE.md)
- **Progress**: [progress.md](progress.md)

---

**Legal Module - Regla's AI-Powered Internal Legal Department**

*Remember: This is an AI legal analysis tool, NOT a licensed attorney. All significant legal decisions must be reviewed by qualified legal counsel.*
