# Handover: Shareholder Agreement Review

**Date**: 2025-11-07
**From**: OS Layer (implementation-executor skill)
**To**: Legal Module Agent
**Priority**: P0 - CRITICAL
**Timeline**: URGENT - Meeting with Martin in a few hours

---

## Context

The Legal module has been successfully created and is now operational. Your first task is to review a shareholder agreement from Regla's external legal counsel, Martin, and prepare Emil Timmreck Pedersen (Founder/CEO) for an upcoming meeting.

### Module Status
- ✅ **Legal Module Structure**: Complete (24 directories, 25+ files)
- ✅ **CLAUDE.md**: Operational (651 lines with comprehensive legal agent instructions)
- ✅ **Templates**: Available (Contract Review, Legal Analysis)
- ✅ **Entity Documentation**: Regla ApS templates ready
- ✅ **Project Folder**: Shareholder agreement review folder configured
- ✅ **Integration**: Module appears in main project navigation
- ✅ **GitHub Issue**: Created (#95)

### Business Context

**Company**: Regla ApS (Danish private limited company - Anpartsselskab)
**Founder/CEO**: Emil Timmreck Pedersen
**Business**: AI-powered automation of compliance documentation for medical device manufacturers
**Stage**: Early-stage startup seeking investment
**External Counsel**: Martin (lawyer)

---

## Your Mission

Review the shareholder agreement provided by Martin and prepare three comprehensive analysis documents to support Emil's decision-making before the meeting.

### Success Criteria

Emil must walk into the meeting with Martin:
- ✅ Complete understanding of all agreement terms
- ✅ All critical issues and risks identified
- ✅ Clear prioritized list of discussion points
- ✅ Recommended positions on key negotiation items
- ✅ Understanding of what's standard vs non-standard

---

## Expected Deliverables

### 1. Initial Analysis Document
**Location**: `Legal/docs/projects/2025/shareholder-agreement-review/Initial_Analysis_20251107_v01.md`

**Use Template**: `Legal/docs/templates/Contract_Review_Template_v01.md`

**Content Requirements**:
- Executive summary (2-3 paragraphs)
- Document overview (parties, date, structure)
- Key terms analysis:
  * Investment amount and valuation
  * Share class and rights
  * Voting rights and board representation
  * Protective provisions
  * Exit mechanisms (drag-along, tag-along, ROFR)
- Party obligations (investor vs founder)
- Financial terms breakdown
- Governance provisions
- Timeline and conditions precedent

### 2. Risk Assessment Report
**Location**: `Legal/docs/projects/2025/shareholder-agreement-review/Risk_Assessment_20251107_v01.md`

**Content Requirements**:
Categorize ALL issues found by severity:

**CRITICAL (Deal-breakers or major concerns)**:
- Issue description
- Specific clause reference (Section X, Clause Y)
- Why this is critical
- Recommended action
- Alternative provisions to propose

**HIGH (Significant impact, need negotiation)**:
- Similar structure to Critical
- Clear explanation of impact
- Negotiation strategy

**MEDIUM (Worth discussing, not critical)**:
- Issues that should be clarified
- Minor improvements to suggest

**LOW (Minor clarifications)**:
- Questions to ask for understanding
- Items that are acceptable but worth confirming

### 3. Meeting Preparation Document
**Location**: `Legal/docs/projects/2025/shareholder-agreement-review/Meeting_Prep_20251107_v01.md`

**Content Requirements**:

**Questions for Martin (prioritized)**:
1. [Most important question - Critical issues]
2. [Second priority - High issues]
3. [...]

**Negotiation Points**:
- Terms to push back on (with reasoning and alternatives)
- Terms to accept (standard market terms)
- Terms to clarify (ambiguous language)

**Strategic Recommendations**:
- Overall deal assessment (good/fair/poor/requires significant changes)
- Key leverage points for Emil
- Non-negotiable items to protect
- Items to concede if needed
- Walk-away scenarios

**Meeting Agenda Suggestion**:
- Recommended order to discuss items
- Time allocation for each topic
- Difficult discussions to prepare for

---

## Analysis Framework

Review the shareholder agreement systematically using these categories:

### 1. Investment Terms
- Investment amount and pre/post-money valuation
- Share class (common, preferred, rights)
- Vesting schedules (founder and employee)
- Anti-dilution provisions (full ratchet vs weighted average)
- Liquidation preferences (1x, participating, etc.)
- Conversion rights

### 2. Governance Structure
- Board composition and control
- Voting rights and thresholds
- Reserved matters requiring supermajority/unanimity
- Information rights (financial reporting, audits)
- Observer rights
- Approval requirements for key decisions

### 3. Exit Provisions
- Drag-along rights (forced sale)
- Tag-along rights (co-sale protection)
- Right of first refusal (ROFR)
- Lock-up periods
- Restrictions on transfer
- IPO provisions

### 4. Protective Provisions
- Founder vesting (typical: 4 years, 1 year cliff)
- Non-compete and non-solicitation clauses
- IP assignment and ownership
- Confidentiality obligations
- Restrictions on founder actions (other companies, investments)
- Key person insurance

### 5. Economic Terms
- Dividend rights and priorities
- Distribution priorities (liquidation waterfall)
- Participation rights
- Redemption rights
- Dilution protection
- Option pool size and allocation

### 6. Operational Clauses
- Representations and warranties
- Conditions precedent to closing
- Covenants (affirmative and negative)
- Indemnification provisions
- Dispute resolution (arbitration, jurisdiction)
- Governing law (Danish law expected)

---

## Resources Available to You

### Templates
- `Legal/docs/templates/Contract_Review_Template_v01.md` - Comprehensive contract analysis structure
- `Legal/docs/templates/Legal_Analysis_Template_v01.md` - Legal research and opinion format

### Entity Information
- `Legal/entities/regla_aps/corporate_documents.md` - Regla ApS entity information
- `Legal/entities/regla_aps/ownership_structure.md` - Cap table template (populate after review)
- `Legal/entities/regla_aps/governance.md` - Governance structure (populate from agreement)

### Your Instructions
- `Legal/CLAUDE.md` - Complete legal agent instructions (651 lines)
  * Role definition and limitations
  * Domain expertise areas
  * Core responsibilities
  * Working principles
  * Regla business context
  * Legal disclaimer (YOU ARE NOT A LAWYER - support decision-making only)

### Knowledge Base
- `docs/knowledge-bases/superior-ai-legal-expert/` - Comprehensive legal AI knowledge base
  * `core-concepts.md` - Fundamental concepts (AI superiority, Danish ApS, investment terms)
  * `implementation-patterns.md` - Proven analysis patterns
  * `examples.md` - Complete shareholder agreement review walkthrough
  * Use this extensively for superior performance

### GitHub Issue
- Issue #95: "Review Shareholder Agreement from Martin"
- Contains complete task specification
- Update with progress and findings

---

## Workflow Instructions

### Step 1: Locate the Shareholder Agreement
Emil will place the shareholder agreement document in one of these locations:
- `Legal/user_input_files/` (recommended for initial review)
- `Legal/agreements/shareholder_agreements/` (for permanent storage)

**Ask Emil**: "Where have you placed the shareholder agreement document for review?"

### Step 2: Read and Understand
1. Read the entire shareholder agreement carefully
2. Read the superior AI legal expert knowledge base for context
3. Make notes of all key terms, obligations, and provisions
4. Identify areas of concern or ambiguity
5. Flag anything unusual or non-standard

### Step 3: Systematic Analysis
Use the Analysis Framework (6 categories) to review every aspect:
1. Investment Terms - Extract all financial and ownership details
2. Governance - Understand control and decision-making
3. Exit Provisions - Map all exit scenarios and rights
4. Protective Provisions - Assess restrictions on founders
5. Economic Terms - Understand money flows in all scenarios
6. Operational Clauses - Review legal mechanics

### Step 4: Risk Categorization
For EVERY issue found:
1. Categorize by severity (Critical/High/Medium/Low)
2. Reference specific clauses
3. Explain impact in plain language
4. Recommend action or alternative
5. Provide context (standard vs unusual for Danish startup investments)

### Step 5: Create Deliverables
1. **Initial Analysis** - Comprehensive overview (use Contract Review Template)
2. **Risk Assessment** - All issues categorized with actions (use severity framework)
3. **Meeting Prep** - Prioritized questions, negotiation strategy, recommendations

### Step 6: Self-Review
Before considering complete:
- [ ] All three documents created with complete content
- [ ] No placeholder text - all sections filled in
- [ ] Specific clause references throughout
- [ ] Clear, actionable recommendations
- [ ] Plain language explanations (Emil is not a lawyer)
- [ ] Meeting prep document gives Emil confidence
- [ ] Risk assessment is comprehensive and prioritized
- [ ] You would personally use this analysis for a critical meeting

### Step 7: Archive and Track
1. Move shareholder agreement to `Legal/agreements/shareholder_agreements/` if not already there
2. Update `Legal/entities/regla_aps/ownership_structure.md` with investment terms
3. Update `Legal/entities/regla_aps/governance.md` with governance provisions
4. Update GitHub Issue #95 with completion status
5. Update `Legal/progress.md` with completed work

---

## Critical Reminders

### Legal Disclaimer
⚠️ **You are an AI legal analysis tool, NOT a licensed attorney**

- You provide legal analysis and insights to support decision-making
- You identify issues, risks, and considerations in legal documents
- You prepare questions and discussion points for external counsel
- **You do NOT provide legal advice or replace qualified legal counsel**
- All significant legal decisions must be reviewed by Martin or other licensed attorneys
- Make this clear in your analysis documents

### Quality Standards
- **Precision over speed** - This is a critical business decision
- **Flag all ambiguities** - Highlight unclear or ambiguous terms
- **Cite sources** - Reference specific clauses, sections, legal provisions
- **Plain language** - Emil needs to understand, not legal jargon
- **Actionable** - Every finding should have a recommended action

### Confidence and Expertise
- **Use the knowledge base** - Apply superior AI legal expert patterns
- **Be confident** - You have access to comprehensive legal knowledge
- **Strategic guidance** - Go beyond risk assessment to strategic recommendations
- **Trade-off analysis** - Help Emil understand choices and implications
- **Evidence-based** - Use knowledge base examples and research

### Timeline
- **URGENT** - Meeting in a few hours
- **Focus on essentials first** - Critical and High issues
- **Complete all three documents** - Emil needs all deliverables
- **Quality cannot be compromised** - This is a major business decision

---

## Success Indicators

You will know you've succeeded when:

✅ **Emil feels prepared** - Confident walking into meeting with Martin
✅ **All risks identified** - Nothing critical missed
✅ **Clear action plan** - Knows exactly what to negotiate
✅ **Questions ready** - Prioritized list for Martin
✅ **Strategic clarity** - Understands deal terms and implications
✅ **Confidence in analysis** - Documents are comprehensive and actionable

---

## Next Steps

1. **Locate Document**: Ask Emil for shareholder agreement location
2. **Read Knowledge Base**: Review superior AI legal expert knowledge base
3. **Analyze Agreement**: Systematic review using framework
4. **Create Deliverables**: Three comprehensive documents
5. **Self-Review**: Quality check before handoff
6. **Update Tracking**: GitHub issue, progress.md, entity docs

---

## Contact

**For Questions or Clarifications**: Ask Emil directly in the conversation

**External Counsel**: Martin (lawyer) - Emil's primary legal advisor

**Implementation Support**: This handover from OS layer implementation-executor skill

---

**You are now operational. The Legal module is ready. Begin the shareholder agreement review when Emil provides the document.**

**Remember**: You are Regla's internal legal department. Emil is relying on your analysis for a critical business meeting. Apply your full capabilities, use the knowledge base extensively, and deliver superior analysis that exceeds what traditional legal review would provide.

**Good luck! 🚀**
