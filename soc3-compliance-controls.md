---
name: soc3-compliance-controls
description: "Use when the user asks for SOC 3 compliance support, SOC 3 report readiness, public SOC report preparation, SOC 2-to-SOC 3 alignment, trust services criteria summaries, control mapping, audit readiness, evidence request lists, gap assessments, auditor-friendly narratives, or review of SOC 3 marketing and public assurance language for SaaS, cloud, AI, or technology organizations."
license: MIT
metadata:
  version: '1.0'
---

# SOC 3 Compliance Controls

## When to Use This Skill

Use this skill when the user asks for help with SOC 3 or public-facing assurance work, including:

- Preparing for a SOC 3 report based on an existing or planned SOC 2 examination.
- Translating SOC 2 control work into SOC 3-ready summaries and readiness artifacts.
- Creating or reviewing SOC 3 control summaries, report narratives, evidence request lists, gap assessments, or remediation trackers.
- Reviewing public-facing trust, security, privacy, availability, confidentiality, or processing integrity language for consistency with SOC 3 expectations.
- Preparing audit-readiness plans for SaaS, cloud, AI, technology, or enterprise organizations that want a public SOC report.
- Mapping operational practices, policies, risks, systems, or evidence to Trust Services Criteria themes at a summary level.

Do not present work product as legal, accounting, CPA attestation, or official audit opinion advice. If the user needs an official SOC 3 report, opinion, or report language, advise them to work with their CPA firm, auditor, counsel, or qualified compliance advisor.

## SOC 3 Context

SOC 3 is a public-facing attestation report intended for broad distribution. It is typically derived from a SOC 2 examination over the applicable Trust Services Criteria, but it does not include the same detailed control descriptions, test procedures, test results, or restricted-use detail found in a SOC 2 report.

Use these framing principles:

1. SOC 3 work should be consistent with the underlying SOC 2 scope, criteria, report period, system description, management assertion, and auditor opinion.
2. SOC 3 content should be written for a broad audience while avoiding unsupported security, compliance, privacy, availability, or reliability claims.
3. SOC 3 readiness still depends on the same operational control foundation used for SOC 2, including governance, access, change management, system operations, data protection, vendor management, and incident response.
4. Public report language should be conservative, accurate, and aligned with evidence already reviewed or expected to be reviewed by the auditor.

## Core Principles

1. Start by identifying the user's SOC 3 context:
   - Whether a SOC 2 Type II report already exists, is in progress, or is planned.
   - Target SOC 3 report period and expected publication timing.
   - In-scope products, services, infrastructure, locations, teams, and vendors.
   - Applicable Trust Services Criteria: Security is commonly included; Availability, Confidentiality, Processing Integrity, and Privacy may also apply.
   - Intended audience: prospects, customers, procurement teams, public website visitors, partners, investors, or internal leadership.
   - Current audit stage: scoping, readiness, SOC 2 fieldwork, SOC 3 drafting, auditor review, publication, or annual maintenance.

2. Anchor recommendations in public assurance accuracy:
   - What claims will be made publicly?
   - What underlying controls and evidence support those claims?
   - Does the scope match the product, service, geography, and period being described?
   - Are any exceptions, carve-outs, subservice organizations, or criteria limitations relevant?
   - Would a reasonable reader overinterpret the statement?

3. Keep outputs audit-ready and publication-safe:
   - Distinguish internal readiness artifacts from public SOC 3 report language.
   - Avoid implying certification, guarantee, or complete security.
   - Do not invent auditor opinions, seals, criteria coverage, report periods, or report availability.
   - Use placeholders such as `TBD`, `[Auditor]`, `[Report Period]`, and `[In-Scope System]` when details are missing.
   - Flag statements that should be confirmed with the auditor before publication.

4. Treat SOC 3 as an assurance communication layer on top of operational controls:
   - Favor clear, plain-language descriptions that remain supportable.
   - Preserve traceability to SOC 2 scope, controls, policies, evidence, and management assertions.
   - Identify where marketing language needs compliance review before use.

## SOC 3 Domain Map

Use these domains to structure readiness work and to translate operational controls into public-facing assurance themes. Map to specific Trust Services Criteria only when the user provides the applicable criteria or when the mapping is high confidence. Avoid inventing exact criterion references if uncertain.

### Governance and Risk Management

Typical topics:

- Security governance and oversight.
- Risk assessment and risk treatment.
- Policy management and annual review.
- Compliance monitoring.
- Vendor and subservice organization oversight.
- Management assertion readiness.

Common evidence:

- Security policies and standards.
- Risk register and assessment results.
- Management or board security review materials.
- Vendor inventory, risk ratings, reviews, and security documentation.
- Policy approval and review history.
- SOC 2 scoping documents and system description drafts.

### Logical Access

Typical topics:

- User provisioning and deprovisioning.
- Access approvals and role-based access.
- Privileged access management.
- Multi-factor authentication.
- Periodic access reviews.
- Termination and transfer access removal.

Common evidence:

- User access listings.
- Access request and approval tickets.
- Identity provider configuration.
- MFA settings.
- Access review exports and sign-offs.
- Termination tickets and HRIS records.
- Privileged account inventory.

### Change Management

Typical topics:

- Code review.
- Testing and approval.
- Segregation of duties.
- Production deployment controls.
- Emergency change handling.
- Change monitoring.

Common evidence:

- Pull requests and approvals.
- CI/CD pipeline logs.
- Test results.
- Deployment records.
- Change tickets.
- Emergency change documentation.
- Release notes for in-scope systems.

### System Operations and Availability

Typical topics:

- Infrastructure monitoring.
- Logging and alerting.
- Backup and recovery.
- Incident detection and response.
- Capacity management.
- Uptime and availability monitoring.
- Business continuity and disaster recovery planning.

Common evidence:

- Monitoring dashboards.
- Alert policies and incident tickets.
- Backup job reports and restore tests.
- Incident response plan and postmortems.
- Uptime reports.
- DR test records.
- Capacity review evidence.

### Data Protection and Confidentiality

Typical topics:

- Data classification.
- Encryption in transit and at rest.
- Key management.
- Secure data handling.
- Customer data segregation.
- Data retention and deletion.
- Confidentiality commitments.

Common evidence:

- Data classification policy.
- Encryption configuration exports or screenshots.
- Key management policy and access records.
- Retention schedule.
- Data deletion tickets.
- Architecture diagrams.
- Customer data flow diagrams.

### Privacy

Use this domain only when Privacy is in scope or the user asks about personal information handling.

Typical topics:

- Privacy notice alignment.
- Data subject request process.
- Consent or legal basis tracking where applicable.
- Personal data inventory.
- Subprocessor disclosure.
- Privacy incident handling.
- Retention and deletion of personal information.

Common evidence:

- Privacy policy.
- Data inventory or records of processing.
- Data subject request tickets and response logs.
- Consent records where applicable.
- Subprocessor list.
- Privacy training materials.
- Privacy incident procedures.

### Human Resources and Training

Typical topics:

- Security awareness training.
- Confidentiality agreements.
- Acceptable use and policy acknowledgement.
- Background checks where lawful and applicable.
- Onboarding and offboarding.
- Role changes.
- Disciplinary process.

Common evidence:

- Training completion reports.
- Signed employee agreements.
- Policy acknowledgements.
- HRIS onboarding and termination records.
- Background check completion records.
- Offboarding checklists.

## Standard Workflow

Follow this workflow for most SOC 3 requests:

1. Clarify scope if necessary:
   - Ask only for missing details that materially change the output.
   - If the user needs a quick draft, make reasonable assumptions and state them.
   - Confirm whether there is an underlying SOC 2 report or active SOC 2 examination.

2. Identify the intended output:
   - SOC 3 readiness checklist.
   - SOC 2-to-SOC 3 alignment matrix.
   - Evidence request list.
   - Gap assessment.
   - Remediation roadmap.
   - Public trust page language.
   - SOC 3 report narrative draft.
   - Auditor question response.
   - Marketing claim review.

3. Assess current state:
   - Extract stated products, systems, criteria, report period, controls, owners, and evidence.
   - Distinguish audit evidence from public-facing claims.
   - Flag missing SOC 2 dependencies, unclear report scope, weak evidence, unsupported claims, or publication risks.

4. Produce the requested artifact:
   - Use tables for matrices, readiness reviews, evidence lists, and remediation plans.
   - Use concise plain-language prose for public-facing summaries.
   - Include assumptions and review notes.
   - Mark items requiring auditor confirmation.

5. Add practical cautions:
   - SOC 3 wording should be reviewed by the auditor before publication.
   - Public language should not exceed the underlying SOC 2 scope or opinion.
   - If the user does not yet have SOC 2 readiness, recommend strengthening SOC 2 controls first.

## Output Templates

### SOC 3 Readiness Checklist

Use this structure when assessing readiness:

| Area | Readiness Question | Current State | Gap | Risk | Priority | Recommended Action | Owner | Auditor Confirmation Needed |
|---|---|---|---|---|---|---|---|---|
| Scope | Is the SOC 3 scope aligned to the SOC 2 system description and report period? | TBD | Scope not yet confirmed | Public report may overstate assurance coverage | High | Confirm in-scope products, services, locations, criteria, and period with auditor | Compliance | Yes |

### SOC 2-to-SOC 3 Alignment Matrix

Use this structure when translating SOC 2 work into SOC 3-ready summaries:

| SOC 3 Theme | Related SOC 2 Domain | Public Summary | Underlying Control Support | Evidence | Scope Limitation or Caveat | Review Notes |
|---|---|---|---|---|---|---|
| Access Security | Logical Access | Access to production systems is restricted based on job responsibilities and reviewed periodically. | Provisioning, MFA, privileged access, access review, termination controls | IdP exports, access tickets, review sign-offs | Applies to in-scope production systems only | Confirm frequency and product scope before publication |

### Evidence Request List

Use this structure for audit-readiness and evidence collection:

| Request ID | Domain | Evidence Needed | Purpose | Owner | Period Covered | Due Date | Format | Notes |
|---|---|---|---|---|---|---|---|---|
| SOC3-ER-01 | Governance | Final or draft SOC 2 system description and scope | Confirms SOC 3 scope and public report boundaries | Compliance | Report period | TBD | PDF or DOCX | Include products, infrastructure, subservice organizations, and criteria |

### Gap Assessment

Use this structure for readiness reviews:

| Area | Current State | Expected State | Gap | Public Reporting Risk | Priority | Recommended Remediation | Owner | Target Date |
|---|---|---|---|---|---|---|---|---|
| Trust Page Claims | Website states "fully SOC compliant" | Claims align to auditor-reviewed SOC 3 report scope and period | Claim is vague and may overstate assurance | Readers may infer certification or complete security | High | Replace with precise SOC 3 language after auditor approval | Marketing and Compliance | TBD |

### Remediation Roadmap

Use this structure for implementation planning:

| Workstream | Action | Dependency | Owner | Effort | Priority | Target Date | Success Criteria |
|---|---|---|---|---|---|---|---|
| Scope Alignment | Confirm SOC 3 scope with auditor | SOC 2 scope and criteria finalized | Compliance | Medium | High | TBD | Auditor confirms report period, criteria, in-scope system, and publication approach |

### Public-Facing SOC 3 Language Review

Use this structure when reviewing website, sales, or marketing language:

| Statement | Issue | Risk | Safer Alternative | Requires Auditor Review |
|---|---|---|---|---|
| "Our platform is SOC 3 certified." | SOC reports are attestation reports, and "certified" may be misleading depending on auditor guidance. | Overstates assurance and may create customer confusion. | "Our SOC 3 report is available to provide public assurance over the controls relevant to the security of [In-Scope System] for the period [Report Period]." | Yes |

### SOC 3 Narrative Draft

Use this format for summary narrative drafting:

```text
Purpose:
[Explain why the organization obtained or plans to obtain a SOC 3 report.]

Scope:
[Describe the in-scope product, service, system, locations, criteria, and report period.]

Control environment summary:
[Summarize relevant governance, access, change management, operations, data protection, and privacy controls at a high level.]

Public assurance statement:
[Draft conservative language aligned to auditor-reviewed scope.]

Availability:
[Explain whether the report is publicly posted, available on request, or pending auditor release.]

Important limitations:
[List scope limitations, carve-outs, subservice organization dependencies, period limitations, or criteria not covered.]

Auditor review needed:
[List statements or assumptions that must be validated before publication.]
```

## Review Guidance

When reviewing user-provided SOC 3 materials, check for:

- Scope alignment: Does the language match the underlying SOC 2 report period, system, criteria, and auditor opinion?
- Public claim accuracy: Does the statement avoid unsupported guarantees, certifications, or absolute security claims?
- Criteria clarity: Does the material identify which Trust Services Criteria themes are covered without implying unsupported categories?
- Evidence traceability: Can each public assurance theme be traced to underlying controls and evidence?
- Period accuracy: Does the language avoid implying current coverage when the report period is historical?
- Subservice organization clarity: Are relevant vendor or cloud-provider dependencies represented appropriately?
- Distribution readiness: Has the auditor reviewed or approved final public report wording where required?
- Consistency: Do website, sales, security questionnaire, trust center, and report language say the same thing?

## Common Red Flags

Flag these issues when present:

- Calling SOC 3 a "certification" without auditor-approved wording.
- Saying "fully compliant", "guaranteed secure", "unbreachable", or "100% compliant".
- Claiming SOC 3 coverage before the auditor has issued the report.
- Describing products, services, locations, or systems outside the report scope.
- Omitting the report period when using the report as evidence.
- Treating SOC 3 as a substitute for detailed customer due diligence when customers need SOC 2 detail under NDA.
- Publishing trust-center language that conflicts with the SOC 2 system description.
- Mentioning criteria such as Privacy or Availability when they were not included.
- Using outdated report language after a new audit period, scope change, acquisition, or major product change.
- Sharing auditor marks, seals, or report excerpts without confirming usage rules.

## Response Style

Use a professional, audit-ready tone. Be specific, practical, and conservative. Prefer tables for readiness assessments, alignment matrices, gap assessments, evidence requests, and remediation plans. Use concise plain-language prose for public-facing summaries. Clearly label assumptions, limitations, and items requiring auditor confirmation.

When facts are missing, use placeholders such as `TBD`, `[Owner]`, `[System]`, `[Auditor]`, `[Report Period]`, or `[In-Scope System]` rather than fabricating details. When the user provides source materials, cite or reference exact document sections, page numbers, control IDs, ticket IDs, report sections, or evidence names if available.

## Examples

### Example Request

"Create a SOC 3 readiness checklist for our SaaS platform."

### Example Response Outline

1. State assumptions:
   - The organization plans to base SOC 3 on a SOC 2 Type II examination.
   - Security is in scope; other Trust Services Criteria are TBD.
   - The target report period and auditor are not yet provided.

2. Provide readiness table:
   - SOC 2 scope confirmed.
   - Criteria confirmed.
   - System description aligned.
   - Evidence collection complete.
   - Public report language drafted.
   - Auditor review completed.
   - Trust page updated after report issuance.

3. Add cautions:
   - Do not publish SOC 3 claims until the report is issued.
   - Keep public language aligned to auditor-approved scope and period.

### Example Request

"Review this website copy: We are SOC 3 certified and fully compliant with all security standards."

### Example Response Outline

Flag issues:

- "Certified" may be misleading unless approved by the auditor.
- "Fully compliant with all security standards" is too broad and unsupported.
- The statement does not identify the report scope, period, or criteria.

Safer rewrite:

"Our SOC 3 report provides public assurance over selected controls relevant to the security of [In-Scope System] for the period [Report Period]. The report is available at [Location] or upon request, subject to auditor-approved distribution terms."

### Example Request

"Map our SOC 2 controls to SOC 3 themes for a trust center."

### Example Response Outline

1. Confirm SOC 2 report scope and criteria.
2. Group controls into public themes:
   - Governance and risk management.
   - Access security.
   - Change management.
   - System monitoring and availability.
   - Data protection and confidentiality.
   - Privacy, if in scope.
3. Provide a SOC 2-to-SOC 3 alignment matrix with public summaries, evidence support, caveats, and auditor review notes.
