---
name: soc2-compliance-controls
description: "Use when the user asks for SOC 2 compliance support, control mapping, trust services criteria analysis, evidence request lists, audit readiness, gap assessments, control narratives, policy-to-control alignment, or security compliance controls for SaaS, cloud, or technology organizations."
license: MIT
metadata:
  version: '1.0'
---

# SOC 2 Compliance Controls

## When to Use This Skill

Use this skill when the user asks for help with SOC 2 or security compliance work, including:

- Mapping policies, procedures, risks, systems, or evidence to SOC 2 controls.
- Creating or reviewing SOC 2 control descriptions, control matrices, or narratives.
- Preparing audit-readiness plans, evidence request lists, or remediation trackers.
- Performing gap assessments against SOC 2 Trust Services Criteria.
- Translating operational practices into auditor-friendly control language.
- Aligning SaaS, cloud, IT, security, HR, vendor, incident, change, access, availability, confidentiality, or privacy processes to SOC 2 expectations.

Do not present work product as legal, accounting, or audit attestation advice. If the user needs an official audit opinion, advise them to consult their CPA firm, auditor, counsel, or qualified compliance advisor.

## Core Principles

1. Start by identifying the user's SOC 2 context:
   - Type I or Type II.
   - Target report period.
   - In-scope products, systems, infrastructure, teams, locations, and vendors.
   - Applicable Trust Services Criteria: Security is always included; Availability, Confidentiality, Processing Integrity, and Privacy may also apply.
   - Audit stage: scoping, readiness, evidence collection, fieldwork, remediation, or report review.

2. Anchor recommendations in practical control objectives rather than abstract compliance language:
   - What risk is the control mitigating?
   - Who performs it?
   - How often does it operate?
   - What evidence proves it operated?
   - What exception would indicate failure?
   - Who reviews exceptions and how are they remediated?

3. Keep outputs auditor-ready:
   - Use clear control owner, frequency, evidence, system, and population fields.
   - Distinguish control design from operating effectiveness.
   - Separate existing controls, gaps, remediation actions, and optional enhancements.
   - Avoid unsupported claims such as "compliant" unless evidence has been reviewed.

4. Treat SOC 2 as a risk and operations framework:
   - Favor controls that are sustainable and embedded in normal workflows.
   - Note where manual controls may need stronger evidence or review trails.
   - Flag ambiguous ownership, missing documentation, untested processes, or weak evidence.

## SOC 2 Domain Map

Use these common control domains to organize work. Map to the applicable Trust Services Criteria when needed, but avoid inventing exact criterion references if uncertain.

### Governance and Risk Management

Typical topics:

- Control environment and oversight.
- Risk assessment process.
- Information security governance.
- Policy management and annual review.
- Vendor risk management.
- Compliance monitoring.

Common evidence:

- Security policies and standards.
- Risk register and risk assessment results.
- Board or management meeting minutes.
- Vendor inventory, risk ratings, reviews, and security documentation.
- Policy approval and review history.

### Logical Access

Typical topics:

- User provisioning.
- Access approvals.
- Role-based access.
- Privileged access.
- Multi-factor authentication.
- Periodic access reviews.
- Termination and transfer access removal.

Common evidence:

- User access tickets.
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
- Emergency changes.
- Change monitoring.

Common evidence:

- Pull requests and approvals.
- CI/CD pipeline logs.
- Test results.
- Deployment records.
- Change tickets.
- Emergency change documentation.

### System Operations and Monitoring

Typical topics:

- Infrastructure monitoring.
- Logging and alerting.
- Backup and recovery.
- Vulnerability management.
- Incident detection and response.
- Capacity and availability monitoring.

Common evidence:

- Monitoring dashboards.
- Alert policies and incident tickets.
- Backup job reports and restore tests.
- Vulnerability scans and remediation records.
- Incident response plan and postmortems.
- Uptime reports.

### Data Protection and Confidentiality

Typical topics:

- Data classification.
- Encryption in transit and at rest.
- Key management.
- Data retention and deletion.
- Secure data handling.
- Customer data segregation.

Common evidence:

- Data classification policy.
- Encryption configuration screenshots or exports.
- Key management policy and access records.
- Retention schedule.
- Data deletion tickets.
- Architecture diagrams.

### Privacy

Use this domain only when Privacy is in scope or the user asks about personal information handling.

Typical topics:

- Privacy notice alignment.
- Data subject request process.
- Consent or legal basis tracking.
- Personal data inventory.
- Subprocessor disclosure.
- Privacy incident handling.

Common evidence:

- Privacy policy.
- Data inventory or records of processing.
- DSR tickets and response logs.
- Consent records where applicable.
- Subprocessor list.
- Privacy training materials.

### Human Resources and Training

Typical topics:

- Background checks where lawful and applicable.
- Security awareness training.
- Confidentiality agreements.
- Onboarding and offboarding.
- Role changes.
- Disciplinary process.

Common evidence:

- Training completion reports.
- Signed employee agreements.
- HRIS onboarding and termination records.
- Background check completion records.
- Offboarding checklist.

## Standard Workflow

Follow this workflow for most SOC 2 requests:

1. Clarify scope if necessary:
   - Ask only for missing details that materially change the output.
   - If the user needs a quick draft, make reasonable assumptions and state them.

2. Identify the relevant control domains:
   - Map the user's request to one or more domains from the SOC 2 Domain Map.
   - Note likely Trust Services Criteria categories if helpful.

3. Assess current state:
   - Extract stated controls, systems, owners, frequencies, and available evidence.
   - Distinguish documented process from actual operating practice.
   - Flag missing evidence, unclear owners, weak review trails, or inconsistent timing.

4. Produce the requested artifact:
   - Control matrix.
   - Evidence request list.
   - Gap assessment.
   - Remediation roadmap.
   - Control narrative.
   - Audit response.
   - Policy-to-control mapping.

5. Add practical cautions:
   - Call out assumptions.
   - Identify dependencies on auditor expectations.
   - Recommend validation with the user's auditor for final report treatment.

## Output Templates

### Control Matrix

Use this structure when creating or revising controls:

| Control ID | Domain | Control Objective | Control Activity | Owner | Frequency | Evidence | Systems | Design Notes | Operating Effectiveness Notes |
|---|---|---|---|---|---|---|---|---|---|
| SOC2-XX-01 | Access | Ensure only authorized users have access to production systems | Access requests are approved by the system owner before provisioning | IT or Security | Per request | Access ticket, approval record, user list | IdP, production system | Confirm approval happens before access is granted | Test sample of new users during the period |

### Evidence Request List

Use this structure for audit-readiness and evidence collection:

| Request ID | Domain | Evidence Needed | Purpose | Owner | Period Covered | Due Date | Format | Notes |
|---|---|---|---|---|---|---|---|---|
| ER-01 | Access | User access listing for production systems | Supports access review and provisioning controls | IT | Audit period | TBD | CSV export | Include user, role, status, creation date, and last login if available |

### Gap Assessment

Use this structure for readiness reviews:

| Area | Current State | Expected Control | Gap | Risk | Priority | Recommended Remediation | Owner | Target Date |
|---|---|---|---|---|---|---|---|---|
| Access Reviews | Reviews occur informally | Formal periodic review with evidence of reviewer, date, population, and actions | No documented sign-off | Unauthorized access may persist | High | Implement quarterly access review workflow and retain exports/sign-offs | Security | TBD |

### Remediation Roadmap

Use this structure for implementation planning:

| Workstream | Action | Dependency | Owner | Effort | Priority | Target Date | Success Criteria |
|---|---|---|---|---|---|---|---|
| Access | Implement quarterly production access reviews | Complete user inventory | Security | Medium | High | TBD | Review completed, exceptions tracked, evidence retained |

### Control Narrative

Use this format for auditor-friendly control descriptions:

```text
Control objective:
[Describe the risk or objective.]

Control activity:
[Describe who performs the control, what they do, how often, where it is documented, and what evidence is retained.]

Systems and data in scope:
[List relevant systems, repositories, environments, or datasets.]

Control owner:
[Role or team.]

Frequency:
[Per occurrence, daily, weekly, monthly, quarterly, annually.]

Evidence:
[List evidence artifacts.]

Exceptions and remediation:
[Describe how exceptions are identified, tracked, approved, and resolved.]

Assumptions:
[List assumptions or dependencies.]
```

## Review Guidance

When reviewing user-provided controls or evidence, check for:

- Completeness: Does the control include owner, frequency, scope, evidence, and exception handling?
- Precision: Is the control specific enough to test?
- Consistency: Does the control align with policies, tickets, system settings, and actual workflow?
- Evidence quality: Is evidence complete, dated, attributable, and retained?
- Population clarity: Can the auditor determine the full population for sampling?
- Timing: Does the control operate at the promised frequency throughout the report period?
- Segregation of duties: Are request, approval, implementation, and review responsibilities appropriately separated?
- Exception tracking: Are deviations documented, risk-assessed, and remediated?

## Common Red Flags

Flag these issues when present:

- Control says "all" but evidence only covers a subset.
- Control owner is a team mailbox or tool rather than an accountable role.
- Reviews are performed but not dated, signed off, or linked to the population reviewed.
- Access is granted before approval.
- Terminated users are removed manually with no SLA or evidence trail.
- Change approvals happen after deployment.
- Vulnerability remediation timelines exist in policy but are not tracked.
- Backups run but restore tests are not performed.
- Vendors are listed but not risk-ranked or reviewed.
- Policies exist but have no approval, review date, or owner.
- Monitoring alerts exist but incident response procedures are not tested.

## Response Style

Use a professional, audit-ready tone. Be specific, practical, and direct. Prefer tables for matrices, gap assessments, evidence requests, and remediation plans. Use bullets for observations and recommendations. Clearly label assumptions and avoid overstating assurance.

When facts are missing, use placeholders such as `TBD`, `[Owner]`, or `[System]` rather than fabricating details. When the user provides source materials, cite or reference the exact document sections, page numbers, control IDs, ticket IDs, or evidence names if available.

## Examples

### Example Request

"Create a SOC 2 evidence request list for access management."

### Example Response Outline

1. State assumptions:
   - Security criteria are in scope.
   - Production systems, identity provider, HRIS, and ticketing system are in scope.
   - Audit period is not yet provided.

2. Provide evidence table:
   - User access listing.
   - New user provisioning tickets.
   - Termination records.
   - Quarterly access review evidence.
   - MFA configuration.
   - Privileged access listing.

3. Add collection notes:
   - Include full population exports, not screenshots only.
   - Preserve timestamps and approver identity.
   - Reconcile HR terminations to access removals.

### Example Request

"Review this access control and make it auditor-ready: We review access sometimes and remove people who should not have access."

### Example Response Outline

Rewrite:

"On a quarterly basis, the Security team exports the active user listing for in-scope production systems from [System]. The system owner reviews each user's role and business need, documents approval or removal decisions in [Ticketing System], and tracks exceptions through remediation. Evidence retained includes the user listing, reviewer sign-off, exception log, and completion ticket."

Notes:

- Replace "sometimes" with a defined frequency.
- Identify the reviewer and system owner.
- Define evidence and exception handling.
- Confirm whether the review covers all in-scope production systems.
