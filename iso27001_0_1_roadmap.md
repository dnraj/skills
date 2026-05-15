# ISO 27001 Implementation Roadmap and Control Matrix for a Managed Services Company

This document provides a practical ISO/IEC 27001:2022 implementation roadmap and managed-services-specific control matrix for an organization building an Information Security Management System from the ground up. It is designed for MSPs, MSSPs, cloud operations providers, IT outsourcing firms, help desk providers, monitoring teams, backup service providers, endpoint management providers, and organizations that administer customer environments.

## Assumptions

- The organization provides managed services involving customer system access, service desk operations, monitoring, remote administration, backup, patching, endpoint management, cloud operations, or similar services.
- The target framework is ISO/IEC 27001:2022.
- The organization is building toward certification readiness, but certification outcomes depend on the certification body, audit scope, actual implementation, and operating evidence.
- The scope, timelines, and control owners should be adjusted based on company size, service model, countries of operation, contractual commitments, cloud/on-premises environment, and customer requirements.

## ISMS Scope Definition

The first step is to define the certification boundary. For a managed services organization, the ISMS scope should explicitly describe the services, systems, people, locations, customer access model, and supporting third parties included in the Information Security Management System.

### Recommended Scope Statement

The Information Security Management System covers the people, processes, technology, facilities, and third-party services used to deliver managed services to customers, including service desk operations, remote administration, monitoring, endpoint management, patch management, backup operations, cloud operations, customer environment administration, internal business systems, security operations, and supporting infrastructure. The scope includes employees, contractors, remote workers, in-scope offices, cloud services, identity and access management systems, ticketing systems, RMM tools, documentation platforms, password vaults, monitoring tools, endpoint security tools, backup platforms, vendor platforms, and customer-facing operational processes used to deliver managed services.

### Scope Artifacts

| Artifact | Purpose | Owner | Review cadence |
|---|---|---|---|
| ISMS scope statement | Defines certification boundary | Executive sponsor / ISMS owner | Annual and upon major change |
| In-scope systems inventory | Identifies systems supporting managed services | IT/Security | Monthly or quarterly |
| Customer environment access register | Identifies customer systems and access paths | Managed services operations | Monthly or quarterly |
| Service catalog | Defines in-scope services and service owners | Managed services leadership | Quarterly |
| Vendor register | Identifies third parties supporting in-scope services | Procurement / operations | Quarterly |
| Data inventory | Identifies customer, personal, confidential, and operational data | Security / privacy / operations | Quarterly |

## Governance Model

ISO 27001 should be governed as an operating program. The organization should define accountability, decision-making forums, control ownership, reporting metrics, and escalation paths.

| Role | Responsibility |
|---|---|
| Executive sponsor | Approves ISMS scope, policy, objectives, resources, and risk acceptance |
| ISMS owner | Owns ISO 27001 program execution, risk process, SoA, evidence readiness, and audit coordination |
| Security lead | Owns security controls, incident response, vulnerability management, logging, monitoring, and access standards |
| Managed services leader | Owns service delivery controls, customer access, change management, patching, backup operations, and SLA evidence |
| IT operations | Operates internal systems, endpoint controls, backups, identity, network, and cloud infrastructure |
| HR | Owns screening, onboarding, awareness training, disciplinary process, and offboarding triggers |
| Procurement / vendor owner | Owns vendor due diligence, contracts, and supplier monitoring |
| Control owners | Operate assigned controls and maintain evidence |
| Internal auditor | Independently reviews ISMS conformity and control operation |

## Implementation Roadmap

### Phase Summary

| Phase | Timeline | Objective | Key activities | Primary deliverables | Audit focus |
|---|---:|---|---|---|---|
| Foundation | Weeks 1-2 | Establish scope, governance, and accountability | Define scope, interested parties, roles, objectives, ISMS governance cadence | Scope statement, governance charter, RACI, information security policy | Clauses 4, 5, and 6 |
| Risk and SoA | Weeks 3-5 | Build risk-based control foundation | Define risk methodology, perform risk assessment, create treatment plan, draft SoA | Risk methodology, risk register, risk treatment plan, Statement of Applicability | Clauses 6 and 8 |
| Policy and Process Design | Weeks 6-8 | Define documented control expectations | Draft core policies, procedures, standards, control narratives, evidence requirements | Policy set, procedures, control matrix, evidence plan | Clauses 7 and 8 |
| Control Implementation | Weeks 9-12 | Configure and operationalize high-priority controls | MFA, access reviews, PAM, RMM hardening, logging, change workflow, vulnerability tracking, backup monitoring | Configurations, inventories, workflows, implementation evidence | Annex A control implementation |
| Operating Evidence | Weeks 13-18 | Run controls consistently and retain evidence | Access reviews, patch reviews, vendor reviews, backup tests, incident tabletop, training, change reviews | Completed tickets, sign-offs, logs, metrics, training records, test results | Stage 2 operating effectiveness |
| Internal Assurance | Weeks 19-21 | Validate readiness before certification audit | Internal audit, management review, corrective action planning | Internal audit report, management review minutes, corrective action tracker | Clauses 9 and 10 |
| Certification Readiness | Weeks 22-24 | Prepare audit package and remediate final gaps | Evidence QA, pre-assessment, final SoA update, risk review, audit logistics | Stage 1 and Stage 2 audit package | Certification readiness |

### Phase Details

#### Foundation

| Activity | Description | Output | Owner |
|---|---|---|---|
| Define ISMS scope | Identify included services, systems, locations, people, vendors, and customer access paths | Approved scope statement | Executive sponsor / ISMS owner |
| Identify interested parties | Document customer, regulator, contractual, vendor, employee, and leadership requirements | Interested parties register | ISMS owner |
| Assign ISMS roles | Define control owners and accountability | ISMS RACI | Executive sponsor |
| Establish governance cadence | Create monthly ISMS steering meeting and quarterly management review cadence | Governance calendar | ISMS owner |
| Approve security policy | Create high-level information security policy | Approved policy | Executive sponsor |

#### Risk and SoA

| Activity | Description | Output | Owner |
|---|---|---|---|
| Define risk methodology | Define likelihood, impact, risk rating, treatment options, and acceptance authority | Risk methodology | ISMS owner |
| Build asset and service inventory | List systems, services, data types, vendors, and customer access models | Asset, service, vendor, and data inventories | IT/Security/Operations |
| Conduct risk assessment | Evaluate risks to managed services operations and customer environments | Risk register | ISMS owner / security |
| Create risk treatment plan | Select controls, owners, target dates, and residual risk decisions | Risk treatment plan | ISMS owner |
| Draft Statement of Applicability | Determine Annex A applicability, justification, implementation status, and evidence | SoA | ISMS owner / security |

#### Policy and Process Design

| Policy or procedure | Purpose | Owner |
|---|---|---|
| Information Security Policy | Sets ISMS direction and leadership commitment | Executive sponsor |
| Access Control Policy | Defines access lifecycle, least privilege, MFA, reviews, and privileged access | Security / IT |
| Customer Environment Access Procedure | Defines how staff access customer systems and how access is approved, reviewed, and removed | Managed services operations |
| Privileged Access Management Procedure | Defines privileged account approval, vaulting, monitoring, emergency access, and review | Security / IT |
| Change Management Procedure | Defines normal, standard, and emergency changes, approvals, testing, rollback, and customer approval | Managed services operations |
| Vulnerability and Patch Management Procedure | Defines scanning, severity ratings, remediation SLAs, exception handling, and reporting | Security / operations |
| Incident Response Plan | Defines triage, escalation, customer notification, evidence preservation, and lessons learned | Security |
| Backup and Recovery Procedure | Defines backup scope, frequency, monitoring, retention, restore testing, and failure response | IT / operations |
| Supplier Management Procedure | Defines vendor due diligence, risk tiering, contract requirements, and annual reviews | Procurement / operations |
| Logging and Monitoring Procedure | Defines log sources, alerting, review cadence, retention, and escalation | Security |
| Data Classification and Handling Policy | Defines handling of customer data, credentials, screenshots, logs, tickets, and confidential data | Security / privacy |
| Business Continuity Plan | Defines continuity for service delivery and critical platforms | Operations / leadership |
| HR Security Procedure | Defines screening, onboarding, training, role changes, and offboarding | HR |

#### Control Implementation

Priority implementation areas for managed services:

| Area | Implementation focus |
|---|---|
| Identity and access | MFA, SSO, least privilege, access request workflow, quarterly access reviews |
| Privileged access | Named admin accounts, password vault, PAM, break-glass controls, logging, customer admin review |
| RMM and remote access | MFA, IP restrictions where feasible, role-based access, session logging, vendor security review |
| Customer access | Customer-specific authorization, access register, approval records, segregation between customer environments |
| Ticketing and documentation | Role-based access, data handling rules, retention, restricted credential storage |
| Change management | Approval workflow, testing, rollback, emergency change review, customer approval where required |
| Vulnerability management | Scanning, remediation SLAs, patch reports, exception approvals, metrics |
| Backup and recovery | Backup monitoring, restore testing, failed backup remediation, retention requirements |
| Incident response | Escalation paths, incident categories, customer notification criteria, tabletop exercise |
| Vendor management | Critical vendor due diligence, contract security requirements, annual review |
| Logging and monitoring | Identity, RMM, cloud console, ticketing, VPN, EDR, backup, and admin logs |

#### Operating Evidence

The organization should collect evidence continuously. Evidence should be retained in a structured repository with folders by control area, month or quarter, and evidence type.

| Evidence area | Examples |
|---|---|
| Access management | Access requests, approvals, access review exports, reviewer sign-offs, remediation tickets |
| Privileged access | Privileged user inventory, PAM logs, break-glass access reviews, admin session logs |
| Customer access | Customer access matrix, customer approvals, remote access logs, offboarding records |
| Change management | Change tickets, approvals, testing evidence, rollback plans, emergency change reviews |
| Vulnerability management | Scan reports, patch reports, remediation tickets, exception approvals, SLA dashboards |
| Backup and recovery | Backup success reports, failed backup tickets, restore test evidence, retention settings |
| Incident response | Incident tickets, severity classification, communications, post-incident reviews, tabletop records |
| Vendor management | Vendor register, risk assessments, SOC/ISO reports, security questionnaires, review records |
| Awareness and HR | Training completion, onboarding records, offboarding tickets, policy acknowledgments |
| Governance | ISMS meeting minutes, management review minutes, metrics, internal audit report, corrective actions |

## Managed Services Risk Register Starter

| Risk ID | Risk scenario | Inherent risk | Treatment decision | Selected controls | Residual risk target | Risk owner |
|---|---|---:|---|---|---|---|
| R-001 | Unauthorized access to customer environments due to excessive permissions | Critical | Mitigate | MFA, least privilege, access approval, quarterly access reviews, logging | Medium | Security / operations |
| R-002 | RMM or remote access platform compromise impacts multiple customers | Critical | Mitigate | MFA, RBAC, hardening, monitoring, vendor review, incident playbook | Medium | Security |
| R-003 | Former employee retains access to internal or customer systems | High | Mitigate | JML workflow, HR trigger, offboarding checklist, access removal validation | Low | HR / IT |
| R-004 | Unapproved customer-impacting change causes service outage | High | Mitigate | Change approval, testing, rollback, emergency review, customer approval | Medium | Managed services operations |
| R-005 | Critical vulnerabilities are not remediated within customer or internal SLA | High | Mitigate | Scanning, patch SLAs, remediation tracking, exception approval | Medium | Security / operations |
| R-006 | Customer data is exposed through ticket attachments, screenshots, or documentation | High | Mitigate | Data handling policy, restricted access, retention, awareness training | Medium | Service desk / security |
| R-007 | Failed backups are not detected or restores are unsuccessful | High | Mitigate | Backup monitoring, failure tickets, restore testing, recovery metrics | Medium | IT operations |
| R-008 | Critical vendor platform suffers a security incident affecting service delivery | High | Transfer / mitigate | Vendor due diligence, contracts, monitoring, incident notification requirements | Medium | Procurement / operations |
| R-009 | Security incidents are not escalated or customers are not notified timely | High | Mitigate | Incident response plan, escalation matrix, customer notification criteria, tabletop testing | Medium | Security |
| R-010 | Inadequate segregation between customer environments causes cross-customer exposure | Critical | Mitigate | RBAC, tenant segregation, access matrix, technical configuration review | Medium | Security / operations |

## ISO 27001 Managed Services Control Matrix

| Control ID | ISO reference | Control area | Managed services control activity | Owner | Frequency | Evidence | Evidence type | Priority |
|---|---|---|---|---|---|---|---|---|
| ISO-MS-001 | Clause 4.3 | ISMS scope | Define and approve an ISMS scope covering managed services, customer access, in-scope systems, people, locations, vendors, and exclusions | Executive sponsor / ISMS owner | Annual and upon major change | Scope statement, in-scope systems list, service catalog | Design | Critical |
| ISO-MS-002 | Clause 4.2 | Interested parties | Maintain a register of customer, contractual, regulatory, vendor, employee, and leadership information security requirements | ISMS owner | Annual and upon major change | Interested parties register, contract requirement summary | Design | High |
| ISO-MS-003 | Clause 5.2 | Information security policy | Approve and communicate an information security policy aligned to managed services risks and customer commitments | Executive sponsor | Annual | Approved policy, employee acknowledgment | Design / operating effectiveness | High |
| ISO-MS-004 | Clause 5.3 | Roles and responsibilities | Assign ISMS roles, control owners, risk owners, incident roles, and service delivery security responsibilities | Executive sponsor / ISMS owner | Annual and upon change | RACI, role descriptions, governance charter | Design | High |
| ISO-MS-005 | Clause 6.1 | Risk assessment | Perform information security risk assessments covering managed services operations, customer environments, vendors, and critical tools | ISMS owner / security | Annual and upon major change | Risk methodology, risk register, assessment records | Design / operating effectiveness | Critical |
| ISO-MS-006 | Clause 6.1 | Risk treatment | Maintain a risk treatment plan tying risks to selected controls, owners, due dates, and residual risk decisions | ISMS owner | Quarterly | Risk treatment plan, risk acceptance approvals | Operating effectiveness | Critical |
| ISO-MS-007 | Clause 6.1.3 | Statement of Applicability | Maintain an SoA showing applicable Annex A controls, justification, status, linked risks, and evidence | ISMS owner | Quarterly and upon major change | Statement of Applicability | Design / operating effectiveness | Critical |
| ISO-MS-008 | Clause 6.2 | Security objectives | Define measurable security objectives for access reviews, vulnerabilities, backup success, incident response, training, and vendor reviews | Leadership / ISMS owner | Quarterly | Objectives dashboard, metrics reports | Operating effectiveness | High |
| ISO-MS-009 | Clause 7.2 | Competence | Ensure staff performing managed services have appropriate technical and security competence | HR / operations | Upon hire and annually | Training records, role requirements, competency records | Operating effectiveness | Medium |
| ISO-MS-010 | Clause 7.3 | Awareness | Provide security awareness training covering customer data handling, phishing, incident reporting, remote access, and credential protection | HR / security | Upon hire and annually | Training completion reports, policy acknowledgments | Operating effectiveness | High |
| ISO-MS-011 | Clause 7.5 | Documented information | Control ISMS documents, policies, procedures, evidence retention, versioning, and approvals | ISMS owner | Ongoing | Document register, approval history, retention rules | Design / operating effectiveness | High |
| ISO-MS-012 | Clause 8.1 | Operational planning | Plan and control managed services processes needed to meet security requirements and risk treatment plans | Operations / ISMS owner | Ongoing | Process maps, SOPs, service delivery controls | Design | High |
| ISO-MS-013 | Clause 9.1 | Monitoring and measurement | Monitor ISMS metrics including access review completion, patch SLA, incidents, backup success, training, and vendor reviews | ISMS owner | Monthly / quarterly | Metrics dashboard, ISMS meeting minutes | Operating effectiveness | High |
| ISO-MS-014 | Clause 9.2 | Internal audit | Conduct internal audits of the ISMS and managed services controls using independent reviewers | Internal auditor | Annual | Internal audit plan, checklist, report, findings | Operating effectiveness | Critical |
| ISO-MS-015 | Clause 9.3 | Management review | Conduct management reviews covering ISMS performance, risks, incidents, objectives, audit results, and resource needs | Executive sponsor / ISMS owner | At least annual; recommended quarterly | Management review agenda, minutes, action items | Operating effectiveness | Critical |
| ISO-MS-016 | Clause 10.1 | Nonconformity and corrective action | Track nonconformities, control failures, audit findings, root cause, corrective actions, and closure evidence | ISMS owner | Ongoing | Corrective action tracker, closure evidence | Operating effectiveness | Critical |
| ISO-MS-017 | Annex A organizational controls | Security roles | Define security responsibilities for service desk, cloud operations, backup, monitoring, and customer administration | ISMS owner / operations | Annual | RACI, job descriptions, SOP ownership | Design | High |
| ISO-MS-018 | Annex A organizational controls | Segregation of duties | Segregate duties for access approval, privileged access operation, change approval, and control review where feasible | Security / operations | Annual / quarterly review | Role matrix, access review records | Design / operating effectiveness | High |
| ISO-MS-019 | Annex A organizational controls | Contact with authorities | Maintain procedures for contacting law enforcement, regulators, CERTs, or other authorities when incidents require escalation | Security / legal | Annual | Incident response plan, contact list | Design | Medium |
| ISO-MS-020 | Annex A organizational controls | Threat intelligence | Monitor relevant threat information affecting MSPs, RMM tools, cloud services, customer administration, and critical vendors | Security | Weekly / monthly | Threat bulletins, review notes, action tickets | Operating effectiveness | Medium |
| ISO-MS-021 | Annex A organizational controls | Asset inventory | Maintain an inventory of internal systems, managed services platforms, customer access tools, endpoints, cloud assets, and data stores | IT / security | Monthly / quarterly | Asset inventory export, review records | Operating effectiveness | Critical |
| ISO-MS-022 | Annex A organizational controls | Acceptable use | Define acceptable use for company devices, customer systems, remote access, credentials, and collaboration tools | HR / security | Annual | Acceptable use policy, acknowledgments | Design / operating effectiveness | High |
| ISO-MS-023 | Annex A organizational controls | Return of assets | Recover company devices, tokens, credentials, and access during employee and contractor offboarding | HR / IT | Upon termination | Offboarding checklist, asset return record | Operating effectiveness | High |
| ISO-MS-024 | Annex A organizational controls | Information classification | Classify customer data, credentials, tickets, logs, screenshots, configuration data, and internal confidential data | Security / data owners | Annual | Data classification policy, data inventory | Design | High |
| ISO-MS-025 | Annex A organizational controls | Information handling | Define handling rules for customer data in tickets, documentation, screenshots, logs, backups, and communications | Security / operations | Annual and ongoing | Data handling policy, training, ticket review records | Design / operating effectiveness | Critical |
| ISO-MS-026 | Annex A organizational controls | Access control policy | Maintain access control requirements for internal systems, customer systems, least privilege, MFA, privileged access, and periodic reviews | Security / IT | Annual | Access control policy, review evidence | Design / operating effectiveness | Critical |
| ISO-MS-027 | Annex A organizational controls | Identity management | Maintain unique user identities for employees and contractors across internal systems and customer access platforms where feasible | IT / security | Ongoing | User directory export, IAM configuration | Implementation | Critical |
| ISO-MS-028 | Annex A organizational controls | Authentication information | Protect passwords, API keys, secrets, recovery codes, and customer credentials using approved vaulting and rotation processes | IT / security | Ongoing | Password vault configuration, secret inventory, rotation records | Implementation / operating effectiveness | Critical |
| ISO-MS-029 | Annex A organizational controls | Access rights | Approve, provision, review, modify, and revoke access to internal and customer systems based on business need | IT / security / operations | Ongoing; quarterly review | Access requests, approvals, access review records, remediation tickets | Operating effectiveness | Critical |
| ISO-MS-030 | Annex A organizational controls | Supplier relationships | Risk-rank suppliers supporting managed services, including RMM, PSA, cloud, backup, EDR, SIEM, and subcontractors | Procurement / operations | Upon onboarding and annually | Vendor register, risk ratings, due diligence records | Operating effectiveness | Critical |
| ISO-MS-031 | Annex A organizational controls | Supplier agreements | Include confidentiality, security, incident notification, access control, data protection, and audit/right-to-review terms in critical supplier agreements | Procurement / legal | Upon contract and renewal | Contracts, security addenda, review checklist | Design / implementation | High |
| ISO-MS-032 | Annex A organizational controls | ICT supply chain | Assess supply chain risks for critical managed services platforms and subcontractors | Procurement / security | Annual | Supplier security reviews, risk treatment actions | Operating effectiveness | High |
| ISO-MS-033 | Annex A organizational controls | Cloud services | Approve, configure, monitor, and periodically review cloud services used for managed services delivery | IT / security | Ongoing; annual review | Cloud inventory, configuration baselines, access reviews | Implementation / operating effectiveness | High |
| ISO-MS-034 | Annex A organizational controls | Incident management | Maintain incident response procedures covering internal incidents, customer-impacting incidents, escalation, communications, and lessons learned | Security | Annual and upon incident | Incident response plan, incident tickets, PIRs | Design / operating effectiveness | Critical |
| ISO-MS-035 | Annex A organizational controls | Incident reporting | Require employees to report suspected incidents, credential exposure, customer data mishandling, and suspicious activity | Security / HR | Ongoing | Training, reporting channel, incident records | Operating effectiveness | High |
| ISO-MS-036 | Annex A organizational controls | Business continuity | Maintain continuity plans for critical managed services platforms, staff availability, customer support, monitoring, backup, and incident response | Operations / leadership | Annual and after major change | BCP, test results, continuity review | Design / operating effectiveness | High |
| ISO-MS-037 | Annex A organizational controls | Legal and contractual compliance | Track customer contractual security requirements, regulatory obligations, data protection commitments, and audit obligations | Legal / ISMS owner | Annual and contract review | Obligations register, contract summaries | Design / operating effectiveness | High |
| ISO-MS-038 | Annex A people controls | Screening | Perform pre-employment or contractor screening appropriate to role risk and permitted by law | HR | Upon hire | Screening records or attestations | Operating effectiveness | Medium |
| ISO-MS-039 | Annex A people controls | Terms of employment | Include confidentiality, acceptable use, security responsibility, and customer data protection obligations in employment or contractor agreements | HR / legal | Upon hire and contract change | Employment terms, contractor agreements | Design / implementation | High |
| ISO-MS-040 | Annex A people controls | Security awareness | Train personnel on customer data handling, privileged access, phishing, remote work, incident reporting, and secure service delivery | HR / security | Upon hire and annually | Training completion reports | Operating effectiveness | High |
| ISO-MS-041 | Annex A people controls | Disciplinary process | Define disciplinary consequences for security policy violations, credential misuse, unauthorized access, or customer data mishandling | HR / legal | Annual | Disciplinary policy, case records if applicable | Design / operating effectiveness | Medium |
| ISO-MS-042 | Annex A people controls | Remote work | Secure remote work through endpoint controls, VPN or secure access, MFA, device encryption, and acceptable use rules | IT / security | Ongoing | Remote work policy, endpoint compliance reports | Implementation / operating effectiveness | High |
| ISO-MS-043 | Annex A physical controls | Secure areas | Restrict physical access to offices, equipment rooms, and areas where customer or confidential information is handled | Facilities / IT | Ongoing; periodic review | Badge reports, access lists, review records | Operating effectiveness | Medium |
| ISO-MS-044 | Annex A physical controls | Equipment security | Protect laptops, network equipment, backup media, and endpoint devices from loss, theft, damage, or unauthorized access | IT / facilities | Ongoing | Asset inventory, encryption reports, MDM records | Implementation / operating effectiveness | High |
| ISO-MS-045 | Annex A physical controls | Secure disposal | Sanitize or securely dispose of devices, media, printed materials, and storage containing customer or confidential data | IT / facilities | Upon disposal | Disposal certificates, wipe records | Operating effectiveness | High |
| ISO-MS-046 | Annex A technological controls | Endpoint protection | Deploy and monitor endpoint security controls such as EDR/AV, disk encryption, screen lock, and device compliance | IT / security | Ongoing | EDR reports, MDM compliance, encryption reports | Implementation / operating effectiveness | Critical |
| ISO-MS-047 | Annex A technological controls | MFA | Enforce MFA for identity provider, email, cloud consoles, RMM, PSA/ticketing, VPN, remote access, password vault, and privileged systems | IT / security | Ongoing; quarterly review | MFA configuration, user coverage report | Implementation / operating effectiveness | Critical |
| ISO-MS-048 | Annex A technological controls | Privileged access management | Control privileged internal and customer access through approval, least privilege, vaulting, monitoring, and review | Security / IT | Ongoing; quarterly review | PAM records, privileged user list, access approvals, review sign-offs | Operating effectiveness | Critical |
| ISO-MS-049 | Annex A technological controls | Customer environment access | Maintain customer-specific access authorization, access paths, approval records, and periodic recertification | Managed services operations | Ongoing; quarterly review | Customer access matrix, access tickets, customer approvals | Operating effectiveness | Critical |
| ISO-MS-050 | Annex A technological controls | Joiner-mover-leaver | Provision, modify, and remove access based on HR or contractor lifecycle events, including customer systems and service tools | HR / IT / operations | Per event | Onboarding/offboarding tickets, access removal evidence | Operating effectiveness | Critical |
| ISO-MS-051 | Annex A technological controls | RMM and remote access hardening | Harden remote management tools with MFA, RBAC, least privilege, logging, restricted integrations, and administrative review | Security / operations | Quarterly | RMM configuration, admin list, hardening checklist, logs | Implementation / operating effectiveness | Critical |
| ISO-MS-052 | Annex A technological controls | Secure authentication | Apply strong authentication standards including password policy, SSO, session timeout, lockout, and conditional access where feasible | IT / security | Ongoing | IAM configuration, conditional access policy | Implementation | High |
| ISO-MS-053 | Annex A technological controls | Malware protection | Protect endpoints and servers with malware protection and alert handling | IT / security | Ongoing | EDR dashboard, alert tickets, remediation records | Operating effectiveness | High |
| ISO-MS-054 | Annex A technological controls | Vulnerability management | Identify, assess, prioritize, remediate, and track vulnerabilities across internal systems and managed services platforms | Security / operations | Continuous; monthly review | Scan reports, remediation tickets, exception approvals, SLA metrics | Operating effectiveness | Critical |
| ISO-MS-055 | Annex A technological controls | Patch management | Deploy patches according to severity-based SLAs for internal systems and customer-managed systems where contractually responsible | Operations / IT | Monthly or risk-based | Patch reports, deployment records, exception approvals | Operating effectiveness | Critical |
| ISO-MS-056 | Annex A technological controls | Configuration management | Maintain secure configuration baselines for endpoints, servers, network devices, cloud services, RMM, and backup platforms | IT / security | Quarterly | Baselines, configuration reports, exception records | Implementation / operating effectiveness | High |
| ISO-MS-057 | Annex A technological controls | Change management | Approve, test, implement, validate, and review changes to internal and customer systems, including emergency changes | Operations | Per change | Change tickets, approvals, test evidence, rollback plans | Operating effectiveness | Critical |
| ISO-MS-058 | Annex A technological controls | Backup | Back up critical internal systems, service delivery data, configurations, and customer systems where contractually responsible | IT / operations | Per backup schedule | Backup configuration, backup success reports, failure tickets | Operating effectiveness | Critical |
| ISO-MS-059 | Annex A technological controls | Restore testing | Test restoration of critical backups and document results, failures, and corrective actions | IT / operations | Quarterly or semiannual | Restore test records, screenshots, tickets | Operating effectiveness | High |
| ISO-MS-060 | Annex A technological controls | Logging | Enable logs for identity provider, RMM, PSA/ticketing, cloud consoles, VPN, EDR, backup, privileged access, and critical systems | Security / IT | Ongoing | Log source inventory, SIEM configuration, retention settings | Implementation | Critical |
| ISO-MS-061 | Annex A technological controls | Monitoring and alerting | Review security alerts and operational alerts for suspicious activity, backup failures, privileged activity, and service-impacting events | Security / operations | Daily / weekly | Alert tickets, review logs, escalation records | Operating effectiveness | Critical |
| ISO-MS-062 | Annex A technological controls | Network security | Protect internal and service delivery networks using segmentation, firewalls, secure remote access, and monitoring | IT / security | Ongoing; quarterly review | Network diagrams, firewall rules, VPN configuration | Implementation / operating effectiveness | High |
| ISO-MS-063 | Annex A technological controls | Data loss prevention | Protect customer and confidential data from unauthorized sharing through access controls, awareness, monitoring, and approved storage locations | Security / IT | Ongoing | DLP settings if used, ticket reviews, storage access controls | Implementation / operating effectiveness | Medium |
| ISO-MS-064 | Annex A technological controls | Secure development and scripts | Review and control operational scripts, automation, integrations, and infrastructure code used in service delivery | Operations / engineering | Per change | Code reviews, change tickets, repository permissions | Operating effectiveness | Medium |
| ISO-MS-065 | Annex A technological controls | Test data | Prevent unauthorized use of customer production data in test, demo, or troubleshooting environments unless approved and protected | Operations / security | Ongoing | Data handling procedure, approvals, masking records | Design / operating effectiveness | High |
| ISO-MS-066 | Annex A technological controls | Capacity and availability | Monitor capacity and availability of critical managed services platforms and internal systems | Operations | Ongoing; monthly review | Monitoring dashboards, capacity reviews, incident tickets | Operating effectiveness | Medium |
| ISO-MS-067 | Annex A technological controls | Secure information transfer | Protect transfer of customer data, logs, screenshots, credentials, and reports using approved encrypted channels | Operations / security | Ongoing | Secure transfer procedure, tool configuration, training | Design / implementation | High |
| ISO-MS-068 | Annex A technological controls | Deletion and retention | Define retention and deletion requirements for tickets, logs, screenshots, backups, documentation, and customer data | Security / legal / operations | Annual and per event | Retention schedule, deletion logs, system settings | Design / operating effectiveness | High |
| ISO-MS-069 | Annex A technological controls | Clock synchronization | Synchronize clocks across logging, monitoring, endpoint, cloud, and infrastructure systems to support incident investigation | IT / security | Ongoing | NTP configuration, system settings | Implementation | Medium |
| ISO-MS-070 | Annex A technological controls | Technical compliance review | Periodically review systems against security baselines, policy requirements, customer commitments, and regulatory obligations | Security / IT | Quarterly / annual | Compliance review reports, remediation tickets | Operating effectiveness | High |

## Stage 1 Audit Readiness Checklist

Stage 1 generally focuses on ISMS design and documented readiness.

| Area | Evidence to prepare |
|---|---|
| Scope | ISMS scope statement, in-scope systems, services, locations, exclusions |
| Context | Interested parties, internal/external issues, requirements register |
| Leadership | Information security policy, roles and responsibilities, governance records |
| Planning | Risk methodology, risk register, risk treatment plan, Statement of Applicability |
| Support | Competence records, awareness plan, communication plan, document control process |
| Operations | Core policies, procedures, control design, asset inventory, vendor register |
| Performance evaluation | Internal audit plan, metrics approach, management review plan |
| Improvement | Corrective action process, nonconformity procedure |

## Stage 2 Audit Readiness Checklist

Stage 2 generally focuses on whether controls are operating effectively.

| Area | Evidence to prepare |
|---|---|
| Access reviews | Completed access reviews, sign-offs, remediation tickets |
| Privileged access | Admin account list, approval records, PAM logs, break-glass review |
| Customer access | Customer access matrix, customer approvals, recertification records |
| Offboarding | Termination samples, access removal evidence, asset return evidence |
| Change management | Change samples, approvals, testing, rollback, emergency review |
| Vulnerability management | Scan reports, remediation tickets, exceptions, SLA metrics |
| Patch management | Patch reports, deployment evidence, failed patch follow-up |
| Backup and recovery | Backup success reports, restore test evidence, failure remediation |
| Incident response | Incident tickets, post-incident reviews, tabletop exercise |
| Logging and monitoring | Log source inventory, alert tickets, review records |
| Vendor management | Vendor reviews, security reports, risk ratings, contracts |
| Awareness | Training completion, policy acknowledgment |
| Internal audit | Audit report, findings, corrective actions |
| Management review | Meeting minutes, metrics reviewed, decisions, action items |

## Evidence Repository Structure

Use a consistent evidence repository structure so audit evidence can be produced quickly.

```text
ISO-27001-Evidence/
  01-Scope-and-Governance/
  02-Risk-Management/
  03-Statement-of-Applicability/
  04-Policies-and-Procedures/
  05-Asset-and-Data-Inventory/
  06-Access-Control/
  07-Privileged-and-Customer-Access/
  08-Change-Management/
  09-Vulnerability-and-Patch-Management/
  10-Backup-and-Recovery/
  11-Incident-Response/
  12-Logging-and-Monitoring/
  13-Vendor-Management/
  14-HR-and-Training/
  15-Business-Continuity/
  16-Internal-Audit/
  17-Management-Review/
  18-Corrective-Actions/
```

## Recommended 90-Day Quick Start

| Days | Focus | Actions | Outputs |
|---:|---|---|---|
| 1-15 | Scope and governance | Define ISMS scope, assign owners, approve security policy, build service and system inventory | Scope, policy, RACI, inventory |
| 16-30 | Risk foundation | Run risk assessment, create treatment plan, draft SoA | Risk register, treatment plan, SoA |
| 31-45 | Core controls | Implement MFA, access requests, privileged access control, customer access register, offboarding workflow | Access control evidence, customer access matrix |
| 46-60 | Operational controls | Formalize change, vulnerability, patch, backup, incident, logging, vendor, and data handling processes | Procedures, ticket workflows, vendor register |
| 61-75 | Evidence operation | Run access reviews, patch reviews, backup tests, vendor reviews, training, incident tabletop | Operating evidence |
| 76-90 | Readiness validation | Conduct internal readiness review, update SoA and risk register, create corrective action plan | Readiness report, CAPA tracker |

## Practical Success Criteria

The organization is approaching ISO 27001 readiness when:

- The ISMS scope is approved and matches actual managed services operations.
- Risks are documented, rated, treated, assigned to owners, and reviewed.
- The SoA is complete, risk-based, and supported by evidence.
- Policies and procedures reflect how teams actually work.
- Privileged and customer access is approved, reviewed, logged, and removed timely.
- RMM, remote access, ticketing, backup, and cloud platforms are hardened and monitored.
- Change, vulnerability, patch, incident, backup, vendor, and HR controls produce repeatable evidence.
- Internal audit and management review have been performed.
- Corrective actions are tracked to closure.
- Evidence can be retrieved quickly and tied to each control.

