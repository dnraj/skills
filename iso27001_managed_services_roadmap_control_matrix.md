# ISO 27001 Implementation Roadmap and Managed Services Control Matrix

Prepared for: Managed services, MSP, MSSP, IT outsourcing, or cloud operations organization  
Standard baseline: ISO/IEC 27001:2022  
Purpose: Build an Information Security Management System from the ground up and prepare for ISO 27001 audit readiness

## Important note

This document is an implementation and audit-readiness guide. It does not guarantee certification, and the organization should confirm final scope, evidence expectations, and audit interpretation with its certification body, internal leadership, legal counsel, and external auditor as appropriate.

## Source references

ISO describes ISO/IEC 27001 as the standard that defines requirements for an information security management system and supports a risk-based approach to protecting information assets ([ISO](https://www.iso.org/standard/27001)). ISO/IEC 27002:2022 provides the reference set of information security controls that support ISO 27001 risk treatment and control implementation ([ISO](https://www.iso.org/standard/75652.html)). ISO/IEC 27002:2022 is commonly organized into 93 controls across organizational, people, physical, and technological themes ([Splunk](https://www.splunk.com/en_us/blog/learn/iso-27002.html)). Certification audits are typically performed through a Stage 1 documentation-readiness audit followed by a Stage 2 implementation and effectiveness audit ([Johanson Group](https://www.johansonllp.com/blog/iso-27001-stage-1-vs-stage-2)).

## Assumed managed services scope

This roadmap assumes the organization provides managed IT, cloud operations, security monitoring, endpoint management, help desk, backup administration, remote infrastructure support, and customer environment administration. The assumed ISMS scope includes:

- Corporate systems used to deliver managed services, including ticketing, RMM, PSA, SIEM, EDR, IAM, documentation, monitoring, backup, and collaboration tools.
- Personnel who administer or support customer environments, including service desk, NOC, SOC, cloud operations, engineering, account management, and leadership.
- Customer data and customer environment access handled through support tickets, remote access tools, administrative credentials, monitoring platforms, backup platforms, and shared documentation repositories.
- Cloud and SaaS services used to deliver managed services.
- Supplier relationships that affect service delivery, including cloud providers, RMM/PSA vendors, EDR vendors, backup providers, contractors, data centers, and subcontracted support teams.

The assumed scope excludes customer-owned systems that the managed services company does not control, except where the company has administrative access, monitoring responsibility, backup responsibility, or contractual security obligations.

## Open questions to finalize before audit

| Area | Question | Why it matters |
|---|---|---|
| Certification boundary | Which legal entity, offices, services, teams, and systems are in scope? | Defines the ISMS scope statement, audit sample, and certificate wording. |
| Services | Which services are included: MSP, MSSP, cloud operations, backup, help desk, compliance support, vCISO, professional services? | Changes risk scenarios, control owners, evidence, and customer commitments. |
| Customer access | Do staff have privileged access to customer networks, cloud tenants, endpoints, identity providers, or backups? | Drives privileged access, segregation, monitoring, and customer environment controls. |
| Data types | What customer data is processed, stored, viewed, or transmitted? | Drives confidentiality, privacy, retention, encryption, and data deletion requirements. |
| Locations | Are operations remote, office-based, offshore, hybrid, or distributed? | Drives physical security, remote work, endpoint, and personnel controls. |
| Tooling | What are the core PSA, RMM, IAM, SIEM, EDR, backup, vulnerability, HRIS, and GRC tools? | Determines where evidence is generated and retained. |
| Contractual obligations | What security requirements appear in customer contracts, SLAs, DPAs, BAAs, MSAs, or supplier agreements? | These become interested-party and compliance requirements for the ISMS. |
| Certification timeline | Is the target certification window 6, 9, or 12 months? | Determines remediation prioritization and evidence lookback expectations. |

## Ground-up ISO 27001 build approach

### Establish ISMS governance

The first step is to create the management structure for the ISMS. ISO 27001 is not only a technical control framework. It requires leadership commitment, defined roles, documented responsibilities, risk-based planning, performance monitoring, internal audit, management review, and continual improvement.

Minimum governance artifacts:

- ISMS charter or program plan.
- ISMS scope statement.
- Information security policy approved by top management.
- Security roles and responsibility matrix.
- Risk assessment and risk treatment methodology.
- Statement of Applicability.
- Security objectives and metrics.
- Internal audit procedure.
- Management review procedure.
- Corrective action and continual improvement procedure.

Recommended governance roles:

| Role | Primary responsibilities |
|---|---|
| Executive sponsor | Approves ISMS scope, resources, objectives, risk appetite, risk acceptance, and management review decisions. |
| ISMS owner | Owns ISO 27001 implementation, evidence management, audit coordination, and continual improvement. |
| Security lead | Owns technical controls, incident response, vulnerability management, logging, access control, and monitoring. |
| Service operations lead | Owns help desk, NOC/SOC process controls, change control, ticket quality, customer access procedures, and SLA evidence. |
| HR or people operations | Owns screening, onboarding, training, acceptable use, confidentiality, disciplinary process, and offboarding. |
| IT operations | Owns internal endpoints, identity systems, backups, configuration, asset inventory, and network controls. |
| Vendor manager | Owns supplier due diligence, contract security requirements, cloud service reviews, and supplier monitoring. |
| Internal auditor | Performs independent ISMS and control audits. Should not audit their own operational work. |

### Define the ISMS scope

The scope should be clear enough that an auditor can understand what is certified and what is not. For managed services, the scope should address customer environment access explicitly.

Example scope statement:

> The ISMS covers the people, processes, systems, and facilities used by the organization to deliver managed IT, cloud operations, security monitoring, endpoint management, help desk, backup administration, and customer environment support services. The scope includes corporate information systems, service delivery platforms, administrative access processes, monitoring tools, ticketing systems, endpoint devices, and supplier services used to process or access customer information and customer environments. Customer-owned infrastructure is excluded except where the organization administers, monitors, backs up, or otherwise has contractual responsibility for security-related activities.

### Build the risk management foundation

ISO 27001 implementation should be driven by information security risk. A managed services company should define a repeatable risk methodology and then identify risks across customer administration, privileged access, remote operations, monitoring, backup, service continuity, supplier reliance, employee behavior, and contractual obligations.

Minimum risk artifacts:

- Risk assessment methodology.
- Asset inventory and asset ownership.
- Risk register.
- Risk treatment plan.
- Risk acceptance records.
- Statement of Applicability.
- Security objectives linked to risk treatment.

Recommended risk rating model:

| Rating component | Suggested scale |
|---|---|
| Likelihood | 1 rare, 2 unlikely, 3 possible, 4 likely, 5 almost certain |
| Impact | 1 negligible, 2 minor, 3 moderate, 4 major, 5 severe |
| Inherent risk | Likelihood x impact before treatment |
| Residual risk | Likelihood x impact after implemented controls |
| Treatment decision | Mitigate, transfer, avoid, or accept |

### Create a managed-services risk register

Start with risk scenarios that reflect how managed services companies fail in practice.

| Risk ID | Managed services risk scenario | Common impact | Example treatment controls |
|---|---|---|---|
| MS-R1 | Compromise of privileged technician account used across customer environments | Customer breach, service disruption, contractual breach | MFA, PAM, least privilege, named accounts, access review, session logging, emergency access process |
| MS-R2 | RMM or remote access platform compromise | Broad customer impact, ransomware propagation | Vendor risk review, MFA, IP restrictions, conditional access, logging, device trust, change control, alerting |
| MS-R3 | Incomplete offboarding of employee or contractor with customer access | Unauthorized access, customer confidentiality breach | HR-triggered offboarding, access inventory, termination checklist, access revocation evidence |
| MS-R4 | Weak segregation of duties in ticket, change, and admin processes | Unauthorized or unreviewed customer changes | Role-based access, change approval, privileged change review, ticket evidence |
| MS-R5 | Customer backup failure or restoration failure | Availability breach, SLA breach, recovery failure | Backup monitoring, restore testing, exception reporting, customer notification workflow |
| MS-R6 | Security alert missed by NOC or SOC | Delayed incident detection, customer impact | Alert triage procedure, escalation matrix, shift handoff, SIEM tuning, case QA |
| MS-R7 | Vulnerability remediation not tracked across managed assets | Exploitation, customer exposure | Vulnerability scanning, remediation SLAs, exception approvals, recurring reports |
| MS-R8 | Insecure storage of customer credentials or secrets | Unauthorized access, lateral movement | Password vault, secret rotation, access control, logging, no credentials in tickets |
| MS-R9 | Unauthorized customer data stored in tickets, notes, screenshots, or logs | Data exposure, privacy breach | Data handling standard, masking, retention, secure attachment process, DLP where applicable |
| MS-R10 | Supplier outage or compromise affecting managed services | Service interruption, security incident | Supplier due diligence, resilience review, contractual requirements, continuity planning |
| MS-R11 | Lack of evidence that controls operated consistently | Audit failure, customer assurance gaps | GRC repository, control calendar, owner attestations, evidence QA |
| MS-R12 | Customer contract security obligations not tracked | Noncompliance, disputes, lost revenue | Contract requirement register, compliance review, account-level obligation mapping |

### Build the policy and procedure framework

At minimum, create and approve the following documents:

| Document | Purpose |
|---|---|
| Information security policy | Leadership direction, ISMS objectives, commitment to applicable requirements and continual improvement. |
| Access control policy | Identity lifecycle, least privilege, MFA, privileged access, customer access, access reviews. |
| Acceptable use policy | Employee and contractor expectations for systems, devices, customer data, and communications. |
| Asset management policy | Inventory, ownership, classification, acceptable handling, return of assets. |
| Data classification and handling standard | Rules for confidential data, customer data, credentials, screenshots, logs, backups, and tickets. |
| Cryptography and key management standard | Encryption requirements for endpoints, cloud services, backups, secrets, and data transfers. |
| Vulnerability management procedure | Scanning, triage, remediation SLAs, exceptions, and reporting. |
| Change management procedure | Internal and customer-impacting changes, approval, testing, rollback, emergency changes. |
| Incident response plan | Event intake, triage, escalation, customer notification, evidence preservation, lessons learned. |
| Supplier security procedure | Due diligence, contract requirements, ongoing monitoring, cloud service review. |
| Backup and recovery procedure | Backup scope, monitoring, restoration tests, exception handling. |
| Business continuity and disaster recovery plan | Continuity risks, RTO/RPO, crisis communications, alternate work methods. |
| Secure configuration standard | Baseline hardening for laptops, servers, network devices, cloud services, and tools. |
| Logging and monitoring standard | Log sources, retention, alerting, review, escalation, and evidence. |
| Secure development or automation standard | Applies if scripts, integrations, customer automation, or internal tools are developed. |
| HR security procedure | Screening, onboarding, training, role changes, disciplinary process, and offboarding. |
| Internal audit procedure | Audit planning, independence, scope, reporting, and corrective actions. |
| Management review procedure | Leadership review agenda, inputs, outputs, decisions, and retained minutes. |

## ISO 27001 implementation roadmap

The roadmap below assumes a practical 9-month implementation. A smaller organization with strong existing controls may compress this to 4 to 6 months. A larger MSP, MSSP, or multi-location organization may need 9 to 12 months or more.

| Phase | Timing | Objective | Key activities | Primary outputs | Owners |
|---|---:|---|---|---|---|
| Phase 1: Mobilize and scope | Weeks 1-2 | Launch the ISMS program and define boundaries | Appoint sponsor and ISMS owner, identify interested parties, define services and systems in scope, create project plan | ISMS charter, scope draft, stakeholder register, project plan | Executive sponsor, ISMS owner |
| Phase 2: Baseline assessment | Weeks 2-4 | Understand current security and compliance posture | Review existing policies, tools, customer obligations, security processes, access models, ticketing practices, supplier list, and evidence maturity | Gap assessment, prioritized remediation backlog | ISMS owner, security lead, operations lead |
| Phase 3: Risk methodology and asset inventory | Weeks 4-6 | Establish risk-based foundation | Define risk criteria, identify assets, assign asset owners, classify information, document customer access pathways | Risk methodology, asset inventory, classification model | ISMS owner, IT, service operations |
| Phase 4: Risk assessment and treatment | Weeks 6-9 | Identify and treat managed-services risks | Conduct workshops, identify risks, rate inherent risk, select treatments, assign owners and target dates | Risk register, risk treatment plan, risk acceptance records | ISMS owner, risk owners |
| Phase 5: Statement of Applicability | Weeks 8-10 | Select Annex A controls based on risk | Determine applicable controls, justify inclusions and exclusions, map controls to risks, identify implementation status | Statement of Applicability, control mapping | ISMS owner, security lead |
| Phase 6: Policy and procedure build | Weeks 8-14 | Build required documented information | Draft and approve policies and procedures, align to actual operations, train owners | Approved policy suite, procedure library | ISMS owner, legal, HR, IT, operations |
| Phase 7: Technical and operational remediation | Weeks 10-22 | Implement missing controls | MFA, PAM, access reviews, logging, vulnerability management, backup testing, vendor reviews, incident response, change control, asset inventory, secure configurations | Implemented controls, tickets, configuration evidence | Security, IT, operations, vendor manager |
| Phase 8: Evidence operating period | Weeks 16-28 | Demonstrate controls are operating | Run recurring reviews, collect evidence, perform ticket QA, document exceptions, track metrics, resolve control failures | Evidence repository, control calendar, metric dashboard | Control owners |
| Phase 9: Internal audit | Weeks 24-30 | Independently test ISMS conformity | Audit clauses, SoA controls, evidence, interviews, samples, findings, corrective actions | Internal audit report, findings tracker, corrective action plans | Internal auditor, ISMS owner |
| Phase 10: Management review | Weeks 28-32 | Obtain leadership review and decisions | Review risks, objectives, audit results, incidents, nonconformities, performance metrics, resource needs, improvement opportunities | Management review deck, minutes, action items | Executive sponsor, leadership team |
| Phase 11: Stage 1 readiness | Weeks 32-34 | Prepare for documentation audit | Final document QA, SoA QA, risk treatment QA, evidence index, certification body coordination | Stage 1 evidence package, document index | ISMS owner |
| Phase 12: Stage 1 audit and remediation | Weeks 34-38 | Complete documentation review and close findings | Attend Stage 1, respond to auditor requests, close observations and nonconformities | Stage 1 report, remediation evidence | ISMS owner, control owners |
| Phase 13: Stage 2 readiness | Weeks 38-40 | Prepare for implementation audit | Refresh evidence, brief staff, perform mock interviews, validate access reviews and control samples | Stage 2 audit package, interview prep, sample evidence | ISMS owner, security lead |
| Phase 14: Stage 2 audit and corrective actions | Weeks 40-44 | Demonstrate operating effectiveness | Support auditor testing, interviews, sampling, issue response, corrective actions if needed | Stage 2 report, corrective action records | Executive sponsor, ISMS owner |
| Phase 15: Continual improvement | Ongoing | Maintain certification readiness | Quarterly control reviews, annual risk assessment, internal audit program, management review, supplier reviews, training refresh | Improvement backlog, surveillance readiness evidence | ISMS owner, control owners |

## Suggested implementation milestones

| Milestone | Target | Exit criteria |
|---|---:|---|
| ISMS launched | End of week 2 | Sponsor, owner, scope draft, and project plan approved. |
| Risk foundation complete | End of week 6 | Risk methodology, asset inventory, and classification model approved. |
| Risk assessment complete | End of week 9 | Risk register and treatment plan approved by risk owners. |
| SoA approved | End of week 10 | Applicability decisions, justifications, and control status documented. |
| Policy suite approved | End of week 14 | Core policies and procedures approved and communicated. |
| Critical controls implemented | End of week 22 | MFA, access reviews, logging, incident response, backup testing, vulnerability process, supplier review, and change control operating. |
| Evidence period started | Week 16 onward | Control calendar active and evidence retained consistently. |
| Internal audit complete | End of week 30 | Findings issued and corrective actions assigned. |
| Management review complete | End of week 32 | Leadership decisions and actions recorded. |
| Stage 1 ready | End of week 34 | Documentation package and evidence index complete. |
| Stage 2 ready | End of week 40 | Controls operating, staff briefed, samples validated. |

## Managed services control matrix

This matrix is not a full Statement of Applicability. It is a managed-services-focused control matrix that can become the foundation for a full SoA, risk treatment plan, and evidence request list.

| Control area | ISO reference | Managed services control expectation | Evidence type | Example evidence | Owner | Cadence |
|---|---|---|---|---|---|---|
| ISMS scope | Clause 4.3 | Define the ISMS boundary, services, systems, locations, customer access responsibilities, and exclusions. | Design | Approved ISMS scope statement, system inventory, service catalog | ISMS owner | Annual and upon major change |
| Interested parties | Clause 4.2 | Identify customer, regulatory, contractual, supplier, employee, and leadership requirements affecting information security. | Design and operating effectiveness | Interested party register, contract requirement register, review minutes | ISMS owner, legal | Annual and upon new contract type |
| ISMS processes | Clause 4.4 | Maintain the ISMS process map and show how governance, risk, controls, audit, review, and improvement interact. | Design | ISMS process map, governance calendar | ISMS owner | Annual |
| Leadership commitment | Clause 5.1 | Leadership approves security policy, resources, risk appetite, objectives, and management review decisions. | Operating effectiveness | Approved policies, budget approvals, management review minutes | Executive sponsor | Quarterly or annual |
| Information security policy | Clause 5.2, A.5.1 | Maintain an approved policy communicated to employees and relevant interested parties. | Design and operating effectiveness | Policy, approval record, employee acknowledgment | Executive sponsor, ISMS owner | Annual |
| Roles and responsibilities | Clause 5.3, A.5.2 | Define ISMS and control ownership across service desk, NOC, SOC, IT, HR, security, and vendor management. | Design | RACI matrix, job descriptions, control owner list | ISMS owner | Annual and upon reorganization |
| Risk assessment | Clause 6.1.2 | Perform repeatable information security risk assessment covering customer administration, tooling, remote access, suppliers, and service continuity. | Operating effectiveness | Risk methodology, risk register, workshop notes, risk approvals | ISMS owner, risk owners | Annual and upon major change |
| Risk treatment | Clause 6.1.3 | Maintain treatment plans for unacceptable risks and link selected controls to the SoA. | Operating effectiveness | Risk treatment plan, risk owner approvals, treatment tickets | ISMS owner | Monthly until closed, then quarterly |
| Statement of Applicability | Clause 6.1.3 | Document Annex A applicability, justification, implementation status, linked risks, and evidence. | Design and operating effectiveness | SoA, risk-control mapping, exclusion justifications | ISMS owner | Annual and upon major change |
| Security objectives | Clause 6.2 | Define measurable objectives such as MFA coverage, patch SLA, backup restore success, alert triage SLA, training completion, and access review completion. | Operating effectiveness | Metrics dashboard, objective tracking, management review materials | ISMS owner, leadership | Monthly or quarterly |
| Competence and awareness | Clause 7.2, 7.3, A.6.3 | Train staff on customer data handling, phishing, credential security, incident reporting, remote support, and acceptable use. | Operating effectiveness | Training records, completion reports, awareness materials | HR, security | On hire and annual |
| Documented information | Clause 7.5 | Control policies, procedures, risk records, SoA, evidence, approvals, and retention in a managed repository. | Design and implementation | Document control register, version history, evidence repository | ISMS owner | Continuous |
| Operational planning | Clause 8.1 | Plan and control recurring ISMS processes, including risk reviews, access reviews, vulnerability remediation, supplier reviews, and evidence collection. | Operating effectiveness | ISMS calendar, control attestations, completed review records | ISMS owner | Monthly or quarterly |
| Monitoring and measurement | Clause 9.1 | Track ISMS metrics and control performance relevant to managed services. | Operating effectiveness | KPI dashboard, SLA reports, control exception reports | ISMS owner, operations | Monthly |
| Internal audit | Clause 9.2 | Perform independent internal audit covering clauses, SoA controls, evidence, and managed services processes. | Operating effectiveness | Audit plan, audit report, samples tested, findings | Internal auditor | Annual before certification or surveillance |
| Management review | Clause 9.3 | Leadership reviews ISMS performance, risks, incidents, audit results, objectives, resources, and improvement opportunities. | Operating effectiveness | Management review agenda, deck, minutes, actions | Executive sponsor | Quarterly preferred, at least annual |
| Nonconformity and corrective action | Clause 10.1 | Track audit findings, control failures, incidents, and corrective actions through closure and effectiveness review. | Operating effectiveness | CAPA tracker, root cause analysis, closure evidence | ISMS owner | As needed, reviewed monthly |
| Continual improvement | Clause 10.2 | Maintain improvement backlog based on incidents, audits, metrics, customer feedback, and risk changes. | Operating effectiveness | Improvement register, leadership decisions, completed actions | ISMS owner | Quarterly |
| Threat intelligence | A.5.7 | Collect and review threat intelligence relevant to RMM tools, MSP-targeted attacks, cloud services, vulnerabilities, and customer environments. | Operating effectiveness | Threat bulletins, review notes, tickets created from intelligence | Security lead | Weekly or monthly |
| Segregation of duties | A.5.3 | Separate approval and execution for high-risk activities such as privileged access grants, production/customer changes, backup deletion, and security rule changes. | Design and operating effectiveness | Role matrix, workflow approvals, exception approvals | Operations lead, security | Quarterly review |
| Contact with authorities and special interest groups | A.5.5, A.5.6 | Maintain escalation contacts for law enforcement, regulators, cyber insurance, CERTs, vendors, and industry groups where relevant. | Design | Contact register, incident escalation procedure | Security lead | Annual |
| Project management security | A.5.8 | Include security requirements in onboarding new customers, deploying RMM agents, integrating monitoring, and delivering professional services projects. | Operating effectiveness | Project checklists, security signoffs, onboarding records | Service delivery lead | Per project |
| Asset inventory | A.5.9 | Maintain inventory of corporate assets, service delivery tools, privileged platforms, customer access mechanisms, and assigned owners. | Implementation and operating effectiveness | CMDB, SaaS inventory, endpoint inventory, customer access inventory | IT, operations | Monthly or quarterly |
| Acceptable use | A.5.10 | Define acceptable use of company systems, customer systems, remote access tools, removable media, AI tools, and collaboration tools. | Design and operating effectiveness | Policy, acknowledgments, exception records | HR, IT | On hire and annual |
| Return of assets | A.5.11 | Recover laptops, tokens, badges, keys, customer devices, and removable media during offboarding. | Operating effectiveness | Termination checklist, asset return records | HR, IT | Per termination |
| Information classification | A.5.12 | Classify customer data, credentials, tickets, screenshots, logs, configurations, contracts, and internal security records. | Design and implementation | Classification standard, labels, repository rules | ISMS owner, data owners | Annual |
| Information handling | A.5.13 | Define handling rules for customer confidential data, passwords, evidence exports, logs, ticket attachments, and screenshots. | Design and operating effectiveness | Handling standard, ticket QA results, secure transfer records | Security, operations | Quarterly QA |
| Access control rules | A.5.15 | Establish rules for access to internal systems, customer tools, customer environments, and privileged service platforms. | Design and operating effectiveness | Access control policy, role matrix, access approval tickets | IT, security | Quarterly |
| Identity management | A.5.16 | Use named accounts wherever possible and maintain full joiner, mover, and leaver lifecycle for employees, contractors, and service accounts. | Operating effectiveness | IAM exports, HR triggers, access request tickets, termination samples | IT, HR | Per event, quarterly review |
| Authentication information | A.5.17 | Protect passwords, API keys, recovery codes, certificates, and customer credentials using vaulting and rotation rules. | Implementation and operating effectiveness | Password vault records, rotation tickets, MFA configuration | Security, IT | Quarterly |
| Access rights | A.5.18 | Review access to PSA, RMM, SIEM, EDR, cloud consoles, backup tools, password vaults, customer portals, and admin groups. | Operating effectiveness | Access review exports, reviewer approvals, remediation tickets | System owners | Quarterly |
| Supplier relationships | A.5.19, A.5.20, A.5.21 | Perform supplier due diligence and include security requirements in contracts for critical vendors and subcontractors. | Design and operating effectiveness | Supplier register, due diligence reviews, contracts, SOC/ISO reports | Vendor manager | Annual and before onboarding |
| Cloud services security | A.5.23 | Review cloud and SaaS services for shared responsibility, logging, encryption, access, backup, retention, and customer data handling. | Design and operating effectiveness | Cloud service assessments, configuration reviews, vendor documents | Security, IT | Annual and before onboarding |
| Incident management planning | A.5.24, A.5.25 | Define how employees detect, report, triage, escalate, investigate, and communicate security events and incidents. | Design and operating effectiveness | Incident response plan, incident tickets, escalation matrix | Security lead | Annual exercise, per incident |
| Incident response and lessons learned | A.5.26, A.5.27 | Conduct post-incident reviews and track corrective actions for internal and customer-impacting incidents. | Operating effectiveness | PIR reports, lessons learned, corrective action tickets | Security lead | Per incident |
| Evidence collection | A.5.28 | Preserve logs, ticket histories, forensic artifacts, screenshots, and communications during incident investigations. | Design and operating effectiveness | Evidence handling procedure, chain of custody records | Security lead | Per incident |
| Business continuity | A.5.29, A.5.30 | Maintain continuity plans for service desk, monitoring, remote access, backup operations, and critical SaaS/platform outages. | Design and operating effectiveness | BCP, tabletop records, DR tests, continuity contact list | Operations, IT | Annual and after major change |
| Legal and contractual requirements | A.5.31, A.5.32, A.5.33, A.5.34 | Track security, privacy, intellectual property, records retention, and customer contractual obligations. | Design and operating effectiveness | Legal register, contract requirement matrix, retention schedule | Legal, ISMS owner | Annual |
| Independent review | A.5.35 | Conduct independent reviews of the ISMS through internal audit, external readiness assessment, or qualified independent reviewer. | Operating effectiveness | Review report, findings, corrective actions | Internal auditor | Annual |
| Compliance with policies and standards | A.5.36 | Monitor adherence to policies through evidence reviews, ticket QA, access review QA, and exception tracking. | Operating effectiveness | Compliance review records, exceptions, remediation tickets | ISMS owner | Quarterly |
| Documented operating procedures | A.5.37 | Maintain procedures for service desk, customer onboarding, remote support, monitoring, backup, change, incident, and access management. | Design | Procedure library, version history, approvals | Operations lead | Annual |
| Screening | A.6.1 | Screen employees and contractors according to role sensitivity and law before granting access to customer environments. | Operating effectiveness | Background check records or attestations, screening policy | HR | Before hire or engagement |
| Terms and conditions of employment | A.6.2 | Include confidentiality, acceptable use, security obligations, and customer data obligations in employment or contractor agreements. | Design and operating effectiveness | Signed agreements, handbook acknowledgments | HR, legal | On hire and update |
| Disciplinary process | A.6.4 | Define consequences for policy violations involving customer access, credentials, data handling, and security misconduct. | Design | Disciplinary policy, HR procedure | HR | Annual |
| Responsibilities after termination | A.6.5 | Ensure confidentiality and security obligations continue after termination where applicable. | Design and operating effectiveness | Agreements, exit checklist, reminder notices | HR, legal | Per termination |
| Confidentiality agreements | A.6.6 | Require NDAs or confidentiality agreements for employees, contractors, and suppliers with sensitive access. | Operating effectiveness | Signed NDA records | HR, legal | On hire or onboarding |
| Remote working | A.6.7 | Protect remote service delivery using managed devices, MFA, VPN or conditional access, endpoint security, secure Wi-Fi expectations, and workspace privacy. | Implementation and operating effectiveness | Remote work policy, device compliance reports, conditional access settings | IT, security | Quarterly |
| Security event reporting | A.6.8 | Train staff to report suspicious emails, customer alerts, credential exposure, lost devices, policy violations, and abnormal tool behavior. | Operating effectiveness | Awareness records, reported events, phishing simulation results | Security | Continuous, reviewed monthly |
| Physical security perimeters | A.7.1 | Protect offices, data rooms, and areas where customer data or service delivery systems are accessed. | Implementation | Badge logs, visitor records, office access list | Facilities, IT | Quarterly |
| Physical entry | A.7.2 | Restrict and review physical access to offices, network closets, and storage areas. | Operating effectiveness | Access reviews, visitor logs, key inventory | Facilities | Quarterly |
| Securing offices and facilities | A.7.3 | Apply clear desk, screen lock, visitor escort, and secure storage for customer information and devices. | Implementation and operating effectiveness | Office security checklist, walkthrough records | Facilities, ISMS owner | Quarterly |
| Equipment security | A.7.8, A.7.9, A.7.10, A.7.14 | Protect laptops, mobile devices, network equipment, removable media, cabling, and disposal activities. | Implementation and operating effectiveness | MDM reports, encryption status, disposal certificates, asset records | IT | Monthly or quarterly |
| Endpoint devices | A.8.1 | Manage corporate laptops and mobile devices used for customer support with encryption, EDR, patching, screen lock, and configuration baselines. | Implementation and operating effectiveness | MDM exports, EDR coverage, encryption reports | IT, security | Monthly |
| Privileged access rights | A.8.2 | Restrict privileged access to internal and customer systems based on role, approval, MFA, logging, and time-bound need where feasible. | Operating effectiveness | PAM logs, admin group review, approval tickets, session logs | Security, IT | Monthly or quarterly |
| Information access restriction | A.8.3 | Limit access to customer documentation, tickets, credentials, backups, logs, and monitoring data based on need to know. | Operating effectiveness | RBAC configuration, repository permissions, access reviews | System owners | Quarterly |
| Source code or automation access | A.8.4, A.8.25, A.8.28 | Protect scripts, integrations, infrastructure-as-code, and customer automation with code review, repository access control, and secure coding practices. | Operating effectiveness | Repo permissions, pull requests, code review records, secret scans | Engineering, security | Per change, quarterly review |
| Secure authentication | A.8.5 | Enforce MFA, strong authentication, conditional access, and secure session controls for internal and customer-supporting platforms. | Implementation and operating effectiveness | MFA reports, SSO policies, exception approvals | IT, security | Monthly |
| Capacity management | A.8.6 | Monitor capacity for service platforms such as ticketing, monitoring, SIEM, backup repositories, VPN, and remote access tools. | Operating effectiveness | Capacity reports, alerts, scaling actions | IT, operations | Monthly |
| Malware protection | A.8.7 | Deploy and monitor EDR or anti-malware on managed corporate endpoints and servers. | Operating effectiveness | EDR coverage, alert tickets, remediation records | Security | Daily monitoring, monthly reporting |
| Vulnerability management | A.8.8 | Identify, prioritize, remediate, and track vulnerabilities for corporate assets and managed services platforms. | Operating effectiveness | Scan results, patch tickets, exception approvals, SLA reports | Security, IT | Weekly or monthly |
| Configuration management | A.8.9 | Define and monitor secure configurations for endpoints, cloud services, RMM, PSA, SIEM, EDR, backup, and network devices. | Design and operating effectiveness | Baseline standards, configuration exports, drift reports | IT, security | Quarterly |
| Information deletion | A.8.10 | Securely delete customer data, tickets, attachments, backups, logs, credentials, and offboarded customer records according to retention rules. | Operating effectiveness | Deletion logs, retention settings, customer offboarding checklist | IT, operations | Per event, annual review |
| Data masking | A.8.11 | Mask or avoid unnecessary customer secrets, personal data, and sensitive screenshots in tickets, reports, training, and logs. | Implementation and operating effectiveness | Ticket QA results, masking configuration, handling guidance | Operations, security | Quarterly |
| Data leakage prevention | A.8.12 | Prevent unauthorized transfer of customer data through email, file sharing, removable media, unmanaged devices, and public AI tools. | Implementation and operating effectiveness | DLP alerts, sharing restrictions, exception logs | Security, IT | Monthly |
| Backup | A.8.13 | Back up critical corporate and service delivery systems and, where contracted, customer systems; monitor jobs and test restores. | Operating effectiveness | Backup job reports, failure tickets, restore test results | IT, backup team | Daily monitoring, quarterly restore tests |
| Redundancy | A.8.14 | Design critical managed-services tooling and connectivity for appropriate availability and failover. | Design and implementation | Architecture diagrams, failover tests, vendor SLA records | IT, operations | Annual |
| Logging | A.8.15 | Enable logs for IAM, privileged access, RMM, PSA, SIEM, EDR, cloud consoles, backup, and security platforms. | Implementation and operating effectiveness | Log source inventory, retention settings, ingestion reports | Security | Monthly |
| Monitoring activities | A.8.16 | Monitor security events, admin activity, failed logins, privilege changes, RMM activity, EDR alerts, and suspicious customer support activity. | Operating effectiveness | SIEM alerts, monitoring dashboards, triage tickets | SOC/NOC, security | Daily |
| Clock synchronization | A.8.17 | Synchronize system clocks for accurate incident investigation and log correlation. | Implementation | NTP settings, configuration records | IT | Annual or configuration change |
| Privileged utility programs | A.8.18 | Restrict tools capable of bypassing controls, including remote shells, admin consoles, credential tools, forensic tools, and backup deletion utilities. | Operating effectiveness | Admin tool access list, approvals, monitoring logs | Security, IT | Quarterly |
| Software installation | A.8.19 | Control software installation on company endpoints and service delivery systems. | Implementation and operating effectiveness | MDM policy, application allowlist, installation tickets | IT | Monthly |
| Network security | A.8.20, A.8.21, A.8.22 | Segment internal networks, restrict administrative access, protect VPN, and separate customer environments where applicable. | Design and implementation | Network diagrams, firewall rules, VPN configuration, review records | IT, security | Quarterly |
| Web filtering | A.8.23 | Apply web filtering or equivalent controls to reduce malware, phishing, and unsafe access from managed endpoints. | Implementation and operating effectiveness | Filtering policy, block reports, exceptions | IT, security | Monthly |
| Cryptography | A.8.24 | Encrypt endpoints, backups, data transfers, secrets, and sensitive repositories using approved methods. | Implementation | Encryption reports, key management records, TLS settings | IT, security | Quarterly |
| Secure development lifecycle | A.8.25 to A.8.31 | If the organization develops scripts, portals, automations, integrations, or internal tools, implement secure development, testing, change control, code review, and environment separation. | Design and operating effectiveness | SDLC procedure, PR approvals, test records, change tickets | Engineering, security | Per release |
| Change management | A.8.32 | Control changes to internal systems, service platforms, customer environments, monitoring rules, backup jobs, and privileged configurations. | Operating effectiveness | Change tickets, approvals, test evidence, rollback plans | Operations, IT | Per change |
| Test information | A.8.33 | Avoid using live customer data in testing unless approved, minimized, protected, and contractually allowed. | Design and operating effectiveness | Test data procedure, masking records, approvals | Engineering, operations | Per project |
| Audit test protection | A.8.34 | Control audit, penetration test, vulnerability scan, and customer environment testing to prevent disruption and unauthorized access. | Operating effectiveness | Test approvals, scope documents, customer authorizations | Security, operations | Per test |

## Evidence repository structure

Use a central evidence repository with restricted access and clear naming conventions. Recommended folders:

```text
01_ISMS_Governance
02_Scope_and_Interested_Parties
03_Risk_Assessment_and_Treatment
04_Statement_of_Applicability
05_Policies_and_Procedures
06_Access_Control
07_HR_and_Training
08_Asset_and_Configuration_Management
09_Vulnerability_and_Patching
10_Logging_Monitoring_and_Incident_Response
11_Backup_BCP_and_DR
12_Change_Management
13_Supplier_and_Cloud_Security
14_Internal_Audit
15_Management_Review
16_Corrective_Actions
17_Customer_Specific_Obligations
```

## Recurring operating cadence

| Cadence | Activities |
|---|---|
| Daily | Monitor security alerts, backup failures, EDR issues, RMM alerts, and critical service platform health. |
| Weekly | Review high-risk vulnerabilities, open security incidents, overdue access requests, backup failures, and customer-impacting exceptions. |
| Monthly | Review ISMS metrics, control evidence, vulnerability SLA performance, EDR coverage, backup reports, monitoring triage quality, and critical vendor alerts. |
| Quarterly | Perform access reviews, supplier monitoring, ticket QA, change QA, configuration review, risk treatment review, and management review. |
| Semiannual | Conduct incident response tabletop, restore tests for critical systems, business continuity exercise, and policy effectiveness review if needed. |
| Annual | Refresh risk assessment, SoA, policy approvals, security training, internal audit, management review, supplier due diligence, and certification surveillance readiness. |

## Minimum audit-ready evidence list

| Evidence area | Minimum evidence to retain |
|---|---|
| Governance | ISMS scope, policy, objectives, role matrix, governance calendar, management review minutes. |
| Risk | Risk methodology, risk register, risk treatment plan, risk owner approvals, risk acceptance records. |
| SoA | Annex A applicability decisions, justifications, implementation status, linked risks, evidence references. |
| Access control | Access requests, approvals, MFA reports, privileged access reviews, termination access revocation samples. |
| Customer access | Customer admin access inventory, remote support logs, credential vault access records, customer offboarding checklist. |
| HR security | Screening evidence, signed agreements, training completion, offboarding checklist, disciplinary procedure. |
| Asset management | Endpoint inventory, SaaS inventory, service platform inventory, owner assignments, classification records. |
| Vulnerability management | Scan reports, remediation tickets, patch SLA reports, exception approvals. |
| Logging and monitoring | Log source inventory, SIEM/EDR alert tickets, monitoring review records, escalation records. |
| Incident response | Incident tickets, severity classification, communications, post-incident reviews, corrective actions. |
| Backup and recovery | Backup job reports, failure remediation, restore test evidence, backup configuration. |
| Change management | Change tickets, approvals, testing, rollback plans, emergency change reviews. |
| Supplier security | Supplier register, risk ratings, due diligence, contracts, security reports, review records. |
| Cloud security | Cloud service assessments, access configuration, encryption, logging, shared responsibility review. |
| Business continuity | BCP, DR plan, tabletop records, contact list, recovery test evidence. |
| Internal audit | Audit plan, checklist, samples, findings, report, corrective action plan. |
| Corrective action | Root cause analysis, remediation evidence, effectiveness review. |

## Stage 1 readiness checklist

Before Stage 1, confirm:

- ISMS scope is approved and matches services, systems, locations, and customer access responsibilities.
- Interested parties and requirements are documented.
- Risk assessment methodology is approved.
- Risk register and treatment plan are complete.
- Statement of Applicability is complete and approved.
- Core policies and procedures are approved and controlled.
- Security objectives and metrics are defined.
- Internal audit has been performed or scheduled according to certification body expectations.
- Management review has been completed or scheduled according to certification body expectations.
- Evidence index maps clauses and controls to records.
- Major policy gaps and obvious control design gaps are remediated.

## Stage 2 readiness checklist

Before Stage 2, confirm:

- Controls have operated long enough to produce evidence.
- Access reviews have been completed and exceptions remediated.
- Vulnerability remediation evidence supports defined SLAs.
- Backup restoration tests have been completed.
- Incident response records or tabletop evidence exist.
- Supplier reviews are complete for critical vendors.
- Change management samples show approval, testing, and closure.
- Staff can explain their security responsibilities.
- Internal audit findings are tracked and corrective actions are progressing.
- Management review minutes include decisions, actions, and resource needs.
- Evidence is organized and owners are ready for auditor interviews.

## First 30 days action plan

| Week | Priority actions | Deliverables |
|---|---|---|
| Week 1 | Appoint sponsor and ISMS owner, define implementation team, gather existing policies and systems list. | ISMS charter, implementation team roster, document inventory. |
| Week 2 | Draft ISMS scope, identify interested parties, identify critical managed-services tools and customer access paths. | Scope draft, interested party register, service delivery tool inventory. |
| Week 3 | Define risk methodology, start asset inventory, identify top 10 managed-services risks. | Risk methodology, asset inventory draft, initial risk scenarios. |
| Week 4 | Run risk workshop, create remediation backlog, start policy suite build. | Risk register draft, remediation tracker, policy drafting plan. |

## Practical control priorities for a managed services company

If time or resources are constrained, prioritize these controls first:

1. Privileged access management for internal and customer environments.
2. MFA and conditional access for all service delivery platforms.
3. Customer credential vaulting and secret management.
4. Employee and contractor offboarding.
5. RMM, PSA, SIEM, EDR, backup, and cloud console access reviews.
6. Logging and monitoring of privileged and remote support activity.
7. Vulnerability and patch management for corporate and service platforms.
8. Backup monitoring and restore testing.
9. Incident response and customer notification workflow.
10. Supplier and cloud service risk reviews.
11. Change control for customer-impacting work.
12. Evidence management and control owner accountability.

## Final recommendation

Treat ISO 27001 as an operating system for security governance, not as a one-time documentation project. For managed services, auditors and customers will focus heavily on whether the organization can prove consistent control over privileged access, remote administration, customer data handling, monitoring, incident escalation, backup resilience, supplier reliance, and evidence quality. Build the ISMS around those risks, keep the SoA tied to the risk treatment plan, and make control evidence part of normal service operations.
