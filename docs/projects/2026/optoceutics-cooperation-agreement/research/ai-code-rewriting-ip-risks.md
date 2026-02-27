# AI-Assisted Code Rewriting: IP Risks Under Danish and EU Law

**Type**: Legal Research Report
**Date**: 2026-02-26
**Prepared for**: Regla ApS -- OptoCeutics A/S Cooperation Agreement
**Status**: Research complete; not legal advice

---

## Executive Summary

The risk that a licensee uses AI tools to rewrite, translate, or restructure licensed source code into functionally equivalent but textually different code is real and growing. Under current Danish and EU copyright law, this type of non-literal reimplementation is **difficult to protect through copyright alone**, because the CJEU has consistently held that software functionality, algorithms, and programming languages are unprotectable ideas. However, **trade secret law** and **well-drafted contractual provisions** together provide robust, enforceable protection -- and are the recommended approach for Regla's situation.

---

## 1. Danish Copyright Law and Software Derivative Works

### 1.1 Legal Framework

Computer programs are protected as literary works under Section 1(3) of the Danish Copyright Act (Ophavsretsloven, Consolidated Act No. 1144 of 2014, as amended). Denmark implements the EU Software Directive (2009/24/EC), which means EU-level case law applies directly.

The originality threshold follows the CJEU standard: a work must be "the author's own intellectual creation" (per Infopaq International A/S v. Danske Dagblades Forening, C-5/08). For software, this means the specific expression of the code -- its particular textual formulation -- is protected. The underlying ideas, algorithms, functionality, and programming language are not.

### 1.2 What Copyright Protects (and Does Not Protect) in Software

**Protected (expression):**
- The specific source code text as written
- Particular creative choices in how code expresses a solution
- Potentially: the creative selection, arrangement, and combination of programming elements (keywords, syntax patterns, command sequences) if sufficiently original

**Not protected (ideas/functionality):**
- Algorithms and mathematical methods
- Software functionality and behavior
- Programming languages and data file formats
- Standard coding patterns and common design approaches
- The "what the code does" as opposed to "how it is written"

### 1.3 AI-Generated Code as Derivative Work

Under current EU law, purely AI-generated code (produced without meaningful human creative input) does not itself qualify for copyright protection, because it is not "the author's own intellectual creation." However, the critical question is not whether the AI output is copyrightable, but whether it **infringes** the copyright in the original code.

If AI-rewritten code reproduces the original's specific expression -- substantial portions of the same code text, variable names, comments, or highly distinctive structural patterns -- it constitutes infringement. If the AI produces functionally equivalent but textually independent code, it likely does not infringe copyright, even if the AI "saw" the original code. This is the core vulnerability.

### 1.4 Reverse Engineering Rights Under Danish Law

The Ophavsretsloven grants licensees mandatory rights to:
- Observe, study, and test software to determine its underlying ideas and principles (implementing Art. 5(3) of the Software Directive)
- Reverse-engineer for interoperability purposes (implementing Art. 6 of the Software Directive)

These rights are mandatory -- contractual clauses that prohibit reverse engineering for these purposes may be set aside by Danish courts. However, the right to study and understand does not equal the right to reimplementation for commercial purposes, and contractual restrictions on *use* of gained knowledge remain enforceable.

---

## 2. The SAS v. World Programming Ruling and Its Implications

### 2.1 The CJEU Ruling (Case C-406/10, 2012)

The SAS Institute v. World Programming Ltd case is the leading EU authority on non-literal software copying. WPL created software that replicated SAS's functionality -- executing the same scripting language -- without copying SAS's actual source code.

**Key holdings:**
1. The functionality of a computer program is not protected by copyright
2. Neither the programming language nor the format of data files is protected under the Software Directive
3. A licensed user may observe, study, and test the program to determine its underlying ideas and principles
4. Allowing copyright over functionality would "monopolise ideas, to the detriment of technological progress and industrial development"

### 2.2 What SAS v. WPL Means for AI Rewrites

The ruling strongly suggests that if OptoCeutics used AI to create functionally equivalent software -- replicating what Regla's code does but with different textual expression -- this would **not** constitute copyright infringement under the Software Directive. The CJEU was explicit: others should be free "to create similar or even identical programs provided that they refrain from copying."

### 2.3 The Architecture/Structure Gap

The SAS ruling left ambiguous whether software architecture, structure, sequence, and organization receive any protection. The CJEU noted these elements "might be protected as works by copyright under Directive 2001/29 [the InfoSoc Directive], if they are their author's own intellectual creation." This is a separate legal basis from the Software Directive, and has not been tested in the AI rewriting context.

The recent CJEU ruling in Sony v. Datel (Case C-159/23, October 2024) reinforced a code-centric interpretation: modifying variables in working memory does not constitute copyright infringement because it does not affect the "expression of the program" in source or object code.

### 2.4 Post-2012 Developments

No CJEU or Danish court ruling has directly addressed AI-assisted reimplementation. Several cases are pending before the CJEU on the concept of "work" and "originality" (Cases C-580/23, C-649/23, C-598/24) that may further clarify boundaries but are unlikely to resolve the AI-specific question.

The U.S. Federal Circuit's 2023 decision in the same SAS dispute further narrowed protection for non-literal elements, finding SAS failed to establish copyrightability of its software's structure and organization. While not binding in Europe, this reflects the international trend.

**Bottom line:** Copyright is insufficient to protect against AI-assisted code rewriting. Regla must rely on other legal mechanisms.

---

## 3. Trade Secret Protection as the Primary Shield

### 3.1 The Danish Trade Secrets Act

The Danish Trade Secrets Act (Lov om forretningshemmeligheder, Act No. 309 of 25 April 2018) implements EU Directive 2016/943. It provides the strongest available protection against AI-assisted code reimplementation.

**Definition (Section 2):** A trade secret is information that:
1. Is secret (not generally known or readily accessible)
2. Has commercial value because it is secret
3. Has been subject to reasonable measures of secrecy

Regla's source code platform clearly qualifies on all three criteria, provided reasonable secrecy measures are maintained.

### 3.2 Does Sharing Under License Preserve Trade Secret Status?

**Yes**, provided:
- The sharing occurs under a written confidentiality obligation (NDA or license with confidentiality terms)
- Access is limited to persons who need it
- The license expressly identifies the code as confidential
- Technical access controls are in place (e.g., repository access management)

This is well-established under both the Danish Act and the EU Directive. Sharing a trade secret with a business partner under appropriate contractual protections is one of the "reasonable measures" contemplated by the law.

### 3.3 How Trade Secrets Address the AI Rewriting Gap

This is where trade secret law fills the gap that copyright leaves open:

**Under copyright:** Functionality is an unprotectable idea. AI-rewritten code with different expression does not infringe.

**Under trade secret law:** Using confidentially shared source code as the basis for AI rewriting constitutes **unlawful use** of a trade secret, regardless of whether the output code is textually different. What matters is:
- The information was obtained under a duty of confidentiality
- The use exceeds what the license permits
- The output is derived from the confidential information

Article 4(3) of the EU Trade Secrets Directive is explicit: use of a trade secret is unlawful when carried out "in breach of a confidentiality agreement or any other duty not to disclose the trade secret" or "in breach of a contractual or any other duty to limit the use of the trade secret."

### 3.4 Critical Advantage: Process vs. Output

Trade secret law protects against the **process** (feeding confidential code into an AI tool to extract its logic), not just the **output** (the resulting rewritten code). Even if the output would not infringe copyright, the act of using confidential source code as AI input -- beyond what the license permits -- constitutes trade secret misappropriation.

### 3.5 Enforcement Under Danish Law

**Preliminary injunctions:** The Danish Trade Secrets Act provides favorable conditions for preliminary injunctions -- the claimant need only prove or render probable that unlawful acquisition, use, or disclosure occurred or is imminent.

**Limitations:**
- Six-month deadline from knowledge of unlawful use to initiate legal proceedings
- No search-and-seizure provisions under the Trade Secrets Act (unlike patent law)
- Criminal sanctions available only for industrial espionage under the Danish Penal Code Section 263, not for contractual breach

---

## 4. Contractual Best Practices for 2026

### 4.1 The Multi-Layer Approach

The recommended approach combines three layers:

1. **Copyright license with explicit AI restrictions** (addresses literal copying)
2. **Trade secret/confidentiality obligations** (addresses non-literal use)
3. **Specific AI use restrictions** (addresses the process of using AI on the code)

### 4.2 Recommended Contract Clauses

#### Clause 1: Expanded Definition of Derivative Works

```
"Derivative Work" means any work that is based on, derived from, or
incorporates any part of the Licensed Software, whether created manually
or through the use of automated tools, including but not limited to:
(a) translations to other programming languages;
(b) restructured, refactored, or reorganized versions;
(c) code generated by artificial intelligence, machine learning, or
    other automated code generation tools that was produced using,
    trained on, prompted with, or informed by the Licensed Software
    or any knowledge derived from it;
(d) functionally equivalent reimplementations based on study or
    analysis of the Licensed Software.
```

#### Clause 2: AI Tool Restrictions

```
The Licensee shall not, and shall ensure that its employees, contractors,
and agents do not:
(a) input, upload, or otherwise provide any portion of the Licensed
    Software, its documentation, or information derived from study
    of the Licensed Software to any artificial intelligence system,
    large language model, code generation tool, or similar automated
    system;
(b) use any such system to generate code that replicates, reimplements,
    or provides functionality substantially similar to the Licensed
    Software or any component thereof;
(c) use knowledge gained from access to the Licensed Software to
    prompt, instruct, or guide any AI system in producing software
    with similar functionality,

except as strictly necessary for the Licensee's permitted internal
use under this Agreement and subject to the confidentiality obligations
herein.
```

#### Clause 3: Trade Secret Acknowledgment

```
The Licensee acknowledges that the Licensed Software constitutes
valuable trade secrets of the Licensor within the meaning of the
Danish Trade Secrets Act (Lov om forretningshemmeligheder). The
Licensee's access to the Licensed Software shall not diminish its
trade secret status. The Licensee shall maintain at least the same
degree of protection for the Licensed Software as it maintains for
its own most confidential information, and in no event less than
reasonable care.
```

#### Clause 4: Purpose Limitation

```
The Licensee's right to use the Licensed Software is limited strictly
to [internal compliance operations / the specific permitted purpose].
Any use of the Licensed Software, or knowledge derived therefrom,
for the development of products or services for third parties is
expressly prohibited, whether such development is performed manually,
with AI assistance, or through any other means.
```

#### Clause 5: Audit Right (Light Touch)

```
Upon reasonable notice and no more than once per calendar year, the
Licensor may request the Licensee to provide a written certification
signed by an authorized officer confirming compliance with the use
restrictions and AI prohibitions in this Agreement. The Licensor may
also request reasonable evidence of such compliance, including
descriptions of the Licensee's internal policies governing the use
of AI tools in connection with the Licensed Software.
```

### 4.3 Process vs. Output Restriction

**Recommendation: Restrict both, but emphasize process.**

Restricting the output alone (forbidding "derivative works") creates an evidentiary burden -- Regla would need to prove the output was derived from its code. Restricting the process (forbidding the act of inputting code into AI tools) is easier to define and enforce contractually, and is supported by trade secret law.

The combination is strongest: even if the output restriction proves difficult to enforce, the process restriction provides an independent basis for breach.

### 4.4 Danish/EU Model Clauses

No Danish-specific model clauses from DIPO (Danish Intellectual Property Office) or the Danish Bar Association (Advokatsamfundet) specifically address AI code rewriting as of February 2026. However:

- The Authors Guild (US) has published model clauses prohibiting AI training on licensed content, which provide useful structural templates
- Bonterms (open-source contracting framework) has published AI Standard Clauses v1.0 with relevant provisions
- Bird & Bird (with a major Copenhagen office) advises on AI-specific contractual clauses and is a leading firm in this area in Denmark
- Gorrissen Federspiel, Plesner, and Kromann Reumert all have active IP/tech practices advising on these issues

The field is moving fast enough that bespoke drafting based on the principles above is currently more appropriate than relying on standardized templates.

---

## 5. Practical Enforceability

### 5.1 Detection Challenges

Detecting AI-assisted code rewriting is genuinely difficult. If done skillfully, the resulting code will share no textual similarity with the original.

**Indicators that may suggest AI reimplementation:**
- Rapid development of functionality that closely mirrors Regla's platform
- Functional equivalence at a level of detail that suggests intimate knowledge of the original
- Architectural patterns, data structures, or API designs that mirror Regla's non-public design choices
- Former employees or contractors who had access to Regla's code involved in the competing development
- Metadata or digital traces showing AI tool usage on Regla's codebase

### 5.2 Evidence a Danish Court Would Need

For a **copyright claim**: Substantial similarity in the code expression itself, plus proof of access. Under current law, functional similarity alone is insufficient.

For a **trade secret claim**: Evidence that (a) the code qualifies as a trade secret; (b) it was shared under confidentiality obligations; (c) the defendant used it beyond the permitted scope. Circumstantial evidence (timeline, functional similarity, personnel overlap) can support the claim. The burden of proof is lower for preliminary injunctions.

For a **contractual breach claim**: Evidence that the specific contractual prohibitions were violated. This may include evidence of AI tool usage, testimony from employees, or forensic analysis.

### 5.3 Technical Measures

**Code fingerprinting and watermarking** for source code are still nascent compared to image/text watermarking. Practical measures include:

- **Distinctive implementation choices**: Intentionally using unusual variable naming, unique algorithmic approaches, or distinctive architectural patterns that would be difficult to explain away if replicated
- **Canary values and honeypots**: Embedding functionally irrelevant but distinctive elements (specific constant values, unusual comment patterns, distinctive test data) that would transfer through naive AI rewriting
- **Access logging**: Maintaining detailed logs of who accessed the repository, when, and what they viewed
- **Repository forensics**: Git history provides timestamps and access patterns that can be correlated with competing product development timelines

These are not silver bullets, but they shift the evidentiary landscape in Regla's favor.

### 5.4 Realistic Enforcement Scenario

In the most likely scenario -- a good-faith commercial relationship that deteriorates -- the contractual provisions serve primarily as:

1. **Deterrent**: Clear terms make it unambiguous that AI rewriting violates the agreement
2. **Basis for negotiation**: If a dispute arises, clear contractual terms provide leverage for a settlement conversation
3. **Preliminary injunction basis**: Danish courts can grant injunctions based on probable breach of contract or trade secret misappropriation
4. **Damages foundation**: Contractual breach provides a clearer path to damages than copyright infringement in this context

Full litigation is unlikely between two good-faith Danish companies. The contract's primary value is in setting clear expectations and providing negotiating leverage.

---

## 6. Recommendations for This Specific Case

### 6.1 Context Assessment

- **Relationship**: Good-faith consultancy between startup (Regla) and established client (OptoCeutics)
- **License scope**: Internal use permitted, third-party product use restricted
- **Primary risk**: Code knowledge being used to build competing products or products for other clients
- **Risk level**: Medium -- OptoCeutics is a medical device company, not a software company, so the incentive to reimpliment is lower than with a technology competitor

### 6.2 Minimum Effective Protection

**Must have (non-negotiable):**

1. **Clear purpose limitation** in the license (internal compliance use only, no third-party product development)
2. **Explicit confidentiality obligations** that identify the source code as a trade secret and impose reasonable care requirements
3. **AI use restriction** that prohibits inputting the code into AI tools for the purpose of generating replacement or competing software
4. **Expanded derivative works definition** covering AI-generated functionally equivalent code
5. **Survival clause** ensuring confidentiality and use restrictions survive termination of the agreement
6. **Return/destruction obligation** upon termination, including any copies, forks, or modifications

**Should have (strongly recommended):**

7. **Annual compliance certification** (light-touch audit mechanism)
8. **Non-compete on derived products** for a reasonable period (2-3 years) after termination
9. **Injunctive relief acknowledgment** (parties agree that breach may cause irreparable harm, supporting injunction applications)

### 6.3 What Would Be Overkill

Given the good-faith nature of the relationship:

- **Real-time code monitoring** or invasive technical surveillance
- **Escrow requirements** for OptoCeutics' internally developed code
- **Mandatory external code audits** by third-party forensic experts
- **Contractual penalties** (Danish law generally disfavors punitive damages; focus on injunctions and actual damages)
- **Broad non-compete clauses** that prevent OptoCeutics from using other compliance software
- **Overly aggressive restrictions** on studying the code for the permitted internal purpose

### 6.4 Implementation Priority

1. **First**: Draft the purpose limitation and AI restriction clauses (this is the contract's backbone)
2. **Second**: Ensure the confidentiality/trade secret provisions are robust
3. **Third**: Add the audit certification mechanism
4. **Fourth**: Review with Danish IP counsel (Gorrissen Federspiel, Kromann Reumert, or Bird & Bird Copenhagen are well-positioned firms for this work)

---

## 7. Key Legal References

### Danish Law
- Ophavsretsloven (Danish Copyright Act), Consolidated Act No. 1144 of 23 October 2014, as amended
- Lov om forretningshemmeligheder (Danish Trade Secrets Act), Act No. 309 of 25 April 2018
- Danish Penal Code, Section 263 (industrial espionage)

### EU Law
- Directive 2009/24/EC on the legal protection of computer programs (Software Directive)
- Directive 2001/29/EC on copyright in the information society (InfoSoc Directive)
- Directive (EU) 2016/943 on the protection of trade secrets (Trade Secrets Directive)
- Regulation (EU) 2024/1689 (AI Act)

### Key Case Law
- SAS Institute Inc v. World Programming Ltd (CJEU, C-406/10, 2012)
- Infopaq International A/S v. Danske Dagblades Forening (CJEU, C-5/08, 2009)
- Sony v. Datel (CJEU, C-159/23, 2024)

### Pending Cases to Monitor
- Mio and Others (C-580/23)
- Institutul G. Calinescu (C-649/23)
- Gandul Media Network (C-598/24)

---

## Disclaimer

This research report is prepared for internal planning purposes at Regla ApS. It does not constitute legal advice. The legal landscape around AI and intellectual property is evolving rapidly. Regla should engage qualified Danish IP counsel for final contract drafting and specific legal advice.

---

*Prepared by: AI Legal Research Agent*
*Date: 2026-02-26*
*Version: 1.0*
