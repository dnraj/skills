---
name: soc1-compliance-controls
description: "Use when the user asks for SOC 1 compliance support, control mapping, ICFR control objectives, SSAE 18 readiness, Type I or Type II preparation, evidence request lists, gap assessments, process narratives, user control considerations, complementary subservice organization controls, auditor-ready control descriptions, or remediation planning for service organizations whose services may affect user entities' internal control over financial reporting."
license: MIT
metadata:
  version: '1.0'
---

# SOC 1 Compliance Controls

## When to Use This Skill

Use this skill when the user asks for help with SOC 1 work, including:

- Creating, reviewing, or improving SOC 1 control descriptions, control matrices, or control narratives.
- Preparing for a SOC 1 Type I or Type II engagement.
- Mapping business processes, IT general controls, application controls, reports, reconciliations, or evidence to SOC 1 control objectives.
- Creating evidence request lists, readiness workplans, remediation trackers, population support, or exception summaries.
- Drafting or improving a system description, process narrative, control objective set, or management-facing readiness summary.
- Identifying user control considerations, complementary user entity controls, complementary subservice organization controls, and carve-out or inclusive subservice organization considerations.
- Supporting service organizations whose services may affect customer or user-entity internal control over financial reporting.

Do not present work product as legal, accounting, audit, or attestation advice. If the user needs an official audit opinion, report conclusion, management assertion, or interpretation of attestation standards, advise them to consult their CPA firm, service auditor, user auditor, counsel, or qualified compliance advisor.

## Core Principles

1. Anchor SOC 1 work in financial-reporting risk:
   - SOC 1 is focused on controls at a service organization that are likely to be relevant to user entities' internal control over financial reporting.
   - Prioritize transaction processing, data completeness and accuracy, report logic, reconciliations, access, change management, and IT operations that support financially relevant services.
   - Avoid drifting into SOC 2 Trust Services Criteria unless the user explicitly asks for SOC 2 or security/privacy controls outside the ICFR context.

2. Start by identifying the engagement context:
   - Type I or Type II.
   - Report period for Type II, or as-of date for Type I.
   - In-scope services, systems, applications, infrastructure, locations, teams, vendors, and subservice organizations.
   - Relevant transaction classes, financial statement assertions, reports, calculations, and user-entity dependencies.
   - Audit stage: scoping, readiness, control design, evidence collection, walkthroughs, testing, exception response, remediation, or report review.

3. Tie every control to a control objective:
   - What financial-reporting risk is being addressed?
   - Which system, process, transaction, report, or data element is affected?
   - Who performs the control?
   - How often does it operate?
   - What evidence proves the control was performed?
   - How are exceptions identified, reviewed, approved, tracked, and remediated?

4. Distinguish design from operating effectiveness:
   - For Type I, focus on whether controls are suitably designed and in place as of the report date.
   - For Type II, also focus on whether controls operated effectively throughout the report period.
   - Flag controls that are not testable, lack evidence, operate inconsistently, or depend on undocumented judgment.

5. Make outputs auditor-ready:
   - Use clear fields for control objective, control activity, owner, frequency, evidence, population, system, report period, exception handling, and testing notes.
   - Separate existing controls, gaps, remediation actions, optional enhancements, and assumptions.
   - Avoid unsupported statements such as "compliant," "audit-ready," or "effective" unless evidence has been reviewed.

## SOC 1 Domain Map

Use these domains to organize SOC 1 work. Select only the domains relevant to the service organization's system and control objectives.

### Governance and Control Environment

Typical topics:

- Management oversight of the service organization system.
- Role and responsibility assignment.
- Policy management.
- Risk assessment for financially relevant outsourced services.
- Monitoring of control performance and remediation.
- Board, executive, or management review where relevant to the control environment.

Common evidence:

- Policies and procedures.
- Risk assessment results.
- Management review materials.
- Control owner assignments.
- Issue logs and remediation trackers.
- Internal audit or compliance monitoring results.

### Transaction Processing Controls

Typical topics:

- Completeness, accuracy, authorization, and timeliness of transaction processing.
- Intake, validation, calculation, posting, settlement, or reporting of user-entity transactions.
- Exception handling, suspense items, rejects, adjustments, reversals, and corrections.
- Batch controls, interface controls, file transfer controls, and reconciliations.

Common evidence:

- Transaction logs.
- Batch control totals.
- File receipt and transmission logs.
- Reconciliation workpapers.
- Exception reports.
- Adjustment approvals.
- Processing calendars.

### Application and Report Controls

Typical topics:

- System calculations.
- Configurable business rules.
- User-facing or auditor-used reports.
- Completeness and accuracy of system-generated reports.
- Interfaces and data transformations.
- Master data and standing data maintenance.

Common evidence:

- Report inventories.
- Report logic documentation.
- Report parameter screenshots or exports.
- Completeness and accuracy validation.
- Configuration change logs.
- Master data change approvals.
- Interface monitoring evidence.

### Logical Access

Typical topics:

- User provisioning and approvals.
- Role-based access.
- Privileged access.
- Segregation of duties.
- Periodic access reviews.
- Termination and transfer access removal.
- Access to financially relevant applications, databases, infrastructure, and reporting tools.

Common evidence:

- User access listings.
- Access request and approval tickets.
- Privileged account inventory.
- Periodic access review evidence.
- Termination reports and access-removal tickets.
- Role permission matrices.
- MFA or authentication configuration where relevant.

### Change Management

Typical topics:

- Change requests, approvals, testing, and deployment.
- Emergency changes.
- Segregation of duties in development and release.
- Configuration changes affecting calculations, reports, workflows, or access roles.
- Version control, migration, and release monitoring.

Common evidence:

- Change tickets.
- Pull requests and approvals.
- Test evidence.
- Deployment logs.
- Release notes.
- Emergency change documentation.
- Configuration migration records.

### Computer Operations

Typical topics:

- Job scheduling and batch monitoring.
- Backup and recovery.
- Incident management.
- Problem management.
- Interface monitoring.
- System availability where downtime could affect financially relevant processing.

Common evidence:

- Job schedules and completion logs.
- Failed job investigations.
- Backup job reports and restore tests.
- Incident tickets and postmortems.
- Interface error reports.
- Monitoring alerts and resolution records.

### Vendor and Subservice Organization Management

Typical topics:

- Identification of vendors and subservice organizations that support the in-scope system.
- Carve-out or inclusive treatment of subservice organizations.
- Review of SOC reports or equivalent assurance from subservice organizations.
- Monitoring of complementary subservice organization controls.
- Vendor risk assessment and issue tracking.

Common evidence:

- Vendor inventory.
- Subservice organization list.
- SOC report reviews.
- Bridge letters where applicable.
- Vendor risk assessments.
- Contractual responsibility matrices.
- Issue logs and follow-up evidence.

### Complementary User Entity Controls

Typical topics:

- Controls that user entities must operate for the service organization's controls to achieve the stated control objectives.
- User entity responsibilities for data input, approval, reconciliation, access administration, review of reports, or investigation of exceptions.
- Communication of user control considerations in the system description.

Common evidence:

- User responsibility matrix.
- Customer control guide.
- System description sections.
- Customer onboarding materials.
- Service agreements.
- User access administration procedures.

## Standard Workflow

Follow this workflow for most SOC 1 requests:

1. Clarify scope if necessary:
   - Ask only for missing details that materially change the output.
   - If the user needs a quick draft, make reasonable assumptions and label them clearly.
   - Clarify whether the request is for readiness, control design, evidence collection, fieldwork support, or remediation.

2. Identify the financially relevant process:
   - Determine the outsourced service, user entity impact, transaction class, report, calculation, or assertion involved.
   - Note where the service organization's system affects completeness, accuracy, authorization, cutoff, occurrence, existence, valuation, rights, obligations, or disclosure.

3. Identify or draft control objectives:
   - Write control objectives in outcome-oriented language.
   - Keep objectives specific enough to test, but broad enough to support multiple related controls.
   - Avoid mixing unrelated risks into one objective.

4. Assess control design:
   - Confirm who performs the control, when, where, with what data, and what evidence is retained.
   - Confirm the control addresses the stated control objective.
   - Check whether complementary user entity controls or subservice organization controls are necessary.

5. Assess operating readiness:
   - Identify the population for sampling.
   - Determine whether evidence exists for the full report period.
   - Flag inconsistent operation, missing timestamps, unclear reviewer identity, incomplete populations, or undocumented exceptions.

6. Produce the requested artifact:
   - Control matrix.
   - Evidence request list.
   - Gap assessment.
   - Remediation roadmap.
   - Process narrative.
   - System description outline.
   - Control objective mapping.
   - Exception response.
   - Auditor request response.

7. Add practical cautions:
   - State assumptions.
   - Identify dependencies on service auditor expectations.
   - Recommend validation with the user's auditor for final report treatment.

## Output Templates

### Control Matrix

Use this structure when creating or revising SOC 1 controls:

| Control ID | Control Objective | Domain | Control Activity | Owner | Frequency | Population | Evidence | System or Process | CUEC or CSOC Dependency | Design Notes | Operating Effectiveness Notes |
|---|---|---|---|---|---|---|---|---|---|---|---|
| SOC1-XX-01 | Ensure transactions are processed completely and accurately | Transaction Processing | [Owner] reviews the daily processing exception report, investigates exceptions, and documents resolution before close of business | Operations | Daily | Daily processing exception reports | Exception report, investigation notes, resolution ticket | [Application] | User entities reconcile output reports to their records | Confirm review occurs after each processing cycle | Test daily evidence across the report period and inspect exception resolution |

### Control Objective Map

Use this structure when mapping processes to control objectives:

| Process Area | Financial Reporting Risk | Control Objective | Related Controls | Relevant Systems | User Entity Dependency | Notes |
|---|---|---|---|---|---|---|
| Claims Processing | Claims may be calculated inaccurately or omitted from output files | Controls provide reasonable assurance that claims are processed completely and accurately according to configured plan rules | SOC1-CP-01, SOC1-CP-02 | Claims platform, reporting database | User entity provides complete and authorized source data | Validate report logic and exception handling |

### Evidence Request List

Use this structure for readiness and audit evidence collection:

| Request ID | Domain | Control ID | Evidence Needed | Purpose | Owner | Period Covered | Due Date | Format | Population Required | Notes |
|---|---|---|---|---|---|---|---|---|---|---|
| ER-01 | Logical Access | SOC1-LA-01 | User access listing for in-scope financial applications | Supports access provisioning and access review controls | IT | [Report Period] | TBD | CSV export | Full active user population | Include user, role, status, created date, last login if available |

### Gap Assessment

Use this structure for readiness reviews:

| Area | Current State | Expected SOC 1 Control | Gap | Financial Reporting Risk | Priority | Recommended Remediation | Owner | Target Date |
|---|---|---|---|---|---|---|---|---|
| Report Validation | Reports are used for customer reconciliations but report logic is undocumented | Key reports have documented logic and periodic completeness and accuracy validation | No documented validation for key report | User entities may rely on incomplete or inaccurate information | High | Document report logic and perform quarterly validation of report parameters, data source, and output totals | Product or Finance Systems | TBD |

### Remediation Roadmap

Use this structure for implementation planning:

| Workstream | Action | Dependency | Owner | Effort | Priority | Target Date | Success Criteria |
|---|---|---|---|---|---|---|---|
| Transaction Processing | Formalize daily exception review and resolution evidence | Define exception report owner and retention location | Operations | Medium | High | TBD | Daily evidence retained with reviewer, date, exceptions, and resolution status |

### Process Narrative

Use this structure for system descriptions or walkthrough preparation:

```text
Process name:
[Name of process]

Financial reporting relevance:
[Explain why the process, transaction, report, or system matters to user entities' ICFR.]

Process overview:
[Describe the flow from input through processing, review, output, and exception handling.]

Key systems:
[List applications, databases, file transfer tools, reporting systems, infrastructure, and third parties.]

Key inputs:
[List source files, customer instructions, transaction records, master data, or configurations.]

Key processing steps:
1. [Step]
2. [Step]
3. [Step]

Key outputs:
[List reports, files, postings, confirmations, statements, or dashboards.]

Control points:
[List relevant control IDs and where each control occurs in the process.]

Complementary user entity controls:
[List user responsibilities or state TBD.]

Subservice organization considerations:
[List subservice dependencies and carve-out/inclusive treatment if known.]

Evidence retained:
[List evidence artifacts and retention location.]

Assumptions:
[List assumptions and open questions.]
```

### Control Narrative

Use this format for auditor-friendly control descriptions:

```text
Control objective:
[Describe the financial-reporting risk or objective.]

Control activity:
[Describe who performs the control, what they do, how often, where it is documented, and what evidence is retained.]

Systems and data in scope:
[List relevant systems, applications, reports, interfaces, transaction populations, or data elements.]

Control owner:
[Role or team.]

Frequency:
[Per occurrence, daily, weekly, monthly, quarterly, annually.]

Population:
[Describe the complete population from which audit samples may be selected.]

Evidence:
[List evidence artifacts.]

Exceptions and remediation:
[Describe how exceptions are identified, tracked, approved, and resolved.]

CUECs and CSOCs:
[List complementary user entity controls and complementary subservice organization controls if applicable.]

Assumptions:
[List assumptions or dependencies.]
```

### Exception Response

Use this structure when helping respond to auditor findings or exceptions:

| Exception | Control Impact | Root Cause | Compensating Evidence | Remediation Plan | Owner | Target Date | Auditor Follow-up Needed |
|---|---|---|---|---|---|---|---|
| [Describe exception] | [Control objective affected] | [Known or TBD] | [Evidence that may reduce risk] | [Corrective action] | [Owner] | TBD | [Questions or additional support needed] |

## Review Guidance

When reviewing SOC 1 controls or evidence, check for:

- Control objective alignment: Does the control directly address a financially relevant risk?
- Testability: Can an auditor identify a population, select samples, and inspect evidence?
- Completeness: Does the control include owner, frequency, scope, evidence, and exception handling?
- Precision: Is the review precise enough to detect a meaningful error?
- Evidence quality: Is evidence complete, dated, attributable to the performer or reviewer, and retained?
- Population clarity: Can the full population be generated and reconciled to evidence?
- Timing: Did the control operate at the required frequency throughout the Type II period?
- Segregation of duties: Are request, approval, implementation, processing, and review responsibilities appropriately separated?
- Report reliability: Are system-generated reports validated for completeness and accuracy before use as control evidence?
- CUEC clarity: Are user-entity responsibilities specific, realistic, and linked to control objectives?
- Subservice clarity: Are subservice organization dependencies identified, monitored, and reflected consistently in the report approach?

## Common Red Flags

Flag these issues when present:

- Control objectives are copied from SOC 2 and do not relate to ICFR.
- Control language says "all transactions" but evidence covers only a subset.
- Reviews are performed but not dated, signed off, or tied to the reviewed population.
- The same person prepares and approves a financially significant adjustment without compensating review.
- A key report is used as evidence but has no completeness and accuracy validation.
- Access reviews exclude administrators, service accounts, databases, or reporting tools.
- Terminated users are removed manually with no SLA, ticket trail, or periodic review.
- Changes to calculations, reports, or workflows are deployed without testing or business approval.
- Exception reports exist but no one documents investigation or resolution.
- User control considerations are vague, such as "customers are responsible for their controls."
- Subservice organizations are used but not identified as carve-out or inclusive.
- Bridge letters are used without assessing whether they cover the required period and services.
- Control owners are tools, team mailboxes, or departments rather than accountable roles.

## Response Style

Use a professional, audit-ready tone. Be specific, practical, and direct. Prefer tables for matrices, evidence requests, gap assessments, mappings, and remediation plans. Use bullets for observations and recommendations. Clearly label assumptions and avoid overstating assurance.

When facts are missing, use placeholders such as `TBD`, `[Owner]`, `[System]`, `[Report Period]`, or `[Service Auditor]` rather than fabricating details. When the user provides source materials, cite or reference the exact document sections, page numbers, control IDs, ticket IDs, evidence names, or system exports if available.

## Reference Anchors

Use these public references as orientation points, but rely on the user's auditor or CPA firm for final engagement-specific guidance:

- AICPA SOC 1 overview: https://www.aicpa-cima.com/topic/audit-assurance/audit-and-assurance-greater-than-soc-1
- AICPA SOC suite overview: https://www.aicpa-cima.com/resources/landing/system-and-organization-controls-soc-suite-of-services
- AICPA management guide for SOC 1 engagements: https://us.aicpa.org/content/dam/aicpa/interestareas/frc/auditattest/downloadabledocuments/info-for-mgmt-of-serv-org-in-soc-engagement.pdf

## Examples

### Example Request

"Create a SOC 1 evidence request list for access management."

### Example Response Outline

1. State assumptions:
   - SOC 1 Type II readiness is the objective.
   - Production financial application, identity provider, HRIS, ticketing system, and reporting database are in scope.
   - Report period is not yet provided.

2. Provide an evidence table:
   - User access listing.
   - New user provisioning tickets.
   - Termination records.
   - Quarterly access review evidence.
   - Privileged access listing.
   - Role permission matrix.
   - Service account inventory.

3. Add collection notes:
   - Include full population exports, not screenshots only.
   - Preserve timestamps, reviewer identity, and approval records.
   - Reconcile HR terminations to access removals.
   - Validate that access to reporting databases and administration consoles is included.

### Example Request

"Rewrite this SOC 1 control so it is auditor-ready: We check the monthly report before sending it to customers."

### Example Response Outline

Rewrite:

"On a monthly basis, before customer distribution, the Finance Operations Manager reviews the [Monthly Report Name] generated from [System] for completeness and accuracy by reconciling total transaction count and total dollar amount to the approved source file and investigating variances above [Threshold]. The reviewer documents the review date, reconciliation results, identified exceptions, and resolution status in [Workpaper Location]. Evidence retained includes the generated report, source file, reconciliation workpaper, exception log, and reviewer sign-off."

Notes:

- Replace "check" with the specific review procedure.
- Identify the report, source data, reviewer, timing, and evidence.
- Define the variance threshold and exception handling.
- Confirm whether the report is financially relevant to user entities.
