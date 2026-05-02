---
name: iso-42001-compliance-controls
description: "Use when the user asks for ISO/IEC 42001, ISO 42001, AI management system, AIMS, responsible AI governance, AI compliance controls, AI risk management, AI impact assessment, AI lifecycle controls, audit readiness, evidence requests, gap assessments, or control mapping for organizations that develop, provide, procure, or use AI systems."
license: MIT
metadata:
  version: '1.0'
---

# ISO/IEC 42001 Compliance Controls

## When to Use This Skill

Use this skill when the user asks for help with ISO/IEC 42001 or AI management system compliance work, including:

- Creating or reviewing AI management system controls.
- Mapping AI governance practices to ISO/IEC 42001-style requirements.
- Preparing AI compliance control matrices, evidence requests, readiness assessments, or remediation plans.
- Assessing responsible AI governance, AI lifecycle controls, AI risk management, or AI impact assessment practices.
- Translating AI policies, procedures, model development practices, procurement workflows, monitoring processes, and oversight activities into audit-ready controls.
- Supporting organizations that develop, provide, procure, deploy, operate, or use AI systems.

Do not present work product as legal, certification, audit, or accreditation advice. If the user needs a formal certification decision, official interpretation, or audit opinion, advise them to consult their certification body, auditor, counsel, or qualified compliance advisor.

## Core Principles

1. Treat ISO/IEC 42001 as an AI management system framework:
   - Focus on governance, accountability, policies, planning, operational controls, performance evaluation, and continual improvement.
   - Address both AI risks and opportunities.
   - Consider the full AI system lifecycle, including design, development, procurement, deployment, operation, monitoring, change, retirement, and third-party use.

2. Start by identifying the user's AI context:
   - Whether the organization develops, provides, procures, deploys, or uses AI systems.
   - In-scope AI products, models, services, workflows, datasets, vendors, teams, and business processes.
   - Applicable AI use cases, risk tiers, affected stakeholders, and regulatory or customer obligations.
   - Target readiness stage: scoping, implementation, gap assessment, evidence collection, internal audit, management review, certification audit, or remediation.

3. Make controls specific and testable:
   - What AI risk or obligation is addressed?
   - Who owns the control?
   - When or how often does it operate?
   - Which AI systems, datasets, vendors, or business units are in scope?
   - What evidence demonstrates operation?
   - How are exceptions, incidents, model changes, or risk acceptances approved and tracked?

4. Separate design from operating effectiveness:
   - Design asks whether the control is appropriately defined to meet the objective.
   - Operating effectiveness asks whether the control operated as designed over the period.
   - Do not claim conformance unless sufficient evidence has been reviewed.

5. Preserve human accountability:
   - Assign control ownership to roles or teams, not only tools.
   - Identify required approvals, escalation paths, human oversight, and decision rights.
   - Flag automated controls that lack monitoring, exception handling, or accountable review.

## ISO/IEC 42001 Control Domain Map

Use these practical domains to organize 42001 compliance work. These domains are designed for control mapping and audit readiness. Avoid inventing exact clause numbers unless the user provides the standard text or a confirmed control framework.

### AI Governance and Accountability

Typical topics:

- AI policy and objectives.
- AI governance structure.
- Roles, responsibilities, and decision rights.
- Accountability for AI system outcomes.
- Management oversight and reporting.
- Stakeholder expectations.
- Alignment with business, legal, ethical, and risk objectives.

Common evidence:

- AI policy and governance charter.
- RACI matrix for AI responsibilities.
- AI steering committee agendas and minutes.
- AI objectives and key performance indicators.
- AI risk acceptance records.
- Governance reports to senior management.

### AI System Inventory and Scope

Typical topics:

- Inventory of AI systems and AI-enabled features.
- Classification of AI systems by use case, risk, owner, lifecycle stage, and business process.
- Identification of internally developed, third-party, embedded, and open-source AI components.
- Scope definition for the AI management system.

Common evidence:

- AI system inventory.
- AI use case register.
- Model cards or system cards.
- Data flow diagrams.
- Architecture diagrams.
- Vendor and third-party AI inventory.
- Scope statement for the AI management system.

### AI Risk Management

Typical topics:

- AI risk methodology.
- Risk identification, analysis, evaluation, treatment, and acceptance.
- Risk criteria and risk appetite.
- Risk reviews at lifecycle gates.
- Risk ownership and escalation.
- Periodic reassessment.

Common evidence:

- AI risk management procedure.
- AI risk register.
- Risk assessment templates.
- Completed risk assessments.
- Risk treatment plans.
- Risk acceptance approvals.
- Periodic risk review records.

### AI Impact Assessment

Typical topics:

- Assessment of potential impacts on individuals, groups, organizations, society, rights, safety, privacy, security, fairness, transparency, and reliability.
- Intended and reasonably foreseeable misuse.
- Stakeholder impact analysis.
- Benefit and harm evaluation.
- Mitigation planning.

Common evidence:

- AI impact assessment procedure.
- Completed AI impact assessments.
- Stakeholder consultation records.
- Bias, fairness, privacy, safety, or human rights assessments.
- Mitigation tracking.
- Approval records before deployment.

### Data Governance for AI

Typical topics:

- Dataset sourcing and authorization.
- Data quality, lineage, representativeness, labeling, retention, and deletion.
- Sensitive data handling.
- Training, validation, testing, and production data separation.
- Data rights, licensing, and consent where applicable.
- Data drift monitoring.

Common evidence:

- Dataset inventory.
- Data lineage records.
- Data quality checks.
- Data labeling guidance.
- Data retention and deletion records.
- Data protection impact assessments where applicable.
- Dataset approval records.

### AI Development and Lifecycle Management

Typical topics:

- Requirements definition.
- Design review.
- Model selection and development.
- Testing and validation.
- Documentation.
- Release approval.
- Change management.
- Decommissioning.

Common evidence:

- AI lifecycle policy or standard.
- Product requirements and design documents.
- Model development documentation.
- Test plans and results.
- Validation reports.
- Release approvals.
- Change tickets.
- Decommissioning records.

### AI Evaluation, Testing, and Validation

Typical topics:

- Performance testing.
- Robustness, reliability, and safety testing.
- Bias and fairness testing.
- Explainability or interpretability assessment.
- Security testing.
- Red-teaming or abuse testing where appropriate.
- User acceptance testing.

Common evidence:

- Evaluation plan.
- Test cases and results.
- Benchmark reports.
- Bias and fairness analysis.
- Red-team findings and remediation.
- Validation sign-off.
- Acceptance criteria.

### Human Oversight and Use Controls

Typical topics:

- Human-in-the-loop, human-on-the-loop, or human-over-the-loop oversight.
- User instructions and limitations.
- Escalation and override procedures.
- Monitoring of high-impact decisions.
- Training for users and operators.
- Controls over prohibited or restricted uses.

Common evidence:

- Human oversight procedure.
- User guidance.
- Training completion records.
- Decision review logs.
- Override records.
- Escalation tickets.
- Restricted-use approval records.

### Transparency, Documentation, and Communication

Typical topics:

- AI system documentation.
- Notices to users or affected stakeholders.
- Disclosures about AI use.
- Explainability expectations.
- Limitations and known issues.
- External communications and customer documentation.

Common evidence:

- Model cards, system cards, or fact sheets.
- User notices.
- Customer documentation.
- Release notes.
- Known limitations documentation.
- Explainability assessment.
- Communication approval records.

### Security, Privacy, and Resilience

Typical topics:

- Security controls specific to AI systems.
- Prompt injection, model extraction, data leakage, poisoning, adversarial attacks, and abuse prevention.
- Privacy-by-design.
- Access control to models, datasets, prompts, logs, and evaluation results.
- Backup, recovery, continuity, and resilience.

Common evidence:

- Threat model.
- Security review.
- Access control records.
- Privacy assessment.
- AI incident response playbook.
- Abuse monitoring records.
- Backup and recovery test records.

### Third-Party and Supplier AI Management

Typical topics:

- Vendor due diligence for AI systems.
- Contractual obligations and acceptable use.
- Monitoring of third-party AI performance, risk, and changes.
- Supplier risk ratings.
- Open-source model or component governance.

Common evidence:

- AI vendor inventory.
- Vendor risk assessments.
- Security and compliance documentation.
- Contract terms and data processing terms.
- Model or component licensing review.
- Vendor monitoring records.
- Supplier issue logs.

### AI Operations, Monitoring, and Incident Management

Typical topics:

- Production monitoring.
- Model drift, data drift, and performance degradation.
- User feedback and complaint handling.
- AI incidents and near misses.
- Post-deployment review.
- Corrective and preventive action.

Common evidence:

- Monitoring dashboards.
- Drift reports.
- Incident tickets.
- User feedback logs.
- Post-incident reviews.
- Corrective action plans.
- Periodic performance reports.

### Competence, Awareness, and Training

Typical topics:

- Role-based AI training.
- Responsible AI awareness.
- Competence requirements for AI developers, reviewers, operators, and governance stakeholders.
- Training for users of AI-enabled tools.

Common evidence:

- Training matrix.
- Training materials.
- Completion reports.
- Role descriptions.
- Competency assessments.
- Onboarding records.

### Performance Evaluation and Continual Improvement

Typical topics:

- Internal audits.
- Metrics and objectives.
- Management review.
- Corrective actions.
- Continual improvement process.
- Monitoring of AI management system effectiveness.

Common evidence:

- Internal audit plan and reports.
- Management review minutes.
- AI objectives and metrics.
- Nonconformity and corrective action records.
- Improvement backlog.
- Control testing results.

## Standard Workflow

Follow this workflow for most ISO/IEC 42001 requests:

1. Clarify scope only when needed:
   - Ask whether the user develops, provides, procures, deploys, or uses AI if that changes the output.
   - Ask for in-scope AI systems, target readiness stage, and applicable risk profile when necessary.
   - If the user wants a quick draft, state assumptions and proceed.

2. Identify relevant domains:
   - Map the user's request to one or more domains in the control domain map.
   - Identify related evidence, owners, and lifecycle checkpoints.

3. Assess current state:
   - Extract stated practices, policies, controls, systems, roles, approvals, and evidence.
   - Distinguish aspirational policy language from operating practices.
   - Identify missing ownership, weak evidence, unclear scope, untested assumptions, and incomplete risk treatment.

4. Produce the requested artifact:
   - Control matrix.
   - Evidence request list.
   - Gap assessment.
   - Readiness roadmap.
   - AI risk register.
   - AI impact assessment template.
   - AI governance RACI.
   - Audit response.
   - Policy-to-control mapping.

5. Add caveats and next steps:
   - List assumptions.
   - Flag where auditor or certification-body expectations may vary.
   - Recommend validation against the organization's actual ISO/IEC 42001 clause mapping and purchased standard text.

## Output Templates

### Control Matrix

Use this structure when creating or revising controls:

| Control ID | Domain | Control Objective | Control Activity | Owner | Frequency | Scope | Evidence | Design Notes | Operating Effectiveness Notes |
|---|---|---|---|---|---|---|---|---|---|
| AIMS-XX-01 | AI Risk Management | Ensure AI risks are identified and treated before deployment | For each in-scope AI system, the AI owner completes an AI risk assessment before production release. Identified risks are assigned treatment actions, risk owners, and approval status. | AI Governance Lead | Per AI system or material change | In-scope AI systems | Completed risk assessment, treatment plan, approval record | Confirm risk criteria and approval thresholds are defined | Test sample of releases and material changes |

### Evidence Request List

Use this structure for audit-readiness and evidence collection:

| Request ID | Domain | Evidence Needed | Purpose | Owner | Period Covered | Due Date | Format | Notes |
|---|---|---|---|---|---|---|---|---|
| ER-01 | AI System Inventory | Current inventory of AI systems and AI-enabled features | Confirms AIMS scope and control population | AI Governance or Product | Audit period | TBD | Spreadsheet or system export | Include owner, business use, lifecycle stage, risk tier, vendor, data types, and deployment status |

### Gap Assessment

Use this structure for readiness reviews:

| Area | Current State | Expected Control | Gap | Risk | Priority | Recommended Remediation | Owner | Target Date |
|---|---|---|---|---|---|---|---|---|
| AI Inventory | Teams track AI use cases informally | Central inventory of in-scope AI systems with owner, risk tier, lifecycle stage, and review status | No complete control population | AI systems may bypass governance | High | Implement AI system inventory intake and periodic attestation | AI Governance Lead | TBD |

### Readiness Roadmap

Use this structure for implementation planning:

| Workstream | Action | Dependency | Owner | Effort | Priority | Target Date | Success Criteria |
|---|---|---|---|---|---|---|---|
| Governance | Approve AI policy and governance charter | Executive sponsor identified | Legal, Security, Product, AI Governance | Medium | High | TBD | Policy approved, roles assigned, review cadence established |

### AI Risk Register

Use this structure for risk management artifacts:

| Risk ID | AI System | Risk Scenario | Impacted Stakeholders | Likelihood | Impact | Risk Rating | Treatment | Owner | Status | Evidence |
|---|---|---|---|---|---|---|---|---|---|---|
| AIR-01 | [System] | Model output may produce inaccurate recommendation used in business workflow | Customers, users, operations team | TBD | TBD | TBD | Human review for high-impact recommendations; monitoring and feedback loop | Product Owner | Open | Risk assessment, control design, monitoring report |

### AI Impact Assessment

Use this structure for impact assessment work:

| Section | Questions to Answer | Evidence or Input |
|---|---|---|
| Use Case | What is the AI system intended to do, and what decisions or actions does it support? | Product requirements, user documentation |
| Stakeholders | Who may be affected directly or indirectly? | Stakeholder map, user groups |
| Data | What data is used for training, evaluation, prompting, or operation? | Dataset inventory, data lineage |
| Risks and Impacts | What harms, misuse, bias, privacy, safety, security, or reliability issues are reasonably foreseeable? | Risk assessment, testing results |
| Mitigations | What controls reduce likelihood or impact? | Control matrix, treatment plan |
| Oversight | What human review, escalation, or override exists? | Oversight procedure, decision logs |
| Approval | Who approves deployment or continued operation? | Approval record |

### Control Narrative

Use this format for auditor-friendly control descriptions:

```text
Control objective:
[Describe the AI governance, risk, lifecycle, data, oversight, transparency, security, or monitoring objective.]

Control activity:
[Describe who performs the control, what they do, when it occurs, which AI systems are in scope, where it is documented, and what evidence is retained.]

AI systems and lifecycle stage in scope:
[List systems, model types, use cases, environments, or lifecycle stages.]

Control owner:
[Role or team.]

Frequency:
[Per AI system, per release, per material change, continuous, monthly, quarterly, annually.]

Evidence:
[List evidence artifacts.]

Exceptions and remediation:
[Describe how exceptions, incidents, risk acceptances, model issues, or control failures are identified, approved, tracked, and resolved.]

Assumptions:
[List assumptions or dependencies.]
```

## Review Guidance

When reviewing user-provided AI controls or evidence, check for:

- Scope clarity: Does the control identify which AI systems, use cases, vendors, data, or lifecycle stages are covered?
- Ownership: Is an accountable owner assigned?
- Trigger and frequency: Does the control operate at defined lifecycle gates or intervals?
- Evidence: Is evidence complete, dated, attributable, retained, and tied to the relevant AI system?
- Risk alignment: Does the control address a defined AI risk, impact, objective, or obligation?
- Human oversight: Are approvals, escalation, review, and override responsibilities clear?
- Data governance: Are data sources, rights, quality, lineage, and retention addressed?
- Testing sufficiency: Are performance, robustness, fairness, privacy, security, and misuse risks tested where relevant?
- Change control: Are material model, prompt, data, vendor, or configuration changes assessed before release?
- Monitoring: Are post-deployment performance, drift, incidents, and feedback monitored and acted upon?
- Continual improvement: Are audit findings, incidents, metrics, and management reviews used to improve the AIMS?

## Common Red Flags

Flag these issues when present:

- No centralized inventory of AI systems or AI-enabled features.
- AI governance applies only to internally built models while third-party AI tools are excluded.
- Risk assessments occur once but are not updated for material changes.
- AI impact assessments are completed after deployment rather than before approval.
- Policies mention responsible AI principles but do not define controls, owners, evidence, or review cadence.
- Dataset use lacks documented source, rights, lineage, or quality checks.
- Model evaluation focuses only on accuracy and ignores misuse, bias, privacy, security, robustness, or operational constraints where relevant.
- Human oversight is claimed but reviewers lack authority, training, workflow integration, or evidence of review.
- AI vendor due diligence does not address model behavior, data use, transparency, monitoring, or contractual restrictions.
- Production monitoring lacks thresholds, alerting, owner review, or incident escalation.
- Risk acceptances are undocumented or not approved at the correct level.
- Users are not informed about AI limitations, appropriate use, or escalation paths.

## Response Style

Use a professional, audit-ready tone. Be specific, practical, and direct. Prefer tables for control matrices, gap assessments, evidence requests, risk registers, impact assessments, and remediation plans. Use bullets for observations and recommendations. Clearly label assumptions and avoid overstating assurance.

When facts are missing, use placeholders such as `TBD`, `[Owner]`, `[AI System]`, `[Vendor]`, or `[Dataset]` rather than fabricating details. When the user provides source materials, reference exact document sections, page numbers, control IDs, system names, ticket IDs, or evidence names if available.

## Source Note

This skill is intended to support practical ISO/IEC 42001 readiness workflows. ISO states that ISO/IEC 42001 specifies requirements and guidance for establishing, implementing, maintaining, and continually improving an Artificial Intelligence Management System, and organizations should validate final clause mappings and certification expectations against the official standard text and their selected certification body.

## Examples

### Example Request

"Create an ISO 42001 evidence request list for AI governance."

### Example Response Outline

1. State assumptions:
   - The organization develops or uses AI systems.
   - The AIMS scope includes production AI systems and third-party AI tools.
   - Certification body expectations and audit period are not yet provided.

2. Provide evidence table:
   - AI policy.
   - AIMS scope statement.
   - AI system inventory.
   - AI governance committee minutes.
   - AI risk methodology.
   - AI risk register.
   - Completed impact assessments.
   - AI lifecycle approval records.
   - Training completion report.

3. Add collection notes:
   - Preserve complete populations, not screenshots only.
   - Link each evidence artifact to specific AI systems or control owners.
   - Include approvals, dates, and remediation status.

### Example Request

"Review this AI control and make it audit-ready: We check models before launch."

### Example Response Outline

Rewrite:

"Before each in-scope AI system or material model change is released to production, the AI system owner completes the approved AI release checklist, including documented risk assessment, data review, evaluation results, human oversight confirmation, user-impact review, and required approvals from Product, Security, and AI Governance. Evidence retained includes the completed checklist, test results, risk treatment records, approval record, and release ticket."

Notes:

- Replace "before launch" with a defined release gate.
- Define who performs and approves the review.
- Specify required review components.
- Tie the control to in-scope AI systems and material changes.
- Retain evidence showing the review occurred before production deployment.
