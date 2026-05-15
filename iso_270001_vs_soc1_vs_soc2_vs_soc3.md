---
name: soc-iso-assurance-selection
description: "Use when comparing SOC 1, SOC 2, SOC 3, and ISO/IEC 27001; choosing which assurance framework or report a business should pursue; explaining SOC vs ISO differences; preparing executive, sales, procurement, vendor-risk, board, or audit-readiness guidance for SaaS, cloud, AI, fintech, payroll, outsourcing, or technology organizations."
license: MIT
metadata:
  version: '1.0'
  author: Raj Desikavinayagompillai
---

# SOC and ISO Assurance Selection

## When to Use This Skill

Use this skill when the user asks for help with:

- Comparing SOC 1, SOC 2, SOC 3, and ISO/IEC 27001.
- Deciding why a business should choose SOC 1, SOC 2, SOC 3, ISO 27001, or a combination.
- Explaining assurance options to executives, boards, procurement, sales, customer success, vendor-risk teams, security teams, finance teams, or auditors.
- Creating customer-facing or sales-safe language about a company’s compliance roadmap.
- Building an audit-readiness roadmap for SOC reports and ISO 27001 certification.
- Mapping business models such as SaaS, AI, cloud, fintech, payroll, payments, outsourcing, data processing, and managed services to the right assurance path.

Do not use this skill as a substitute for legal, CPA, certification body, or auditor advice. For final scoping, reliance, audit, or certification decisions, recommend that the user consult a qualified CPA firm, auditor, certification body, or counsel.

## Core Distinctions

Anchor every comparison around the business question each option answers:

- **SOC 1**: “Do our controls affect customers’ internal control over financial reporting?”
- **SOC 2**: “Can customers trust our controls over security, availability, processing integrity, confidentiality, or privacy?”
- **SOC 3**: “Can we publicly communicate high-level trust services assurance without sharing restricted SOC 2 detail?”
- **ISO/IEC 27001**: “Do we operate a certified, risk-based information security management system?”

Use precise terminology:

- ISO/IEC 27001 is a certifiable international management system standard for an information security management system, commonly called an ISMS.
- SOC 1, SOC 2, and SOC 3 are attestation reports, not certifications.
- SOC 1 and SOC 2 can be Type 1 or Type 2. Type 1 evaluates design at a point in time. Type 2 evaluates design and operating effectiveness over a period.
- SOC 1 and SOC 2 are commonly restricted-use reports.
- SOC 3 is a general-use report designed for public distribution.
- SOC 2 and SOC 3 use the AICPA trust services criteria. SOC 3 is less detailed than SOC 2 and does not replace SOC 2 when customers need detailed testing results.
- ISO 27001 certification requires an ISMS scope, risk assessment, risk treatment, Statement of Applicability, internal audit, management review, and certification audit process.

## Standard Workflow

### Clarify the business goal

Identify or infer the following:

- **Business model**: SaaS, cloud provider, AI provider, payroll processor, payment processor, fintech, data processor, healthcare technology vendor, managed services provider, outsourcing provider, or professional services firm.
- **Primary requester**: Customer finance teams, customer auditors, security and procurement teams, enterprise buyers, executives, regulators, sales prospects, or the general public.
- **Assurance objective**: Financial reporting reliance, security due diligence, vendor-risk approval, public trust signaling, international market access, formal security governance, customer contract requirements, or audit readiness.
- **Urgency**: Immediate sales blocker, upcoming customer due diligence, board decision, audit planning, or long-term assurance roadmap.
- **Customer wording**: Note whether customer requests specifically mention SOC 1, SOC 2, SOC 3, Type 1, Type 2, ISO 27001 certification, trust services criteria, ICFR, or public assurance.

If context is incomplete, state practical assumptions and give a default recommendation. Ask clarifying questions only when the missing detail would materially change the answer.

### Match the need to the right option

Use this decision logic:

- Recommend **SOC 1** when customers rely on the service for financial reporting, transaction processing, payroll, claims, payments, accounting calculations, revenue-impacting workflows, or other activities relevant to customer financial statements.
- Recommend **SOC 2** when customers need assurance over security, availability, processing integrity, confidentiality, or privacy, especially for SaaS, cloud, AI, data platforms, security vendors, and managed services.
- Recommend **SOC 3** when the company already has, or is pursuing, SOC 2-level trust services assurance and wants a public-facing report for a website, trust center, sales collateral, or broad market communication.
- Recommend **ISO 27001** when the business needs a globally recognized, risk-based security management system certification, especially for international customers, enterprise procurement, public sector expectations, and security governance maturity.
- Recommend **more than one** when business needs overlap. For example, a payroll platform may need SOC 1 for customer financial reporting reliance, SOC 2 for security and confidentiality assurance, and ISO 27001 for global security governance credibility.

### Compare tradeoffs

When comparing options, address:

- Primary purpose and business question.
- Buyer or requester.
- Control or management-system focus.
- Distribution and confidentiality.
- Evidence expectations.
- Time-to-value.
- Sales and market value.
- Audit or certification effort.
- Risks of choosing the wrong option.

Avoid presenting one option as universally better. The right choice depends on customer reliance, buyer expectations, market expectations, and scope.

### Recommend a path

Give a direct recommendation using language like:

- “Choose SOC 1 if…”
- “Choose SOC 2 if…”
- “Choose SOC 3 if…”
- “Choose ISO 27001 if…”
- “Choose both/all if…”

When appropriate, include a phased roadmap:

1. Immediate customer-response language.
2. Readiness or gap assessment.
3. Scope definition.
4. Control and evidence buildout.
5. Initial Type 1 report, SOC 2 readiness milestone, or ISO certification audit preparation.
6. Operating period for Type 2 reporting or ISO surveillance readiness.
7. Public trust center or SOC 3 messaging if supported by the underlying assurance work.

## Standard Comparison Table

Use or adapt this table for direct comparisons:

| Dimension | SOC 1 | SOC 2 | SOC 3 | ISO/IEC 27001 |
|---|---|---|---|---|
| Primary purpose | Assurance over controls relevant to customers’ financial reporting | Assurance over controls relevant to trust services criteria | Public-facing assurance over trust services criteria | Certification of a formal ISMS |
| Best business question | Could our service affect customers’ financial statements? | Can customers trust our security, availability, confidentiality, processing integrity, or privacy controls? | Can we publish a high-level assurance report publicly? | Do we manage information security through a risk-based management system? |
| Main audience | Customer finance teams, customer auditors, and user entities | Security, procurement, legal, vendor-risk teams, enterprise customers, and auditors | Prospects, customers, trust center visitors, and the general public | Enterprise customers, international buyers, procurement, regulators, security teams, and executives |
| Control focus | Financial reporting control objectives and related controls | Trust services criteria and related controls | Same trust services criteria domain as SOC 2, summarized | ISMS governance, risk management, Annex A controls, and continual improvement |
| Output | Restricted-use SOC 1 report | Usually restricted-use SOC 2 report | General-use SOC 3 report | Certificate and audit report from a certification body |
| Distribution | Restricted use | Usually restricted use | Public distribution | Certificate is commonly shareable; detailed audit materials may be controlled |
| Best fit | Payroll, payments, transaction processing, accounting, claims, and financial workflows | SaaS, cloud, AI, data platforms, security vendors, and managed services | Public trust signaling after or alongside SOC 2-level assurance | Global security governance, formal ISMS maturity, and international market expectations |
| Key risk if chosen incorrectly | Not useful for security-only due diligence | May not satisfy financial-reporting reliance needs | Too high-level for customers needing detailed testing | May not satisfy customers asking for detailed control test results |

## Decision Matrix

Use this matrix when the user asks which option a business should choose:

| Business situation | Recommended option | Rationale |
|---|---|---|
| Customers ask about controls affecting financial reporting | SOC 1 | SOC 1 is designed for controls relevant to user entities’ internal control over financial reporting |
| Enterprise customers ask for security due diligence or vendor-risk assurance | SOC 2 | SOC 2 addresses security and other selected trust services criteria |
| Marketing wants a public trust report | SOC 3 | SOC 3 is designed for general-use public distribution |
| International enterprise buyers ask for formal security certification | ISO 27001 | ISO 27001 demonstrates a certified, risk-based ISMS |
| A SaaS company stores sensitive customer data but does not affect financial statements | SOC 2, potentially ISO 27001 | SOC 2 addresses customer security assurance; ISO 27001 may help with global certification expectations |
| A payroll, payment, claims, or accounting platform supports customer financial processes | SOC 1 and likely SOC 2 | SOC 1 addresses financial reporting reliance; SOC 2 addresses security and confidentiality expectations |
| A company wants public assurance but has no SOC 2 readiness | SOC 2 first, then SOC 3 | SOC 3 should be supported by trust services examination work and should not be treated as a shortcut |
| A company wants a mature security operating model and customer audit evidence | ISO 27001 and SOC 2 | ISO 27001 supports security governance; SOC 2 supports detailed customer trust services assurance |

## Output Formats

### Executive recommendation

Use this structure for leadership audiences:

1. One-sentence recommendation.
2. Short rationale tied to business model and customer expectations.
3. Comparison table or decision matrix.
4. Risks of choosing the wrong option.
5. Recommended next steps.

### Audit-readiness roadmap

Use this structure for implementation planning:

1. Target framework, report, or combination.
2. Business rationale and primary requester.
3. Scope boundaries, systems, services, locations, vendors, and subservice organizations.
4. Required stakeholders.
5. Evidence categories.
6. Gap assessment activities.
7. Auditor, CPA firm, or certification body coordination.
8. Type 1, Type 2, certification, operating-period, or surveillance considerations.
9. Customer communication plan.

### Buyer-facing explanation

Use this structure for customer, sales, or vendor-risk responses:

1. Plain-English description of the chosen framework or report.
2. What it covers.
3. What it does not cover.
4. How customers can access the report, certificate, trust center, or summary.
5. Confidentiality, NDA, and distribution limitations.

### Board or leadership memo

Use this structure for strategic decisions:

1. Decision needed.
2. Business driver.
3. Options considered.
4. Recommended path.
5. Investment and effort considerations.
6. Customer, revenue, and risk impact.
7. Implementation roadmap.
8. Open questions for auditor, certification body, legal, or executive sponsor.

## Evidence Guidance

Tailor evidence guidance to the selected path:

- **SOC 1**: Control objective narratives, transaction processing controls, reconciliations, review signoffs, financial system access controls, job processing logs, exception handling, change management, and user control considerations.
- **SOC 2**: Security policies, system description support, access reviews, vulnerability management, incident response, vendor management, change management, backup and recovery testing, monitoring, encryption, risk assessments, and privacy processes where applicable.
- **SOC 3**: Evidence normally comes from the underlying trust services examination. Focus on ensuring public claims match the auditor’s report and do not disclose restricted SOC 2 detail.
- **ISO 27001**: ISMS scope, context of the organization, risk assessment, risk treatment plan, Statement of Applicability, security policies, objectives, competence and awareness records, internal audit, management review, corrective actions, and Annex A control evidence.

## Guardrails

Follow these guardrails in every output:

- Do not call SOC 1, SOC 2, or SOC 3 a certification. Use “SOC report,” “SOC examination,” or “attestation report.”
- Do not imply ISO 27001 automatically satisfies every SOC 2 customer request.
- Do not imply SOC 2 automatically satisfies ISO 27001 certification expectations.
- Do not imply SOC 3 is a shortcut or substitute for detailed SOC 2 assurance.
- Do not guarantee certification, audit success, auditor acceptance, or customer acceptance.
- Do not provide legal, regulatory, CPA, or audit opinions.
- Do not recommend sharing restricted SOC 1 or SOC 2 report details publicly.
- When discussing SOC 2, identify the trust services criteria in scope instead of implying all criteria are always included.
- When discussing ISO 27001, distinguish ISMS clauses from Annex A controls and state that scoping matters.
- When presenting a roadmap, note whether the recommendation is for immediate sales response, audit readiness, formal certification, or multi-year assurance maturity.

## Quality Checklist

Before finalizing an answer, verify that:

- The recommendation ties to the business model and customer request.
- SOC 1 is tied to financial reporting reliance.
- SOC 2 is tied to trust services criteria.
- SOC 3 is tied to public distribution and high-level assurance.
- ISO 27001 is described as a certifiable ISMS standard.
- Any multi-framework recommendation explains why more than one is needed.
- Confidentiality and distribution limitations are clear.
- Risks of choosing the wrong option are stated.
- Assumptions and open questions are listed where relevant.

## Example Prompts This Skill Should Handle

- “Compare SOC 1, SOC 2, SOC 3, and ISO 27001 for our executive team.”
- “Why should our business choose ISO 27001 instead of SOC 2?”
- “Should a SaaS company get SOC 2, ISO 27001, or both?”
- “Which compliance report should a payroll platform pursue first?”
- “Explain SOC 1 vs SOC 2 vs SOC 3 vs ISO 27001 for sales and procurement.”
- “Create a customer-facing explanation for why we have SOC 2 but not ISO 27001.”
- “Build a roadmap for SOC 2 Type 1, SOC 2 Type 2, SOC 3, and ISO 27001.”
- “What should we choose if customers keep asking for security assurance?”
