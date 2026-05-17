---
name: hipaa-compliance-controls
description: "Use when the user asks for HIPAA compliance support, HIPAA Privacy Rule, Security Rule, Breach Notification Rule, HITECH, Business Associate Agreements, BAAs, covered entity or business associate obligations, PHI/ePHI safeguards, HIPAA risk analysis, gap assessments, audit readiness, evidence requests, control mapping, policy-to-control alignment, breach triage, or healthcare compliance controls for SaaS, cloud, AI, technology, healthcare providers, payers, clearinghouses, vendors, and service organizations."
license: MIT
metadata:
  version: '1.0'
  author: Hema Raj
---

# HIPAA Compliance Controls

## When to Use This Skill

Use this skill when the user asks for help with HIPAA compliance controls, HIPAA audit readiness, PHI/ePHI safeguards, Business Associate Agreements, risk analysis, breach notification, healthcare vendor security, or control mapping for organizations that create, receive, maintain, transmit, process, host, support, or otherwise interact with protected health information.

Common trigger phrases include:

- HIPAA, HIPAA compliance, HIPAA controls, HIPAA audit readiness
- Privacy Rule, Security Rule, Breach Notification Rule, HITECH
- PHI, ePHI, protected health information, health data
- Covered entity, business associate, subcontractor, healthcare vendor
- BAA, Business Associate Agreement, vendor due diligence
- HIPAA risk assessment, HIPAA risk analysis, safeguard implementation
- Administrative safeguards, physical safeguards, technical safeguards
- HIPAA policy mapping, evidence requests, gap assessment, remediation plan
- Healthcare SaaS, healthcare AI, telehealth, EHR integrations, patient data

Do not use this skill for direct medical advice, diagnosis, treatment decisions, or interpretation of personal health records unless paired with the appropriate health-data skill. This skill is for compliance, governance, controls, and audit readiness.

## Core Operating Principles

When using this skill:

1. Treat HIPAA as an organization-specific compliance program, not a checklist-only exercise. Confirm whether the entity is a covered entity, business associate, subcontractor, or non-HIPAA-regulated vendor where relevant.
2. Separate legal obligations from implementation controls. Explain which items are regulatory requirements, which are common audit expectations, and which are recommended practices.
3. Distinguish PHI from ePHI. Privacy Rule issues often apply to PHI broadly, while Security Rule safeguards apply to electronic PHI.
4. Build outputs around risk analysis, reasonable and appropriate safeguards, documented policies, workforce training, vendor controls, incident response, and evidence.
5. Avoid implying official certification. HIPAA does not have a single government-issued certification comparable to ISO certification.
6. Include a legal-review caveat for contractual, breach, regulatory-reporting, or enforcement-sensitive matters.
7. When the user asks for an auditor-ready deliverable, write in precise, evidence-oriented language suitable for compliance, legal, security, procurement, or healthcare operations teams.

## HIPAA Scope Triage

Before producing detailed recommendations, identify scope if it is not already clear:

- **Entity type**: Covered entity, business associate, subcontractor, hybrid entity, or vendor not directly regulated by HIPAA.
- **PHI role**: Creates, receives, maintains, transmits, stores, accesses, analyzes, de-identifies, supports systems containing, or merely routes PHI.
- **Data type**: PHI, ePHI, de-identified data, limited data set, genetic data, payment data, claims data, images, clinical notes, logs, backups, support tickets, telemetry, or AI training data.
- **Services**: SaaS, cloud hosting, managed services, analytics, AI model operations, telehealth, billing, claims, EHR integration, patient engagement, call center, help desk, backup, disaster recovery, or security monitoring.
- **Environment**: Production, staging, support tooling, data warehouse, SIEM, ticketing system, analytics stack, AI/ML pipeline, mobile app, or endpoint fleet.
- **Jurisdiction overlays**: State breach laws, 42 CFR Part 2, FTC Health Breach Notification Rule, consumer health data laws, PCI, SOC 2, ISO 27001, HITRUST, or contractual requirements.

If the answer depends materially on scope, ask one concise clarifying question before creating a final control matrix. If the user wants a generic starting point, state assumptions and proceed.

## HIPAA Rule Areas

Use these categories to organize analysis.

### Privacy Rule

Focus on how PHI may be used and disclosed, patient rights, minimum necessary use, notices, authorizations, workforce access, administrative processes, and relationships with business associates.

Typical control themes:

- Permitted and required uses and disclosures
- Minimum necessary standard
- Notice of Privacy Practices where applicable
- Individual rights: access, amendment, accounting of disclosures, restrictions, confidential communications
- Authorization management for non-routine uses and disclosures
- Workforce privacy training and sanctions
- Complaint process and privacy incident handling
- Business associate oversight and contract requirements
- De-identification and limited data set controls

### Security Rule

Focus on administrative, physical, and technical safeguards for ePHI. The Security Rule is risk-based and includes required and addressable implementation specifications. Addressable does not mean optional; the organization must implement the specification if reasonable and appropriate, implement an equivalent alternative, or document why neither is reasonable and appropriate.

Administrative safeguard themes:

- Security management process, including risk analysis and risk management
- Assigned security responsibility
- Workforce security and authorization/supervision
- Information access management
- Security awareness and training
- Security incident procedures
- Contingency planning
- Evaluation
- Business associate contracts and other arrangements

Physical safeguard themes:

- Facility access controls
- Workstation use
- Workstation security
- Device and media controls

Technical safeguard themes:

- Access controls
- Unique user identification
- Emergency access procedures
- Automatic logoff
- Encryption and decryption, where reasonable and appropriate
- Audit controls
- Integrity controls
- Person or entity authentication
- Transmission security

### Breach Notification Rule

Focus on whether an impermissible use or disclosure of unsecured PHI occurred, whether there is a low probability that PHI was compromised, and whether notification obligations are triggered.

Use the four-factor risk assessment structure:

- Nature and extent of PHI involved, including identifiers and likelihood of re-identification
- Unauthorized person who used or received the PHI
- Whether the PHI was actually acquired or viewed
- Extent to which the risk has been mitigated

Typical response outputs:

- Triage checklist
- Incident timeline
- Evidence preservation list
- Notification decision record
- Draft regulatory counsel escalation summary
- Remediation and corrective action plan

### HITECH and Enforcement Considerations

Consider HITECH-driven breach notification, business associate liability, enforcement risk, penalty exposure, and the importance of documented risk analysis, risk management, policies, procedures, training, and incident response records.

## Control Domain Framework

When building HIPAA control matrices, organize controls into these domains:

1. Governance and accountability
2. HIPAA scope, data inventory, and PHI/ePHI flows
3. Risk analysis and risk management
4. Policies and procedures
5. Workforce training and sanctions
6. Access control and identity management
7. Audit logging and monitoring
8. Encryption and transmission security
9. Integrity and change control
10. Vulnerability, patch, and configuration management
11. Incident response and breach notification
12. Business associate and subcontractor management
13. Physical security and device/media controls
14. Backup, disaster recovery, and contingency planning
15. Secure development, cloud, and AI/ML lifecycle controls
16. Privacy operations and individual rights
17. De-identification, retention, disposal, and data minimization
18. Compliance evaluation, testing, and management review

## Standard Output Formats

### HIPAA Control Matrix

Use this format when asked for controls, implementation planning, or audit readiness:

| Control ID | Domain | HIPAA Area | Control Objective | Control Activity | Required/Addressable/Expected | Owner | Evidence | Frequency | Risk Notes |
|---|---|---|---|---|---|---|---|---|---|

Guidelines:

- Use short, stable control IDs such as HIPAA-GOV-01, HIPAA-RISK-01, HIPAA-AC-01, HIPAA-IR-01.
- Mark Security Rule implementation specifications as Required or Addressable where known. Mark common audit practices as Expected.
- Include evidence that can actually be produced, such as policies, risk analysis reports, access reviews, training logs, BAA inventory, incident tickets, backup test records, and vulnerability reports.
- Include operational frequency, such as upon hire, annually, quarterly, continuously, per change, per incident, or per vendor onboarding.

### Gap Assessment

Use this format when comparing current practices against HIPAA expectations:

| Area | Current State | HIPAA Expectation | Gap | Risk | Priority | Recommended Remediation | Evidence Needed |
|---|---|---|---|---|---|---|---|

Priority guidance:

- High: Missing risk analysis, lack of access controls, no BAA where required, no incident response process, no encryption decision record for ePHI, no audit logging, unmanaged vendor/subcontractor access, or unresolved breach-notification exposure.
- Medium: Incomplete policies, informal access reviews, inconsistent training, weak backup testing, incomplete data-flow inventory, or incomplete device/media controls.
- Low: Documentation polish, evidence naming, control ownership clarity, or minor procedural gaps.

### Evidence Request List

Use this format for audit readiness:

| Evidence Area | Requested Evidence | Purpose | Owner | Lookback Period | Notes |
|---|---|---|---|---|---|

Common evidence categories:

- HIPAA risk analysis and risk management plan
- HIPAA policies and procedures
- Sanction policy and workforce training records
- Workforce access provisioning, modification, and termination samples
- Role-based access matrix and privileged access review
- Audit log configuration and monitoring evidence
- Incident response plan, incident register, and breach assessment records
- BAA inventory, executed BAAs, subcontractor list, and vendor due diligence
- Encryption standards, key management procedures, and transmission security evidence
- Backup schedules, restore tests, disaster recovery plan, and emergency mode operations plan
- Device/media disposal logs and asset inventory
- Facility or physical access control evidence where applicable
- Privacy complaints, access requests, amendment requests, accounting requests, and related workflows

### Policy-to-Control Mapping

Use this format when mapping HIPAA policies to controls:

| Policy | Policy Requirement | Related Control ID | HIPAA Area | Implementation Evidence | Gap or Enhancement |
|---|---|---|---|---|---|

### BAA Review Summary

Use this format when reviewing Business Associate Agreement language:

| Clause Area | Expected HIPAA Position | Present? | Risk if Missing or Weak | Suggested Revision Theme |
|---|---|---|---|---|

BAA areas to check:

- Permitted and required uses and disclosures
- Use or disclosure only as permitted by the BAA or required by law
- Safeguards to prevent unauthorized use or disclosure
- Reporting of unauthorized uses, disclosures, and security incidents
- Breach notification cooperation and timing
- Subcontractor flow-down obligations
- Access, amendment, and accounting support
- Books and records availability to the Secretary of HHS where applicable
- Return or destruction of PHI at termination, if feasible
- Minimum necessary and data minimization expectations
- Indemnity, limitation of liability, insurance, and audit rights if requested by the user, noting these are contractual risk terms rather than core HIPAA regulatory clauses

### Breach Triage Summary

Use this format for breach or incident questions:

| Triage Question | Known Facts | Assessment | Evidence Needed | Next Step |
|---|---|---|---|---|

Always include:

- Whether PHI/ePHI appears involved
- Whether the PHI was unsecured
- Whether the event appears to be an impermissible use or disclosure
- Four-factor compromise assessment
- Mitigation steps already taken
- Notification deadlines to evaluate with counsel
- Evidence preservation steps
- Recommendation to involve privacy counsel for reportability determinations

## Common HIPAA Control Examples

Use these examples as starting points, adapting to the user's organization and scope.

### Governance and Accountability

- HIPAA-GOV-01: Assign a HIPAA privacy and/or security officer responsible for privacy and security program oversight.
- HIPAA-GOV-02: Maintain HIPAA policies and procedures aligned to current operations, systems, vendors, and PHI data flows.
- HIPAA-GOV-03: Review HIPAA program status, high-risk gaps, incidents, and remediation progress with management at defined intervals.

### Risk Analysis and Risk Management

- HIPAA-RISK-01: Perform and document an enterprise risk analysis covering ePHI systems, assets, threats, vulnerabilities, likelihood, impact, and existing safeguards.
- HIPAA-RISK-02: Maintain a risk treatment plan with owners, target dates, residual risk decisions, and management approval.
- HIPAA-RISK-03: Reassess risk after material changes such as new products, AI use cases, EHR integrations, cloud migrations, acquisitions, or major vendor changes.

### Access Control

- HIPAA-AC-01: Assign unique user IDs for workforce members and service accounts that access ePHI.
- HIPAA-AC-02: Enforce role-based access based on job responsibilities and minimum necessary principles.
- HIPAA-AC-03: Review access to ePHI systems on a defined cadence and upon role change or termination.
- HIPAA-AC-04: Implement emergency access procedures for ePHI during downtime, disaster recovery, or urgent care/support scenarios.

### Audit Logging and Monitoring

- HIPAA-LOG-01: Enable audit logging for systems that create, receive, maintain, or transmit ePHI.
- HIPAA-LOG-02: Monitor logs for unauthorized access, anomalous activity, privileged account use, and data export events.
- HIPAA-LOG-03: Retain logs according to legal, contractual, and operational requirements.

### Encryption and Transmission Security

- HIPAA-ENC-01: Encrypt ePHI at rest where reasonable and appropriate, or document equivalent protections and risk acceptance.
- HIPAA-ENC-02: Encrypt ePHI in transit across open networks using approved protocols.
- HIPAA-ENC-03: Maintain key management procedures covering generation, storage, rotation, revocation, and access.

### Incident Response and Breach Notification

- HIPAA-IR-01: Maintain procedures for identifying, reporting, investigating, documenting, and responding to security incidents involving ePHI.
- HIPAA-IR-02: Maintain a breach assessment workflow using the four-factor low-probability-of-compromise analysis.
- HIPAA-IR-03: Track incidents, mitigation actions, notification decisions, and corrective actions.

### Vendor and Business Associate Management

- HIPAA-BA-01: Maintain an inventory of business associates and subcontractors that create, receive, maintain, or transmit PHI.
- HIPAA-BA-02: Execute BAAs before disclosing PHI to business associates where required.
- HIPAA-BA-03: Require subcontractors to agree to substantially similar restrictions and safeguards.
- HIPAA-BA-04: Perform vendor risk review before onboarding and periodically thereafter based on risk.

### Contingency Planning

- HIPAA-CP-01: Maintain data backup procedures for ePHI.
- HIPAA-CP-02: Maintain disaster recovery and emergency mode operation procedures.
- HIPAA-CP-03: Test backup restoration and contingency procedures periodically.

### Device and Media Controls

- HIPAA-DM-01: Maintain an inventory of devices and media that store or access ePHI.
- HIPAA-DM-02: Sanitize, destroy, or securely dispose of media containing ePHI.
- HIPAA-DM-03: Track movement, reuse, and disposal of ePHI-containing hardware and removable media.

### Secure Development, Cloud, and AI

- HIPAA-SDLC-01: Require security review for applications, APIs, integrations, and AI workflows that handle PHI.
- HIPAA-SDLC-02: Restrict production PHI use in development, testing, analytics, and model-training environments unless approved and protected.
- HIPAA-SDLC-03: Maintain data-flow diagrams for PHI through cloud services, logs, support tools, analytics, and AI systems.
- HIPAA-SDLC-04: Validate that third-party AI, analytics, monitoring, and support vendors are covered by BAAs where required.

## Response Style

When responding:

- Be practical, control-oriented, and evidence-focused.
- Use tables for matrices, gap assessments, and evidence lists.
- State assumptions clearly when facts are missing.
- Identify high-risk gaps first.
- Separate mandatory HIPAA concepts from recommended security practices.
- Avoid unsupported claims that a control alone makes an organization HIPAA compliant.
- Recommend counsel review for BAAs, breach notification, regulatory reporting, enforcement response, or complex applicability questions.

## Common Gotchas

- Addressable Security Rule specifications are not automatically optional. The organization must decide whether each is reasonable and appropriate, implement an equivalent alternative, or document why neither is appropriate.
- A signed BAA does not make a vendor secure. Vendor due diligence and ongoing oversight are still needed.
- HIPAA scope often extends into logs, backups, support tickets, monitoring tools, analytics platforms, and AI workflows.
- De-identified data must meet a recognized de-identification method before it is treated as outside PHI obligations.
- Breach analysis should be documented even when the final decision is that notification is not required.
- Encryption can materially affect breach notification analysis because the Breach Notification Rule focuses on unsecured PHI.
- HIPAA risk analysis must be specific to systems, assets, threats, vulnerabilities, likelihood, impact, and safeguards. A generic security questionnaire is usually not enough.
- Business associates can be directly liable for certain HIPAA obligations and must manage subcontractor flow-down requirements.

## Example Prompts This Skill Should Handle

- "Create a HIPAA control matrix for a healthcare SaaS company."
- "Build a HIPAA evidence request list for audit readiness."
- "Map our access control policy to HIPAA Security Rule safeguards."
- "Review this BAA for missing HIPAA provisions."
- "Create a HIPAA gap assessment for a business associate."
- "What controls do we need for ePHI in AWS?"
- "Prepare a breach triage checklist for a suspected PHI disclosure."
- "Compare our SOC 2 controls to HIPAA expectations."
- "Create a HIPAA remediation roadmap for an AI healthcare product."
