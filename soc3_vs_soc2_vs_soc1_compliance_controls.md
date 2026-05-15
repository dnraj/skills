---
name: soc1-soc2-soc3-compliance-comparison
description: "Use when the user asks to compare SOC 1 vs SOC 2 vs SOC 3 compliance, choose the right SOC report, explain AICPA attestation reports, map SOC report types to business needs, or prepare executive, vendor-risk, sales, audit-readiness, or buyer-facing guidance about SOC reports."
license: MIT
metadata:
  author: Raj Desikavinayagompillai
  version: '1.0'
---

# SOC 1 vs SOC 2 vs SOC 3 Compliance Comparison

## When to Use This Skill

Use this skill when the user asks for help with:

- Comparing SOC 1, SOC 2, and SOC 3 reports.
- Choosing which SOC report an organization needs.
- Explaining SOC report differences to executives, customers, vendors, procurement, sales, security, legal, finance, or audit teams.
- Preparing audit-readiness guidance, evidence planning, buyer enablement language, vendor-risk responses, or public assurance messaging related to SOC reports.
- Mapping business models, services, control objectives, trust services criteria, internal control over financial reporting, or public assurance needs to SOC 1, SOC 2, and SOC 3.

Do not use this skill as a substitute for auditor, CPA, legal, or regulatory advice. If the user needs a formal audit opinion, scope determination, or reliance decision, recommend consulting a qualified CPA firm or auditor.

## Core Distinctions

Always anchor the comparison around the business question each report answers:

- **SOC 1**: Controls relevant to a user entity's internal control over financial reporting, often abbreviated as ICFR.
- **SOC 2**: Controls relevant to security, availability, processing integrity, confidentiality, and privacy, using the AICPA trust services criteria.
- **SOC 3**: A public-facing, general-use summary report covering the same trust services criteria domain as SOC 2, but without the detailed control descriptions, testing procedures, and results normally included in a SOC 2 report.

## Comparison Workflow

When producing a comparison, follow this sequence:

1. **Clarify the user's goal**
   - Identify whether they are trying to satisfy customers, support finance stakeholders, prepare for an audit, respond to procurement, publish assurance material, or decide which report to pursue.
   - Identify the organization type: SaaS, cloud provider, AI provider, payroll processor, payment processor, data processor, healthcare technology vendor, fintech provider, outsourced operations provider, or other service organization.
   - Identify the intended audience: customer auditors, customer finance teams, security/procurement teams, executives, general public, sales prospects, regulators, or internal leadership.

2. **Explain the report purpose**
   - For SOC 1, focus on financial reporting impact and controls that could affect customers' financial statements.
   - For SOC 2, focus on security and operational trust, especially the trust services criteria selected for scope.
   - For SOC 3, focus on broad public assurance and marketing-safe trust communication.

3. **Differentiate report use and distribution**
   - SOC 1 reports are restricted-use reports intended for management, user entities, and user auditors.
   - SOC 2 reports are generally restricted-use reports intended for management, customers, prospective customers under NDA, and other specified parties with a sufficient understanding of the services and controls.
   - SOC 3 reports are general-use reports suitable for public distribution, such as websites, trust centers, and marketing collateral, when supported by the underlying examination.

4. **Compare report content**
   - SOC 1 includes control objectives and related controls tied to financial reporting.
   - SOC 2 includes system description, applicable trust services criteria, controls, auditor tests, and test results.
   - SOC 3 includes a high-level description and auditor opinion suitable for public readers, usually omitting detailed tests and results.

5. **Discuss Type 1 vs Type 2**
   - Type 1 evaluates whether controls are suitably designed as of a point in time.
   - Type 2 evaluates whether controls are suitably designed and operating effectively over a period of time.
   - Explain that SOC 1 and SOC 2 can be Type 1 or Type 2. SOC 3 is commonly associated with a completed SOC 2-style examination and public assurance over the relevant trust services criteria.

6. **Give decision guidance**
   - Recommend SOC 1 when customers need assurance over controls that affect their financial reporting.
   - Recommend SOC 2 when customers need assurance over security, availability, confidentiality, processing integrity, or privacy controls.
   - Recommend SOC 3 when the organization already has or is pursuing SOC 2-level assurance and wants a public-facing report for broad distribution.
   - For organizations with both financial reporting impact and security/privacy expectations, explain that more than one report may be appropriate.

7. **Tailor the output**
   - For executives, keep the answer concise and decision-oriented.
   - For audit readiness, include scope, evidence, owners, timelines, control families, and auditor coordination.
   - For sales or customer success, include plain-English positioning and avoid overclaiming.
   - For vendor risk or procurement, map report type to buyer assurance needs and residual gaps.

## Standard Comparison Table

Use or adapt this table when the user asks for a direct comparison:

| Dimension | SOC 1 | SOC 2 | SOC 3 |
|---|---|---|---|
| Primary purpose | Assurance over controls relevant to customers' financial reporting | Assurance over controls relevant to trust services criteria | Public-facing assurance over trust services criteria |
| Main audience | Customer management and customer auditors | Customers, prospective customers, auditors, vendor-risk teams, and specified parties | General public, prospects, customers, website visitors, and trust center readers |
| Control focus | Financial reporting controls and control objectives | Security, availability, processing integrity, confidentiality, and privacy, depending on scope | Same trust services criteria domain as SOC 2, summarized for public use |
| Distribution | Restricted use | Usually restricted use | General use |
| Detail level | Detailed controls, tests, and results for financial-reporting objectives | Detailed system description, controls, tests, and results | Summary-level report without detailed testing detail |
| Common buyers/requesters | Finance teams, user auditors, customers with SOX or financial-statement reliance needs | Security, compliance, procurement, enterprise customers, vendor risk, legal | Prospects, website visitors, trust center users, marketing, executives |
| Best fit | Services that can materially affect customer financial statements | SaaS, cloud, data processing, AI, security, and technology services | Public trust signal after or alongside SOC 2 assurance |

## Decision Matrix

Use this matrix when the user asks which report they need:

| User need | Recommended report | Rationale |
|---|---|---|
| Customers ask whether the service impacts their financial statements | SOC 1 | The assurance focus is internal control over financial reporting |
| Enterprise customers ask about security controls | SOC 2 | The assurance focus is security and other selected trust services criteria |
| The company wants to publish a public trust report on its website | SOC 3 | SOC 3 is designed for general-use public distribution |
| The service handles payroll, claims, payment flows, transaction processing, or financial calculations for customers | SOC 1, and potentially SOC 2 | SOC 1 may address financial reporting reliance; SOC 2 may address security and confidentiality expectations |
| The service stores sensitive customer data but does not affect financial reporting | SOC 2 | Security, confidentiality, privacy, and availability are typically more relevant than ICFR |
| Customers request a detailed audit report under NDA | SOC 2 or SOC 1, depending on the control objective | Detailed restricted-use reports provide control descriptions and test results |
| Sales wants a short public assurance artifact | SOC 3, trust center summary, or SOC 2 bridge letter depending on maturity | Public messaging should not disclose restricted report details or overstate assurance |

## Recommended Output Formats

### Executive Summary

Use this structure for executive audiences:

1. One-sentence answer: which report fits the user's situation.
2. Three-bullet explanation of why.
3. Short comparison table.
4. Risks of choosing the wrong report.
5. Recommended next steps.

### Audit-Readiness Plan

Use this structure for readiness requests:

1. Target report and scope.
2. Stakeholders and report audience.
3. In-scope systems, services, locations, vendors, and subservice organizations.
4. Control domains or control objectives.
5. Evidence categories.
6. Gap assessment activities.
7. Auditor selection and timeline.
8. Customer communication plan.

### Buyer-Facing Explanation

Use this structure for customer or sales enablement:

1. Plain-English description of the report type.
2. What the report does cover.
3. What the report does not cover.
4. How customers may request or access the report.
5. Any NDA, trust center, or distribution limitations.

## Evidence Guidance

When the user asks about evidence, tailor evidence to the report type:

- **SOC 1 evidence**: Control objective narratives, transaction processing controls, reconciliations, review signoffs, change management, access controls over financial systems, job processing logs, exception handling, and user control considerations.
- **SOC 2 evidence**: Security policies, access reviews, vulnerability management, incident response, vendor management, change management, backup and recovery testing, monitoring, risk assessments, encryption, privacy processes, and system description support.
- **SOC 3 evidence**: Evidence usually comes from the underlying trust services examination. Focus on ensuring public claims match the auditor's report and do not include restricted SOC 2 detail unless approved.

## Guardrails

Follow these rules in every response:

- Do not say that SOC compliance is a certification. Prefer "SOC report," "SOC examination," or "SOC attestation report."
- Do not imply that SOC 3 is a lighter substitute for SOC 2 readiness. Explain that it is a public-facing report with less detail, not a replacement for underlying controls.
- Do not disclose or summarize restricted SOC 1 or SOC 2 report details for public use unless the user confirms they are preparing a controlled, authorized summary.
- Do not claim that one SOC report universally satisfies all customer requests. Tie recommendations to customer assurance needs.
- Do not provide legal, regulatory, or audit opinions. Use practical guidance and recommend auditor consultation where final scoping is needed.
- When discussing SOC 2, specify which trust services criteria are in scope rather than implying all criteria are automatically included.

## Example Responses

### If the user asks, "Which one do we need?"

Start with: "If customers rely on your service for financial reporting, prioritize SOC 1. If customers are asking about security, availability, confidentiality, processing integrity, or privacy, prioritize SOC 2. If you need a public-facing assurance artifact, SOC 3 is usually the add-on after SOC 2-level work."

Then tailor the recommendation to the user's service, buyer profile, and customer requests.

### If the user asks for a simple explanation

Use this short framing: "SOC 1 is for financial reporting reliance, SOC 2 is for security and operational trust, and SOC 3 is the public-facing version of trust services assurance."

### If the user asks for a sales-safe version

Use language like: "Our SOC report provides independent assurance over the controls in scope for the examination. Detailed SOC 1 or SOC 2 reports are typically shared with authorized customers under NDA, while SOC 3 reports are designed for broader public distribution."

Avoid language like: "We are SOC certified," "SOC 3 proves we are secure," or "SOC 2 covers every compliance requirement."
