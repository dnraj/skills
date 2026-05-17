---
name: fedramp-compliance-controls
description: "Use when the user asks for FedRAMP compliance support, FedRAMP Moderate or High readiness, NIST SP 800-53 Rev. 5 control mapping, SSPs, POA&Ms, SAP/SAR support, continuous monitoring, 3PAO evidence requests, agency authorization packages, cloud service provider controls, or federal security compliance control guidance for SaaS, cloud, AI, technology, and managed service organizations."
license: MIT
metadata:
  version: '1.0'
---

# FedRAMP Compliance Controls

## When to Use This Skill

Use this skill when the user asks for help with FedRAMP or federal cloud security compliance work, including:

- Mapping policies, procedures, systems, risks, or evidence to FedRAMP and NIST SP 800-53 Rev. 5 controls.
- Preparing FedRAMP Low, Moderate, High, or Tailored readiness materials.
- Creating or reviewing System Security Plans, control implementation statements, responsibility matrices, inheritance descriptions, or customer responsibility language.
- Preparing evidence request lists, audit-readiness plans, remediation trackers, Plan of Action and Milestones entries, or continuous monitoring packages.
- Translating SaaS, cloud, AI, DevSecOps, managed services, security operations, vendor management, incident response, vulnerability management, identity, logging, encryption, and contingency processes into FedRAMP-ready control language.
- Supporting internal readiness for agency authorization, Joint Authorization Board legacy package review, FedRAMP Marketplace positioning, 3PAO assessment preparation, or annual assessment activities.

Do not present work product as legal advice, an official FedRAMP authorization decision, a 3PAO assessment opinion, or a guarantee of authorization. If the user needs official treatment, advise them to validate with their agency Authorizing Official, FedRAMP advisor, 3PAO, counsel, or qualified compliance advisor.

## Core Principles

1. Start by identifying the user's FedRAMP context:
   - Target authorization path: agency authorization, FedRAMP Marketplace listing, reuse package support, or internal readiness.
   - Target baseline: Low, Moderate, High, Tailored, or unknown.
   - Cloud service model: IaaS, PaaS, SaaS, AI service, managed service, or hybrid model.
   - Deployment model and boundary: authorization boundary, cloud regions, tenants, customer environments, third-party services, inherited controls, and external interconnections.
   - Assessment stage: scoping, gap assessment, SSP drafting, evidence collection, 3PAO readiness, assessment fieldwork, POA&M remediation, continuous monitoring, or annual assessment.

2. Anchor recommendations in the FedRAMP control objective and implementation responsibility:
   - What risk is the control mitigating?
   - Which NIST SP 800-53 Rev. 5 family or FedRAMP control area is relevant?
   - Is the control implemented by the cloud service provider, inherited from an underlying provider, shared with customers, or fully customer-responsible?
   - Who owns the control activity?
   - How often does the control operate?
   - What evidence proves the control is designed and operating?
   - What weakness, deficiency, or risk would become a POA&M item?

3. Keep outputs authorization-package ready:
   - Use clear control IDs, implementation status, responsible roles, systems, frequencies, parameters, evidence artifacts, and boundary assumptions.
   - Distinguish control implementation, inherited control coverage, shared responsibility, and customer responsibility.
   - Separate existing controls, gaps, risks, POA&M items, remediation actions, and optional maturity improvements.
   - Avoid unsupported statements such as "FedRAMP compliant" or "authorized" unless the user has provided evidence of official authorization.

4. Treat FedRAMP as both a compliance framework and an operational security program:
   - Favor sustainable controls embedded in normal cloud operations.
   - Emphasize audit trails, configuration exports, vulnerability remediation evidence, incident records, monitoring logs, access review evidence, and change records.
   - Flag ambiguous boundaries, inherited-control assumptions, undocumented shared responsibilities, missing parameter values, weak evidence, and unsupported customer-facing claims.

## FedRAMP Domain Map

Use these common FedRAMP and NIST SP 800-53 control areas to organize work. Map to exact control IDs when the user provides a baseline, an existing control set, or source documentation. If the exact baseline is unknown, identify likely control families and state that exact applicability should be confirmed against the selected FedRAMP baseline.

### Governance, Risk, and Authorization

Typical topics:

- Authorization boundary definition.
- Information system categorization.
- System Security Plan development.
- Policies and procedures.
- Risk assessment and risk treatment.
- Rules of behavior.
- Security planning and governance.
- Shared responsibility and inherited controls.

Common evidence:

- System Security Plan.
- Boundary diagram and data flow diagrams.
- FIPS 199 categorization rationale.
- Policies, standards, and procedures.
- Risk register and risk assessment results.
- Control implementation matrix.
- Customer responsibility matrix.
- Interconnection security agreements or memoranda where applicable.

### Access Control and Identity

Typical topics:

- Account lifecycle management.
- Privileged access.
- Multi-factor authentication.
- Session controls.
- Remote access.
- Separation of duties.
- Periodic access reviews.
- Service accounts.

Common evidence:

- Identity provider configuration.
- User and privileged account exports.
- Access request and approval records.
- Access review evidence and exception tracking.
- MFA configuration screenshots or exports.
- Privileged access management logs.
- Termination and transfer access removal evidence.

### Audit, Logging, and Monitoring

Typical topics:

- Audit event generation.
- Centralized log collection.
- Log review and alerting.
- Time synchronization.
- Security information and event management.
- Continuous monitoring.
- Event correlation and escalation.

Common evidence:

- Logging architecture.
- Audit log configuration exports.
- SIEM rules and alert policies.
- Alert review records.
- Incident tickets generated from alerts.
- Time synchronization settings.
- Continuous monitoring reports.

### Configuration and Change Management

Typical topics:

- Secure baseline configurations.
- Configuration change control.
- Infrastructure-as-code review.
- Production deployment controls.
- Configuration monitoring.
- Unauthorized change detection.
- Component inventory.

Common evidence:

- Configuration management plan.
- Baseline configuration standards.
- Pull requests, change tickets, approvals, and test results.
- CI/CD pipeline logs.
- Asset inventory.
- Configuration scan results.
- Deviation and exception records.

### Vulnerability, Patch, and Malware Protection

Typical topics:

- Vulnerability scanning.
- Patch management.
- Remediation timelines.
- Risk acceptance.
- Container and image scanning.
- Web application scanning.
- Malware protection.

Common evidence:

- Authenticated vulnerability scan reports.
- Remediation tickets and closure evidence.
- Patch deployment reports.
- Risk acceptance approvals.
- Container scan reports.
- Penetration test reports where applicable.
- POA&M entries for unresolved weaknesses.

### Incident Response

Typical topics:

- Incident response planning.
- Incident detection, triage, escalation, containment, eradication, and recovery.
- Federal or agency notification obligations.
- Incident exercises.
- Post-incident lessons learned.

Common evidence:

- Incident response plan.
- Incident tickets and timelines.
- Escalation procedures.
- Tabletop exercise records.
- Lessons-learned reports.
- Security operations runbooks.
- Notification decision records.

### Contingency Planning and Resilience

Typical topics:

- Backup and recovery.
- Business continuity and disaster recovery.
- System recovery objectives.
- Contingency plan testing.
- Availability monitoring.
- Alternate processing and communications where applicable.

Common evidence:

- Contingency plan.
- Backup configuration and job reports.
- Restore test evidence.
- Disaster recovery test results.
- Availability reports.
- Recovery objective documentation.
- Lessons learned and remediation tracking.

### System and Communications Protection

Typical topics:

- Encryption in transit and at rest.
- Boundary protection.
- Network segmentation.
- Key management.
- DNS, firewall, and security group controls.
- Secure APIs and interconnections.
- Federal cryptographic requirements where applicable.

Common evidence:

- Network diagrams.
- Firewall, security group, and routing exports.
- TLS configuration evidence.
- Encryption and key management configuration.
- Certificate inventory.
- Interconnection documentation.
- API gateway and WAF settings.

### Supply Chain, Vendor, and External Service Management

Typical topics:

- External service dependencies.
- Subcontractors and vendors.
- Supply chain risk management.
- External system services.
- Inherited controls from underlying cloud providers.
- Customer and third-party interconnections.

Common evidence:

- Vendor inventory and risk ratings.
- Supplier security reviews.
- FedRAMP package inheritance documentation.
- External service agreements.
- Data processing and service commitments.
- Interconnection diagrams.
- Vendor monitoring records.

### Personnel Security and Awareness

Typical topics:

- Screening and onboarding.
- Security awareness training.
- Role-based training.
- Rules of behavior.
- Termination and transfer procedures.
- Personnel sanctions.

Common evidence:

- Training completion records.
- Signed rules of behavior.
- Onboarding and offboarding checklists.
- Background screening evidence where lawful and applicable.
- Role-based training records.
- HRIS termination records.

## Standard Workflow

Follow this workflow for most FedRAMP requests:

1. Clarify scope if necessary:
   - Ask only for missing details that materially change the output.
   - If the user needs a quick draft, make reasonable assumptions and label them clearly.
   - Prioritize clarifying target baseline, authorization boundary, cloud service model, deployment environment, and whether the organization is pursuing agency authorization or readiness only.

2. Identify relevant control families and artifacts:
   - Map the request to one or more FedRAMP and NIST SP 800-53 control areas.
   - Note likely artifacts such as SSP, POA&M, security assessment plan, security assessment report, inventory, policies, diagrams, or continuous monitoring deliverables.
   - Avoid inventing exact control IDs if the user's baseline or control set is unavailable.

3. Assess current state:
   - Extract stated controls, systems, services, owners, frequencies, boundary assumptions, inherited controls, and available evidence.
   - Distinguish documented process from actual operating practice.
   - Identify gaps in design, implementation, evidence, ownership, parameterization, inheritance, and customer responsibility language.

4. Produce the requested artifact:
   - Control matrix.
   - SSP control implementation statement.
   - Customer responsibility matrix.
   - Evidence request list.
   - Gap assessment.
   - POA&M tracker.
   - Remediation roadmap.
   - Continuous monitoring checklist.
   - 3PAO readiness package.
   - Audit response or evidence narrative.

5. Add practical cautions:
   - Call out assumptions.
   - Identify dependencies on the selected baseline, agency expectations, FedRAMP PMO guidance, and 3PAO interpretation.
   - Recommend validation with the agency Authorizing Official, 3PAO, or FedRAMP advisor for final authorization-package treatment.

## Output Templates

### FedRAMP Control Matrix

Use this structure when creating or revising controls:

| Control ID | Family | Control Objective | Implementation Statement | Responsibility | Owner | Frequency | Evidence | Systems | Design Notes | Assessment Notes |
|---|---|---|---|---|---|---|---|---|---|---|
| AC-XX | Access Control | Ensure only authorized users access in-scope systems | [Role] approves access requests before provisioning in [System], and access is reviewed [Frequency] | CSP / Inherited / Shared / Customer | Security | Per request and quarterly | Access ticket, approval, user export, review sign-off | IdP, production environment | Confirm scope covers all in-boundary systems | Test samples for provisioning, termination, and review operation |

### SSP Control Implementation Statement

Use this format for System Security Plan-ready narratives:

```text
Control:
[Control ID and title if known]

Implementation status:
[Implemented / Partially implemented / Planned / Not applicable, if supported]

Implementation statement:
[Describe how the control is implemented inside the authorization boundary. Include who performs the activity, what system or process is used, frequency, where evidence is retained, and how exceptions are handled.]

Responsibility:
[CSP / inherited from provider / shared with customer / customer responsibility]

Inherited or shared controls:
[Identify inherited provider, inherited capability, shared responsibility, or customer action required.]

Parameters and assumptions:
[List FedRAMP-defined or organization-defined parameters, boundary assumptions, and dependencies.]

Evidence:
[List evidence artifacts.]

Open risks or POA&M items:
[List known gaps, weaknesses, or planned remediation.]
```

### Evidence Request List

Use this structure for readiness, 3PAO preparation, and evidence collection:

| Request ID | Control Family | Evidence Needed | Purpose | Owner | Period Covered | Due Date | Format | Notes |
|---|---|---|---|---|---|---|---|---|
| ER-01 | Access Control | Current user listing for in-scope production systems | Supports account management and access review testing | IT or Security | Assessment period | TBD | CSV export | Include user, role, status, creation date, last login, and privileged flag if available |

### Gap Assessment

Use this structure for readiness reviews:

| Area | Current State | Expected FedRAMP-Ready Control | Gap | Risk | Priority | Recommended Remediation | Owner | Target Date |
|---|---|---|---|---|---|---|---|---|
| Vulnerability Management | Scans are run but remediation timelines are informal | Authenticated scans are performed on defined cadence and findings are tracked to remediation or approved risk acceptance | No documented remediation SLA or POA&M linkage | Unresolved weaknesses may remain unmanaged | High | Define severity-based remediation timelines, ticket workflow, and POA&M escalation criteria | Security | TBD |

### POA&M Tracker

Use this structure for weaknesses, risks, and remediation planning:

| POA&M ID | Control ID | Weakness Description | Source | Risk Level | Remediation Plan | Milestones | Owner | Scheduled Completion Date | Status | Evidence of Closure |
|---|---|---|---|---|---|---|---|---|---|---|
| POAM-001 | RA-XX | [Weakness] | Readiness assessment | High | [Action plan] | [Milestone list] | [Owner] | TBD | Open | TBD |

### Customer Responsibility Matrix

Use this structure when clarifying shared controls:

| Control Area | CSP Responsibility | Customer Responsibility | Inherited Provider Responsibility | Evidence Available from CSP | Customer Evidence Needed | Notes |
|---|---|---|---|---|---|---|
| Access Management | Provides role-based access controls and audit logging | Configures users, roles, MFA, and periodic access reviews | Provides underlying identity or infrastructure controls if applicable | Configuration exports, logs, access review templates | Customer user list, approvals, review sign-offs | Confirm whether customer-managed admins are inside the authorization boundary |

### Continuous Monitoring Checklist

Use this structure for ongoing FedRAMP operations:

| Activity | Frequency | Owner | Evidence | Related Artifact | Exception Handling |
|---|---|---|---|---|---|
| Vulnerability scan review | Monthly or per program requirement | Security | Scan report, remediation tickets, POA&M updates | Continuous monitoring package | Findings breaching timelines are added to POA&M or risk accepted |

## Review Guidance

When reviewing user-provided FedRAMP controls, SSP sections, or evidence, check for:

- Boundary clarity: Does the statement clearly describe what is inside and outside the authorization boundary?
- Responsibility clarity: Is the control CSP-owned, inherited, shared, or customer-responsible?
- Implementation specificity: Can a 3PAO understand who does what, when, where, and using which system?
- Parameter handling: Are FedRAMP or organization-defined parameters identified rather than ignored?
- Evidence quality: Is evidence complete, dated, attributable, exportable, and retained?
- Population clarity: Can the full population be identified for sampling?
- Operating consistency: Does the process operate at the stated frequency?
- Inheritance support: Are inherited controls tied to a real underlying provider capability or package rather than assumed?
- Exception tracking: Are deviations documented, risk-ranked, remediated, or placed on the POA&M?
- Customer-facing accuracy: Does the language avoid overstating authorization, compliance, or inherited coverage?

## Common Red Flags

Flag these issues when present:

- The authorization boundary is vague or inconsistent across diagrams, SSP text, inventory, and data flows.
- The control says "inherited" but does not identify the inherited provider or inherited capability.
- The organization claims FedRAMP compliance without an authorization status or clearly limited readiness context.
- The SSP describes policy intent but not actual implementation.
- Control statements omit owner, frequency, system, evidence, or exception handling.
- Evidence is screenshot-only where an export or full population would be expected.
- Vulnerability findings are tracked in scanner dashboards but not tied to tickets, remediation timelines, risk acceptance, or POA&M entries.
- Privileged access is not separately identified, approved, reviewed, and monitored.
- Continuous monitoring activities are described but not evidenced.
- Inventory, diagrams, ports, protocols, services, and scan scope do not reconcile.
- Customer responsibilities are buried in contract terms rather than clearly stated in security documentation.
- Third-party services process federal data but are not reflected in the boundary, inventory, or supply chain review.

## Response Style

Use a professional, federal audit-ready tone. Be specific, practical, and direct. Prefer tables for matrices, gap assessments, evidence requests, POA&M trackers, and remediation plans. Use bullets for observations and recommendations. Clearly label assumptions and do not overstate assurance.

When facts are missing, use placeholders such as `TBD`, `[Owner]`, `[System]`, `[Cloud Provider]`, `[Agency]`, or `[3PAO]` rather than fabricating details. When the user provides source materials, cite or reference the exact document sections, page numbers, control IDs, ticket IDs, evidence names, diagram names, or artifact versions if available.

## Examples

### Example Request

"Create a FedRAMP Moderate evidence request list for access management."

### Example Response Outline

1. State assumptions:
   - FedRAMP Moderate baseline is targeted.
   - The in-scope system is a SaaS production environment.
   - Identity provider, production application, cloud console, ticketing system, and HRIS are in scope unless excluded.

2. Provide evidence table:
   - Current user listing.
   - Privileged account listing.
   - New user provisioning tickets.
   - Termination access removal records.
   - Periodic access review evidence.
   - MFA configuration.
   - Service account inventory.
   - Remote access configuration where applicable.

3. Add collection notes:
   - Provide exports rather than screenshots where possible.
   - Preserve timestamps, approver identity, reviewer sign-off, and full population completeness.
   - Reconcile HR terminations to access removals and identify exceptions.

### Example Request

"Review this SSP statement and make it FedRAMP-ready: We use AWS controls for encryption and our app encrypts data."

### Example Response Outline

Rewrite:

"Data within the authorization boundary is encrypted in transit using TLS for external and internal application communications, and data at rest is encrypted using [Service/Database] encryption with keys managed through [Key Management System]. Underlying physical and infrastructure encryption controls are inherited from [Cloud Provider] where applicable. The Security team reviews encryption configuration at least [Frequency] and upon material architecture changes. Evidence retained includes TLS configuration exports, storage encryption configuration, key management settings, architecture diagrams, and review records. Customer-managed encryption responsibilities, if any, are documented in the Customer Responsibility Matrix."

Notes:

- Identify the specific encryption mechanisms and systems.
- Separate inherited provider controls from application-level controls.
- Include frequency, owner, evidence, and boundary assumptions.
- Confirm whether federal cryptographic requirements apply to the service and data type.
