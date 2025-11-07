# User Input Files

## Purpose

This directory is where team members place documents for Legal module review and analysis.

## How to Use

1. **Place documents here** for Legal agent review:
   - Contracts to review
   - Agreements to analyze
   - Legal documents requiring input
   - Supporting materials for legal analysis

2. **Open Claude CLI in Legal/ directory**:
   ```bash
   cd Legal/
   npm run claude  # or your Claude CLI command
   ```

3. **Request analysis**:
   - "Review the shareholder agreement"
   - "Analyze this customer contract"
   - "Review the vendor agreement I just uploaded"

4. **Legal agent will**:
   - Read the document from this directory
   - Perform comprehensive analysis
   - Create analysis documents in docs/projects/
   - Provide recommendations and risk assessment

## Document Storage

### During Review
- Documents being reviewed stay in `user_input_files/`
- Legal agent reads from here for analysis

### After Review
- **Executed contracts**: Move to `Legal/agreements/[contract-type]/` (gitignored for confidentiality)
- **Draft contracts** (not executed): Can be deleted or archived
- **Supporting documents**: Archive in `user_input_files/archive/`

## Confidentiality

**All documents in this directory should be treated as confidential.**

- This directory is in version control (so team can see that documents were received)
- However, **never commit actual sensitive documents** to git
- For highly sensitive documents, place directly in `Legal/agreements/` (which is gitignored)

**Best Practice**:
1. Place document in `user_input_files/` temporarily
2. Request Legal agent analysis
3. After analysis complete, move to appropriate location:
   - Executed contracts → `Legal/agreements/[type]/`
   - Drafts/temporary → Archive or delete

## File Naming Conventions

**Recommended format**: `Document_Type_Party_YYYYMMDD.ext`

**Examples**:
- `Shareholder_Agreement_InvestorName_20251107.pdf`
- `Customer_Contract_CompanyX_20251107.docx`
- `Vendor_Agreement_SupplierY_20251107.pdf`
- `Employment_Contract_JohnDoe_20251107.pdf`

**Why good naming helps**:
- Easy to identify document type
- Easy to find specific documents
- Avoids confusion about version or date
- Professional and organized

## Current Priority

**🔴 URGENT**: Shareholder Agreement Review
- **Status**: Awaiting document
- **Location**: Place shareholder agreement from Martin here
- **Analysis**: Legal agent will produce Initial Analysis, Risk Assessment, and Meeting Prep documents
- **Timeline**: URGENT - meeting with Martin in few hours

**Action**: Once shareholder agreement is placed here, immediately notify Legal agent to begin analysis.

## Archive

`user_input_files/archive/` stores processed documents that don't need to be in agreements/:
- Supporting documents (not contracts)
- Draft contracts (never executed)
- Temporary files used during analysis
- Historical documents for reference

**Archive Naming**: `YYYYMMDD_Document_Description.ext`

## Integration

**Legal agent automatically knows to check this directory when asked to review documents.**

**Example workflow**:
1. Emil places `Shareholder_Agreement_Martin_20251107.pdf` in `user_input_files/`
2. Emil opens Claude CLI in Legal/ directory
3. Emil requests: "Review the shareholder agreement from Martin and prepare me for the meeting"
4. Legal agent:
   - Finds document in `user_input_files/`
   - Performs comprehensive analysis using templates
   - Creates three deliverables in `docs/projects/2025/shareholder-agreement-review/`
   - Reports completion and highlights critical findings
5. Emil reviews deliverables before meeting
6. After meeting, executed agreement moves to `Legal/agreements/shareholder_agreements/`

## Security Notes

- **Never commit sensitive documents to git**
- Use this directory as temporary staging only
- Move sensitive documents to `Legal/agreements/` (gitignored) after processing
- For extra-sensitive documents, place directly in `Legal/agreements/` and reference the path

## Questions

For questions about document placement or process:
- Review `Legal/README.md` for module overview
- Check `Legal/CLAUDE.md` for Legal agent capabilities
- Consult `docs/governance/Legal_Module_Governance_20251107_v01.md` for detailed procedures

---

**Directory**: `Legal/user_input_files/`
**Purpose**: Temporary staging for documents requiring legal review
**Security**: Treat all documents as confidential
**Post-Processing**: Move to appropriate location (agreements/ or archive/)

**Current Priority**: 🔴 Awaiting shareholder agreement for urgent review
