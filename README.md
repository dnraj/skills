# Audit Skills README

This README describes an audit skills capability designed to help teams prepare for and support audits across ISO/IEC 27001, SOC 2, HIPAA, and FedRAMP. ISO/IEC 27001 defines requirements for an information security management system (ISMS), SOC 2 evaluates controls against Trust Services Criteria, HIPAA Security Rule protects electronic protected health information with administrative, physical, and technical safeguards, and FedRAMP provides a standardized approach to security assessment and authorization for cloud services used by the U.S. federal government.[cite:1][cite:6][cite:7][cite:16][cite:17]

## Purpose

The goal of these audit skills is to make audit preparation more repeatable, evidence-driven, and framework-aware. The capability should help security, compliance, engineering, and GRC teams gather evidence, map controls, identify gaps, and maintain readiness for internal reviews, customer diligence, and formal assessments.[cite:1][cite:6][cite:7][cite:17]

## Framework coverage

| Framework | Primary focus | What an audit skills capability should support |
|---|---|---|
| ISO/IEC 27001 | Establishing, implementing, maintaining, and continually improving an ISMS.[cite:1] | Scope definition, risk assessment, Statement of Applicability support, policy and control evidence, internal audit support, corrective actions. [cite:1][cite:2][cite:4] |
| SOC 2 | Independent evaluation of controls against one or more Trust Services Criteria.[cite:6][cite:12] | Security controls inventory, evidence collection, control testing support, user access reviews, change management evidence, vendor and incident records. [cite:6][cite:12][cite:15] |
| HIPAA | Protection of ePHI using administrative, physical, and technical safeguards.[cite:7] | Safeguard mapping, risk analysis support, access control evidence, workforce training records, incident handling documentation, business associate oversight. [cite:7][cite:10] |
| FedRAMP | Standardized security assessment, authorization, and continuous monitoring for cloud services.[cite:16][cite:17][cite:26] | NIST 800-53 control mapping, SSP support, 3PAO evidence packaging, POA&M tracking, continuous monitoring artifacts, agency authorization workflows. [cite:19][cite:21][cite:22][cite:25] |

## Core skills

A useful audit skills implementation should cover the following functions:

- Control mapping across multiple frameworks, especially mapping common controls once and reusing them across ISO 27001, SOC 2, HIPAA, and FedRAMP where practical.[cite:1][cite:6][cite:7][cite:21]
- Evidence collection and normalization, including policies, procedures, screenshots, tickets, logs, risk assessments, training records, and system configurations used to support audit requests.[cite:2][cite:10][cite:19]
- Gap assessment against framework requirements, with clear separation between implemented controls, partially implemented controls, and missing evidence.[cite:4][cite:6][cite:7][cite:21]
- Document support for key audit artifacts such as the ISO Statement of Applicability, SOC narratives and evidence sets, HIPAA safeguard documentation, and FedRAMP SSP, SAR, and POA&M inputs.[cite:2][cite:19][cite:22]
- Continuous monitoring workflows so compliance is maintained between audit cycles, which is especially important for ISO continual improvement and FedRAMP ongoing authorization expectations.[cite:1][cite:17][cite:19][cite:25]

## Recommended repository structure

```text
/audit-skills
  /frameworks
    iso27001.md
    soc2.md
    hipaa.md
    fedramp.md
  /controls
    common-control-library.md
    mappings.csv
  /evidence
    /policies
    /access-reviews
    /risk-assessments
    /incidents
    /training
    /vendors
  /templates
    statement-of-applicability.md
    soc2-request-list.md
    hipaa-risk-analysis.md
    fedramp-ssp-checklist.md
    poam-template.md
  /runbooks
    evidence-collection.md
    audit-interviews.md
    remediation-tracking.md
    continuous-monitoring.md
  README.md
```

This structure separates framework guidance, reusable controls, evidence, and operational runbooks so teams can maintain one working system instead of four disconnected compliance efforts. That approach aligns well with the risk-based and control-centered nature of ISO 27001, SOC 2, HIPAA Security Rule, and FedRAMP.[cite:1][cite:6][cite:7][cite:17][cite:21]

## Minimum deliverables

For practical audit support, the audit skills package should include:

- A common control catalog mapped to each framework requirement or criterion.[cite:1][cite:6][cite:7][cite:21]
- Evidence request checklists by framework and by audit phase, such as readiness, fieldwork, remediation, and ongoing monitoring.[cite:19][cite:22][cite:25]
- Templates for risk assessments, policy attestations, access reviews, incident reports, vendor reviews, and remediation plans.[cite:4][cite:7][cite:10]
- A system for recording owners, review cadence, evidence freshness, exceptions, and compensating controls.[cite:1][cite:4][cite:10][cite:17]
- Guidance on how to package materials for assessors, auditors, customers, or sponsoring agencies.[cite:6][cite:19][cite:22]

## Notes by framework

### ISO/IEC 27001

ISO/IEC 27001 is centered on an ISMS and continual improvement, so the audit skills should emphasize scope, risk treatment, internal audits, management review, and documentation discipline.[cite:1][cite:4] The capability should also support control selection and tracking through a Statement of Applicability.[cite:2]

### SOC 2

SOC 2 is built around the AICPA Trust Services Criteria, with security as the common criterion and availability, processing integrity, confidentiality, and privacy added as needed.[cite:6][cite:12] The audit skills should therefore support narrative-based evidence, operating effectiveness testing, and period-based evidence collection.[cite:6][cite:9]

### HIPAA

HIPAA Security Rule applies to ePHI and requires administrative, physical, and technical safeguards to preserve confidentiality, integrity, and availability.[cite:7] Audit skills should pay special attention to risk analysis, access management, workforce practices, and documentation of reasonable and appropriate safeguards.[cite:7][cite:10]

### FedRAMP

FedRAMP is intended for cloud services used by federal agencies and uses a standardized authorization approach tied to federal security requirements.[cite:16][cite:17][cite:26] Audit skills for FedRAMP should support pre-authorization, SSP preparation, assessment support, POA&M management, and continuous monitoring after authorization.[cite:19][cite:22][cite:25]

## Implementation guidance

Start with a shared control model and map that model outward to each framework, because all four frameworks rely on documented controls, evidence, and ongoing risk management even though the audit mechanics differ.[cite:1][cite:6][cite:7][cite:21] Then define evidence owners, review cycles, and remediation workflows so the repository stays current and usable during an audit window.[cite:4][cite:10][cite:19]

## Example use cases

- Preparing an ISO 27001 internal audit package with policies, risk treatment records, and Statement of Applicability support.[cite:1][cite:2]
- Responding to a SOC 2 readiness assessment by collecting access reviews, change records, and incident management evidence.[cite:6][cite:9]
- Organizing HIPAA Security Rule documentation for systems handling ePHI.[cite:7][cite:10]
- Building a FedRAMP evidence library for SSP sections, 3PAO testing support, POA&M updates, and continuous monitoring submissions.[cite:19][cite:22][cite:25]
