---
name: iso-27001-compliance-controls
description: "Use when the user asks for ISO/IEC 27001, ISO 27001, ISMS, information security management system, Annex A controls, Statement of Applicability, risk treatment, audit readiness, evidence requests, gap assessments, policy-to-control mapping, supplier security, access control, incident management, or security compliance controls for SaaS, cloud, AI, technology, or enterprise organizations."
license: MIT
metadata:
  author: Raj Desikavinayagompillai
  version: '1.0'
---

# ISO 27001 Compliance Controls

## When to Use This Skill

Use this skill when the user asks for help with ISO/IEC 27001 compliance, including:

- Creating or improving an Information Security Management System (ISMS).
- Mapping policies, procedures, systems, or evidence to ISO/IEC 27001 clauses and Annex A controls.
- Preparing audit-readiness plans, evidence request lists, gap assessments, or remediation plans.
- Drafting control narratives, control owners, implementation guidance, or operating procedures.
- Building a Statement of Applicability (SoA), risk assessment, risk treatment plan, or internal audit checklist.
- Comparing ISO 27001 controls to SOC 2, ISO 42001, NIST CSF, CIS Controls, GDPR, or other frameworks.
- Reviewing security documentation for completeness against ISO 27001 expectations.

Do not provide legal advice or claim certification outcomes. Frame outputs as compliance support, audit preparation, and implementation guidance.

## Core Standards Orientation

When working on ISO 27001 tasks, distinguish between:

- **ISO/IEC 27001 clauses**: Mandatory ISMS requirements, including organizational context, leadership, planning, support, operations, performance evaluation, and improvement.
- **Annex A controls**: Reference security controls used to treat information security risks. ISO/IEC 27001:2022 includes 93 Annex A controls grouped into Organizational, People, Physical, and Technological themes.
- **Statement of Applicability**: The organization’s formal record of which Annex A controls apply, why they apply or do not apply, and implementation status.
- **Risk treatment**: The basis for selecting controls. Annex A controls should be tied back to identified risks, business context, regulatory obligations, customer requirements, and contractual commitments.

Always ask or infer which edition applies. Default to ISO/IEC 27001:2022 when the user does not specify an edition, and note that mappings may differ for ISO/IEC 27001:2013.

## Required Working Style

When producing ISO 27001 work:

1. **Clarify the organization context when material**:
   - Business model, industry, geography, cloud/on-premises environment, SaaS/product scope, employee count, and certification boundary.
   - Whether the user needs a lightweight startup-ready implementation or formal enterprise audit evidence.
   - Whether the target is readiness, internal audit, Stage 1 audit, Stage 2 audit, surveillance audit, or remediation.

2. **Anchor outputs to audit expectations**:
   - Tie each recommendation to the relevant clause, Annex A control, or ISMS artifact.
   - Specify what an auditor would expect to see, not just what the organization should do.
   - Separate design evidence from operating effectiveness evidence.

3. **Use practical, implementable language**:
   - Provide concrete procedures, evidence examples, ownership, cadence, and tooling suggestions.
   - Avoid generic “ensure appropriate controls” phrasing unless paired with testable criteria.
   - Prefer concise tables for mappings, evidence lists, and remediation trackers.

4. **Preserve professional caution**:
   - Do not guarantee certification.
   - Do not invent facts about the organization.
   - Flag assumptions clearly.
   - Recommend confirmation with the certification body, auditor, legal counsel, or security leadership where appropriate.

## Standard Workflow

Follow this workflow for most ISO 27001 compliance tasks.

### Scope and assumptions

Identify:

- ISMS scope and boundaries.
- In-scope products, teams, infrastructure, systems, locations, and third parties.
- Data types, including confidential information, personal data, customer data, production data, and security telemetry.
- Applicable legal, regulatory, contractual, and customer requirements.
- Assumptions and open questions.

If the request is underspecified but still actionable, proceed with reasonable assumptions and state them.

### Map requirements

Map the request to the right ISO 27001 components:

- Clauses 4-10 for ISMS governance, risk management, leadership, objectives, support, operations, monitoring, internal audit, management review, nonconformities, and continual improvement.
- Annex A Organizational controls for policies, roles, supplier relationships, cloud services, incident management, business continuity, legal and contractual obligations, privacy, and compliance.
- Annex A People controls for screening, awareness, terms of employment, disciplinary process, remote work, and reporting security events.
- Annex A Physical controls for secure areas, equipment protection, clear desk, cabling, maintenance, and secure disposal.
- Annex A Technological controls for identity and access management, authentication, logging, malware protection, backup, vulnerability management, secure configuration, network security, secure development, test data, and monitoring.

### Assess current state

For gap assessments or reviews, evaluate:

- **Policy design**: Whether documented policy requirements exist and match the control objective.
- **Process design**: Whether procedures, owners, cadence, and escalation paths are defined.
- **Implementation**: Whether tools and workflows enforce the control.
- **Evidence**: Whether records exist, are retained, and are audit-ready.
- **Operating effectiveness**: Whether the control has run consistently over a representative period.
- **Exceptions**: Whether deviations are approved, risk accepted, tracked, and reviewed.

Use severity ratings such as Critical, High, Medium, Low, or Observation. Define the rating criteria in the output.

### Recommend remediation

For each gap, provide:

- Gap statement.
- Related ISO clause or Annex A control.
- Risk or audit impact.
- Recommended remediation.
- Evidence to create or retain.
- Owner.
- Target date or priority.
- Dependencies.

### Package audit-ready outputs

Depending on the request, produce one or more of:

- Evidence request list.
- Control mapping matrix.
- Statement of Applicability draft.
- Risk register or risk treatment plan.
- Policy or procedure outline.
- Internal audit checklist.
- Management review agenda.
- Remediation tracker.
- Executive summary of readiness posture.

## Output Templates

### Evidence request list

Use this structure when the user asks what evidence to prepare:

| Area | ISO reference | Evidence request | Evidence type | Owner | Lookback period | Notes |
|---|---|---|---|---|---|---|
| Access control | Annex A technological controls | User access review export, reviewer sign-off, and remediation tickets | Operating effectiveness | IT/Security | Last 3-12 months | Include privileged access separately |

Evidence type should be one of:

- **Design**: Policy, procedure, standard, architecture diagram, role description, responsibility matrix.
- **Implementation**: Configuration screenshot, system setting, workflow, asset inventory, vendor record.
- **Operating effectiveness**: Logs, review records, tickets, meeting minutes, exception approvals, completed training, incident records.

### Gap assessment table

Use this structure for readiness reviews:

| ISO reference | Requirement or control expectation | Current state | Gap | Severity | Remediation | Evidence needed | Owner |
|---|---|---|---|---|---|---|---|

Keep gap statements specific and testable.

### Statement of Applicability table

Use this structure for SoA drafts:

| Annex A control | Applicability | Justification | Implementation status | Linked risks | Evidence | Owner |
|---|---|---|---|---|---|---|

Applicability should be one of:

- Applicable.
- Not applicable.
- Partially applicable.
- To be confirmed.

For controls marked not applicable, require a clear business and risk-based justification.

### Risk treatment plan

Use this structure when connecting risks to controls:

| Risk ID | Risk scenario | Inherent risk | Treatment decision | Selected controls | Residual risk | Risk owner | Target date | Evidence |
|---|---|---|---|---|---|---|---|---|

Treatment decision should be one of:

- Mitigate.
- Transfer.
- Avoid.
- Accept.

### Control narrative

Use this structure for control narratives:

- **Control objective**: The risk or requirement the control addresses.
- **Control activity**: The specific procedure performed.
- **Frequency**: Real-time, daily, weekly, monthly, quarterly, annually, or event-driven.
- **Owner**: Role accountable for operation.
- **Systems/tools**: Systems used to operate or evidence the control.
- **Evidence retained**: Records that demonstrate performance.
- **Exceptions**: How exceptions are documented, approved, remediated, and reviewed.
- **Testing approach**: How an auditor or internal reviewer can test design and operating effectiveness.

## Common ISO 27001 Work Products

### Audit readiness assessment

Include:

- Executive summary.
- Readiness rating.
- Scope and assumptions.
- Key strengths.
- Priority gaps.
- Evidence maturity.
- Remediation roadmap.
- Annex with detailed control-by-control findings.

### Internal audit checklist

Include:

- Audit objective.
- Audit scope.
- Criteria.
- Interviewees.
- Documents to inspect.
- Sample testing approach.
- Findings template.
- Nonconformity and observation definitions.

### Management review package

Include:

- ISMS performance metrics.
- Status of objectives.
- Audit results.
- Risk assessment and treatment status.
- Security incidents and lessons learned.
- Supplier and third-party issues.
- Nonconformities and corrective actions.
- Resource needs.
- Continual improvement decisions.

### Policy-to-control mapping

For every policy section, map:

- Policy requirement.
- ISO clause or Annex A control.
- Evidence source.
- Owner.
- Review cadence.
- Gaps or missing procedures.

## Mapping and Crosswalk Guidance

When crosswalking ISO 27001 to another framework:

1. State that mappings are directional, not perfect one-to-one equivalence.
2. Preserve the original framework wording where possible.
3. Include confidence levels such as Strong, Partial, or Weak.
4. Note control intent differences, evidence differences, and testing differences.
5. Identify unmapped requirements and areas requiring human review.

Use this table:

| Source framework requirement | ISO 27001 mapping | Mapping strength | Rationale | Evidence overlap | Gaps |
|---|---|---|---|---|---|

## Quality Bar

Before finalizing ISO 27001 outputs, check that:

- The scope and assumptions are clear.
- Clauses and Annex A controls are not mixed together incorrectly.
- Evidence requests distinguish design, implementation, and operating effectiveness.
- Recommendations are actionable, owned, and testable.
- The output does not imply certification is guaranteed.
- Any missing organization-specific facts are listed as open questions.
- Tables are formatted cleanly and can be copied into spreadsheets or audit workpapers.

## Example Prompts This Skill Should Handle

- “Create an ISO 27001 evidence request list for a SaaS company.”
- “Map our access control policy to ISO 27001:2022.”
- “Build a Statement of Applicability template.”
- “Review these security policies for ISO 27001 gaps.”
- “Create an ISO 27001 audit readiness roadmap.”
- “Crosswalk ISO 27001 and SOC 2 controls.”
- “Draft control narratives for vulnerability management and access reviews.”
- “Prepare an internal audit checklist for the ISMS.”
