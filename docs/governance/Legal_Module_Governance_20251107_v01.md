# Legal Module Governance

**Version**: v01
**Date**: 2025-11-07
**Status**: Active
**Owner**: Legal Module + Emil Timmreck Pedersen (CEO)

## Purpose and Scope

This document establishes the governance framework for the Legal module, defining how Regla's AI-powered internal legal department operates, handles confidential information, escalates matters to external counsel, and integrates with other modules.

### Scope
- Legal module operations and workflows
- Confidentiality and security requirements
- External counsel coordination
- Integration with main project governance
- Decision documentation protocols
- Quality standards for legal analysis

### Out of Scope
- Regla ApS corporate governance (see entities/regla_aps/governance.md)
- External legal counsel's own governance
- Domain-specific regulations (see compliance/ directories)

## Governance Principles

### 1. Legal Analysis Tool, Not Legal Counsel

**Core Principle**: The Legal module is an AI legal analysis tool that supports decision-making. It is NOT a licensed attorney and does NOT provide legal advice.

**Implementation**:
- Legal disclaimer included in all module documentation (CLAUDE.md, README.md, outputs)
- All analysis documents clearly state they are AI-generated analysis, not legal advice
- Significant legal decisions require review by licensed attorney (Martin)
- Legal module flags matters requiring external counsel involvement

### 2. Confidentiality is Paramount

**Core Principle**: Legal documents often contain highly sensitive information that must be protected rigorously.

**Implementation**:
- .gitignore excludes agreements/ directory from version control
- Sensitive documents stored in Legal/agreements/ only (never committed to git)
- Analysis documents use anonymization when documenting patterns
- Access to sensitive documents limited to authorized individuals
- Secure channels used for transmitting confidential documents

### 3. Precision and Thoroughness

**Core Principle**: Legal analysis requires careful, thorough review. Speed is secondary to accuracy.

**Implementation**:
- No rushing legal analysis - take time needed for thorough review
- Read every word of contracts (no skimming)
- Research unfamiliar terms or concepts before proceeding
- Consider edge cases and "what if" scenarios
- Double-check conclusions before reporting
- Use templates for consistency and completeness

### 4. Risk-Based Approach

**Core Principle**: Categorize all issues by severity to enable prioritized decision-making.

**Implementation**:
- Use four-tier risk categorization (Critical/High/Medium/Low)
- Critical issues escalated immediately to Emil and external counsel
- High issues must be addressed before contract execution
- Document risk assessment methodology in each analysis
- Track risk mitigation actions

### 5. Escalation When Needed

**Core Principle**: Know when to involve external legal counsel. When in doubt, escalate.

**Implementation**:
- Always escalate: Contract execution, regulatory violations, disputes, material corporate changes, high-value transactions (>€50,000)
- Consider escalating: Unfamiliar legal territory, high complexity, time-sensitive high-stakes matters
- Document escalation decisions in analysis
- Coordinate with Emil on external counsel budget and timing

## Operating Procedures

### Contract Review Workflow

1. **Intake**:
   - Contract received in user_input_files/ or agreements/
   - Document received date, source, party requesting review
   - Create project folder: docs/projects/YYYY/[contract-name]/

2. **Initial Review**:
   - Read contract completely (no skimming)
   - Identify contract type and applicable review framework
   - Note any immediate red flags

3. **Detailed Analysis**:
   - Use Contract_Review_Template_v01.md
   - Extract key terms (parties, services, payment, duration, termination)
   - Analyze obligations, rights, restrictions for each party
   - Assess financial terms and economic impact
   - Review governance provisions (if applicable)
   - Evaluate risk allocation (warranties, indemnities, liability caps)
   - Compare against market standards (research if needed)

4. **Risk Assessment**:
   - Categorize all issues (Critical 🔴 / High 🟠 / Medium 🟡 / Low 🟢)
   - For each issue: specific clause reference, explanation, impact assessment, recommendation
   - Prioritize issues for discussion/negotiation

5. **Output Preparation**:
   - Create contract review document in docs/projects/YYYY/[contract-name]/
   - Include executive summary, detailed analysis, risk assessment, recommendations
   - If negotiation needed, prepare redlines with tracked changes
   - Flag areas requiring external counsel review

6. **Escalation**:
   - Escalate to Martin for review before execution
   - Provide complete analysis package
   - Prepare question list for counsel discussion

7. **Post-Execution**:
   - Store executed contract in Legal/agreements/[contract-type]/
   - Update entity documentation if contract affects corporate structure
   - Add to compliance calendar if ongoing obligations
   - Document key terms in contracts register (if maintained)

### Legal Research Workflow

1. **Question Formulation**:
   - Clearly state legal question to be researched
   - Identify why this question is being asked (business context)
   - Determine applicable law (Danish, EU, international)

2. **Research**:
   - Use Legal_Analysis_Template_v01.md
   - Research primary sources (statutes, regulations)
   - Research secondary sources (government guidance, legal databases if available)
   - Research industry standards and common practices
   - Document all sources with citations

3. **Analysis**:
   - Apply law to Regla's specific situation
   - Consider different interpretations and outcomes
   - Assess risks and implications
   - Reach preliminary conclusion with reasoning

4. **Validation**:
   - Self-review: Are there gaps in analysis? Assumptions that need validation?
   - Flag if external counsel review needed
   - Note confidence level (High/Medium/Low)

5. **Documentation**:
   - Save research to docs/investigations/ or docs/guides/
   - Use clear, structured format
   - Include executive summary for quick reference
   - Provide actionable recommendations

6. **Follow-Up**:
   - If external counsel consulted, update research with counsel's input
   - Circulate findings to relevant team members
   - Update guides if research reveals new best practices

### Compliance Monitoring Workflow

1. **Obligation Identification**:
   - Identify all regulatory obligations (corporate, GDPR, industry-specific)
   - Identify contractual obligations with deadlines
   - Document in compliance/ directories

2. **Calendar Maintenance**:
   - Create compliance calendar with all deadlines
   - Set reminders (30 days, 7 days, 1 day before)
   - Coordinate with Regla_Admin for calendar management

3. **Tracking**:
   - Monitor upcoming deadlines
   - Alert responsible parties in advance
   - Verify completion of obligations
   - Document completion (filing confirmations, etc.)

4. **Gap Analysis**:
   - Periodically review compliance status
   - Identify areas of non-compliance or risk
   - Recommend remediation actions
   - Escalate significant gaps to Emil and external counsel

5. **Reporting**:
   - Provide periodic compliance status reports
   - Flag upcoming major deadlines
   - Report on remediation progress

### Meeting Preparation Workflow

1. **Context Gathering**:
   - Understand meeting purpose and objectives
   - Gather all relevant documents (contracts, correspondence, previous advice)
   - Review entity documentation for relevant background

2. **Issue Identification**:
   - List all legal questions and issues for discussion
   - Research each issue to the extent possible
   - Identify what decisions need to be made

3. **Question Development**:
   - Develop specific, prioritized questions for external counsel
   - Most important/urgent questions first
   - Include context for each question
   - Draft potential positions on key issues

4. **Document Preparation**:
   - Create Meeting_Prep_YYYYMMDD_v01.md
   - Include: objectives, key questions (prioritized), background/context, potential positions, alternatives, decision points
   - Attach relevant documents
   - Distribute to Emil in advance

5. **Post-Meeting**:
   - Document counsel's advice and recommendations
   - Update relevant project files with outcomes
   - Create action items list
   - Track implementation of advice

## Confidentiality and Security Requirements

### Document Classification

**Highly Confidential** (Never commit to git):
- Executed contracts with third parties
- Documents containing specific financial terms or valuations
- Legal opinions from external counsel
- Settlement agreements
- Documents marked "Confidential" or "Privileged"
- Personal information requiring GDPR protection

**Confidential** (Can be in docs/, but use care):
- Legal analysis documents (use anonymization if shared beyond core team)
- Research memos on legal questions
- Template contracts (without specific terms)
- Governance policies

**Internal Use**:
- Templates
- Process documentation
- Meeting agendas (without confidential content)

### Storage Requirements

**Highly Confidential Documents**:
- **Location**: Legal/agreements/[type]/ (GITIGNORED)
- **Access**: Emil, Legal module, authorized parties only
- **Backup**: [Secure backup solution, to be determined]
- **Encryption**: [If storing locally, encryption required]

**Confidential Documents**:
- **Location**: Legal/docs/projects/YYYY/[matter-name]/
- **Access**: Project team, Legal module, relevant parties
- **Version Control**: Git (but exclude specific sensitive terms)

**Templates and Policies**:
- **Location**: Legal/docs/templates/ or Legal/docs/governance/
- **Access**: All team members
- **Version Control**: Git

### Anonymization Guidelines

When documenting legal analysis patterns or examples:
- Replace party names with generic labels ("Company A", "Investor B", "Customer X")
- Replace specific financial amounts with ranges (" €X", "between €100K-€500K")
- Remove confidential business details (customer names, proprietary methodologies)
- Focus on legal principles and analysis approach, not specific deal terms
- If in doubt, ask Emil before including in documentation

### Transmission Security

**Email**:
- Use secure email for confidential documents (encrypted if available)
- Mark emails "Confidential" if containing sensitive information
- Verify recipient before sending

**File Sharing**:
- Use secure file sharing platforms (not public links)
- Password-protect highly sensitive documents
- Set expiration dates on shared links
- Track who has accessed documents

**Physical Documents**:
- Store in locked filing cabinet if printed
- Shred sensitive documents when no longer needed
- Do not leave sensitive documents unattended

## External Counsel Coordination

### Primary External Counsel

**Martin**:
- **Firm**: [To be added]
- **Contact**: [To be added]
- **Scope**: Corporate law, investment agreements, commercial contracts, general legal advice

### When to Involve External Counsel

**Always Involve**:
- Contract execution (all contracts reviewed by Martin before execution)
- Regulatory violations or potential violations
- Disputes or threatened litigation
- Material changes to corporate structure
- High-value transactions (>€50,000)
- Complex IP matters (patents, trademarks, complex licensing)
- Employee terminations with potential dispute risk
- Matters where Legal module expresses low confidence

**Consider Involving**:
- Unfamiliar legal territory
- High complexity requiring specialized expertise
- Time-sensitive matters with significant consequences
- Matters where Emil expresses concern or uncertainty
- Second opinion on Legal module's analysis

### Engagement Process

1. **Pre-Engagement**:
   - Legal module prepares comprehensive analysis
   - Develops prioritized question list
   - Gathers relevant documents
   - Emil reviews and approves engagement (budget consideration)

2. **Engagement**:
   - Provide counsel with complete context and analysis
   - Ask specific, prioritized questions
   - Take detailed notes of counsel's advice
   - Clarify any ambiguities

3. **Post-Engagement**:
   - Document counsel's advice in project files
   - Update entity documentation if needed
   - Implement recommendations
   - Track legal costs (coordinate with Regla_Admin)

4. **Follow-Up**:
   - Provide updates to counsel on significant developments
   - Seek clarification if questions arise during implementation
   - Thank counsel and provide feedback on advice quality

### Cost Management

- **Budget Awareness**: Be mindful of legal costs (hourly rates are high)
- **Preparation**: Thorough preparation minimizes counsel time needed
- **Specific Questions**: Ask specific questions rather than open-ended "what should we do?"
- **Coordination**: Coordinate multiple questions into single call/meeting when possible
- **Tracking**: Document legal costs in Regla_Admin module for budget monitoring

## Integration with Main Project Governance

### Documentation Standards

Follow main project standards:
- **Naming Conventions**: Component_Feature_Description_YYYYMMDD_v##.md
- **Decision Records**: Use Lightweight Decision Records (LDR) for significant legal decisions
- **Progress Tracking**: Update Legal/progress.md after significant work
- **File Organization**: Follow documentation lifecycle policy (governance, projects, templates, guides, investigations, archive)

### Cross-Module Coordination

**OptoCeutics**:
- Review customer contracts before execution
- Advise on regulatory compliance questions (GDPR, EU MDR legal aspects)
- Support on customer disputes or issues

**AI_Lab**:
- Clarify IP ownership of research outputs
- Review open source license compliance
- Support on third-party data usage agreements

**Regla_Admin**:
- Track legal costs and external counsel spend
- Coordinate on insurance (D&O, E&O, general liability)
- Support on financial agreements (banking, financing)

**OS**:
- Review infrastructure contracts (Oracle Cloud, hosting)
- Advise on vendor agreements and terms of service
- Support on software licensing questions

### Decision Documentation

**When to Create LDR** (Lightweight Decision Record):
- Selection of legal structures or entity types
- Contract negotiation positions with significant implications
- Compliance approaches requiring policy choices
- IP ownership policies affecting multiple projects
- Risk acceptance decisions on material legal matters

**LDR Template** (see decisions/index.md):
- **Title**: Clear, specific decision
- **Date**: Decision date
- **Status**: Proposed / Approved / Implemented / Superseded
- **Context**: Why this decision is needed
- **Decision**: What was decided
- **Rationale**: Why this approach was chosen
- **Alternatives Considered**: Other options and why not chosen
- **Consequences**: Implications of this decision
- **References**: Relevant documents, external advice

## Quality Standards

### Legal Analysis Quality

**Completeness**:
- Address all material issues in contract/question
- Consider implications from multiple angles (risk, cost, operational, reputational)
- Research unfamiliar terms or concepts
- Don't leave gaps or assumptions unaddressed

**Accuracy**:
- Verify all factual statements
- Cite sources for legal propositions
- Flag when uncertain or confidence is low
- Distinguish between analysis and opinion

**Clarity**:
- Use clear, plain language (avoid unnecessary legalese)
- Structure analysis logically
- Provide executive summary for quick reference
- Use visual aids (tables, lists) to organize information

**Actionability**:
- Provide specific recommendations, not just analysis
- Prioritize issues by importance
- Include next steps
- Make clear what decisions are needed

### Review Process

**Self-Review**:
- Before delivering analysis, Legal module performs self-review:
  - Is analysis complete?
  - Are all sources cited?
  - Is risk assessment clear and accurate?
  - Are recommendations specific and actionable?
  - Is escalation determination appropriate?
  - Would Emil have questions we can preemptively answer?

**External Review**:
- Critical matters reviewed by external counsel before final delivery
- Emil provides feedback on Legal module analysis quality
- Continuous improvement based on feedback

### Continuous Improvement

**Learning from Experience**:
- After external counsel involvement, compare Legal module analysis to counsel's advice
- Identify areas where Legal module's analysis was incomplete or incorrect
- Update templates and processes to prevent similar gaps
- Document lessons learned in docs/guides/

**Template Refinement**:
- Periodically review templates for effectiveness
- Update based on experience and feedback
- Ensure templates capture all necessary analysis elements

**Process Improvement**:
- Identify bottlenecks or inefficiencies in workflows
- Streamline processes without sacrificing quality
- Document improved processes in governance policy updates

## Governance Policy Updates

### Amendment Process

**Minor Updates** (clarifications, non-substantive changes):
- Legal module can update
- Document changes in version history
- Notify Emil of changes

**Major Updates** (substantive policy changes):
- Propose changes to Emil
- Discuss rationale and implications
- Emil approves or rejects
- If approved, increment version number (v01 → v02)
- Document changes in update history

### Review Schedule

- **Annual Review**: Full policy review for relevance and effectiveness
- **Post-Investment**: Review after major corporate events (funding, acquisition, etc.)
- **Issue-Driven**: Review if governance policy proves inadequate or causes problems

### Version History

- **v01 (2025-11-07)**: Initial governance policy created during Legal module setup

## Related Policies

- **Main Project Governance**: [Main project CLAUDE.md](../../../CLAUDE.md)
- **Documentation Lifecycle**: See main project documentation governance
- **Entity Governance**: [entities/regla_aps/governance.md](../../entities/regla_aps/governance.md)
- **Confidentiality**: This document (Confidentiality and Security Requirements section)
- **External Counsel Engagement**: This document (External Counsel Coordination section)

---

**This governance policy ensures the Legal module operates effectively, securely, and in coordination with Regla's overall governance framework.**

**Owner**: Legal Module + Emil Timmreck Pedersen
**Review Date**: 2025-11-07 (annual review due 2026-11-07)
**Status**: Active
