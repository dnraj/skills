# FedRAMP Implementation Roadmap and Control Matrix for a Managed Services Company

Prepared for: Hema Raj  
Prepared date: May 16, 2026  
Purpose: Ground-up FedRAMP readiness and implementation plan for a managed services provider, MSP, MSSP, cloud operations provider, or managed IT/security services company.

## Important disclaimer

This document is a practical FedRAMP readiness and implementation guide, not a FedRAMP authorization decision, legal opinion, 3PAO assessment opinion, or guarantee of authorization. Final control applicability, parameter values, package treatment, and authorization strategy should be validated with the sponsoring agency Authorizing Official, FedRAMP advisor, 3PAO, counsel, or qualified compliance advisor.

## Working assumptions

- **Target baseline**: FedRAMP Moderate is assumed because it is the common starting point for many federal SaaS and managed-service offerings; confirm Low, Moderate, High, or LI-SaaS before finalizing the control set.
- **Authorization path**: Agency authorization is assumed. FedRAMP describes the agency authorization path as preparation, authorization, and continuous monitoring phases, with optional FedRAMP Ready work, security assessment, agency authorization review, and post-authorization ConMon activities ([FedRAMP Agency Authorization Path](https://fedramp.gov/docs/rev5/playbook/csp/authorization/agency-authorization-path/)).
- **Service model**: The organization provides managed services such as help desk, cloud administration, monitoring, vulnerability management, endpoint management, backup/recovery, incident response support, and customer environment administration.
- **Boundary model**: The FedRAMP boundary should include the systems, people, processes, cloud resources, tools, repositories, logging platforms, remote access paths, ticketing systems, CI/CD systems, backup systems, and administrative interfaces used to deliver the federal managed service.
- **Inherited controls**: The organization may inherit some physical, environmental, infrastructure, network, and platform controls from an underlying FedRAMP-authorized cloud provider, but inherited coverage must be explicitly documented and tied to the provider capability.
- **Shared responsibility**: Managed services often create shared control responsibilities with customers because the provider may operate customer environments while the customer retains mission, data, account ownership, or agency-specific approval responsibilities.

## Executive implementation strategy

The organization should build FedRAMP as an operational security program, not as a one-time documentation project. FedRAMP relies on NIST SP 800-53 controls, authorization package evidence, independent assessment, POA&M management, and ongoing continuous monitoring activities. NIST describes the Risk Management Framework as a seven-step process: Prepare, Categorize, Select, Implement, Assess, Authorize, and Monitor ([NIST Risk Management Framework](https://csrc.nist.gov/projects/risk-management)). FedRAMP also requires post-authorization continuous monitoring, and FedRAMP states that CSPs provide monthly ConMon deliverables such as updated POA&Ms, vulnerability scan files and reports, deviation requests, significant change requests, incident reporting, and annual assessment packages ([FedRAMP Agency Authorization Path](https://fedramp.gov/docs/rev5/playbook/csp/authorization/agency-authorization-path/)).

For a managed services company, the hardest FedRAMP work is usually not selecting controls. The hard work is defining the authorization boundary, proving repeatable operations across customer environments, clarifying which controls are provider-owned versus customer-owned, producing complete evidence populations, and operating vulnerability, change, access, incident, logging, backup, and supplier controls consistently.

## Target operating model

### Governance structure

| Role | Primary FedRAMP responsibilities | Suggested owner |
|---|---|---|
| Executive sponsor | Budget, prioritization, agency relationship, risk acceptance escalation | CEO, COO, CTO, CISO |
| FedRAMP program manager | Roadmap, workstream coordination, package readiness, POA&M governance | Compliance/GRC lead |
| System owner | Authorization boundary, service description, operational accountability | Product/service executive |
| Security officer | Control implementation, monitoring, incident response, vulnerability governance | CISO/security lead |
| Engineering/cloud operations lead | Infrastructure, secure configuration, deployment, network, backup, logging | Cloud operations |
| Managed services operations lead | Help desk, customer administration, endpoint operations, service tickets | Managed services director |
| IAM owner | Identity lifecycle, MFA, privileged access, access reviews | IT/security |
| Vendor/supply chain owner | Vendor inventory, external services, subcontractor security reviews | Procurement/GRC |
| 3PAO liaison | Assessment coordination, evidence quality, assessor requests | Compliance/GRC |
| Agency liaison | Agency AO coordination, customer responsibility review, ConMon communication | Executive sponsor/program manager |

### Core implementation principles

- **Boundary-first**: Do not begin SSP drafting until the authorization boundary, data flows, system inventory, external services, customer responsibilities, and administrative access paths are defined.
- **Evidence-first operations**: Every recurring managed-services process should create durable evidence, including tickets, approvals, exports, logs, reports, review sign-offs, exceptions, and closure records.
- **One system of record per control process**: Access requests, change approvals, vulnerability remediation, incidents, vendor reviews, backups, and exceptions should each have a defined system of record.
- **Shared responsibility clarity**: Every control should be classified as CSP-owned, inherited, shared, or customer-responsible.
- **ConMon from day one**: Build monthly POA&M, inventory, scan, incident, significant change, and deviation workflows before 3PAO fieldwork. FedRAMP states that continuous monitoring is intended to provide operational visibility, managed change control, and attention to incident response duties ([FedRAMP Continuous Monitoring Overview](https://fedramp.gov/docs/rev5/playbook/csp/continuous-monitoring/overview/)).

## FedRAMP implementation roadmap

### Phase 1: Executive mobilization and authorization strategy

| Item | Detail |
|---|---|
| Objective | Establish sponsorship, funding, business case, target baseline, authorization path, and FedRAMP program governance. |
| Key actions | Select target baseline; define service offering; identify federal customers or agency sponsor; appoint executive sponsor; establish GRC, security, engineering, operations, legal, and sales workstreams; approve budget for tools, staffing, 3PAO, remediation, and documentation. |
| Managed services focus | Decide whether the managed service itself is the Cloud Service Offering or whether the service supports customer-owned environments. This drives the authorization boundary, customer responsibility matrix, and evidence scope. |
| Deliverables | FedRAMP charter, target baseline decision, authorization path decision, initial service description, program RACI, budget, milestone plan. |
| Exit criteria | Leadership accepts scope, timeline, cost, accountability, and authorization approach. |

### Phase 2: Boundary, architecture, and data-flow definition

| Item | Detail |
|---|---|
| Objective | Define what is inside the FedRAMP boundary and how federal data, access, operations, logging, and customer administration flow through the service. |
| Key actions | Identify all in-scope platforms, cloud accounts, regions, tools, endpoints, repositories, ticketing systems, remote access tools, monitoring systems, backup systems, SIEM, identity providers, admin consoles, customer connections, and third-party services. |
| Managed services focus | Include jump hosts, privileged access tools, RMM/endpoint tools, customer tenant access, scripts, service accounts, SOC tools, help desk tooling, backup systems, and cloud administration consoles if used to deliver the federal managed service. |
| Deliverables | Boundary diagram, data-flow diagrams, network diagram, inventory, interconnection list, external service list, customer responsibility matrix draft, inherited control map. |
| Exit criteria | Boundary, inventory, data flows, and customer/inherited responsibilities reconcile with each other. |

### Phase 3: Current-state gap assessment

| Item | Detail |
|---|---|
| Objective | Compare current security operations and evidence against the selected FedRAMP baseline and managed services operating model. |
| Key actions | Review policies, procedures, technical configurations, tickets, access records, vulnerability reports, change records, incidents, vendor reviews, backup evidence, training records, and logging coverage. |
| Managed services focus | Test whether controls operate consistently across customer environments, support engineers, cloud administrators, SOC analysts, service accounts, subcontractors, and customer-specific exceptions. |
| Deliverables | Gap assessment, control applicability matrix, evidence quality review, remediation backlog, risk register, initial POA&M candidates. |
| Exit criteria | Gaps are prioritized by authorization risk, operational risk, remediation effort, and evidence readiness. |

### Phase 4: Control design and remediation

| Item | Detail |
|---|---|
| Objective | Build or mature the controls that must operate before assessment. |
| Key actions | Implement MFA and privileged access management; formalize access reviews; centralize logging; harden baseline configurations; enforce change control; establish vulnerability SLAs; configure authenticated scanning; document incident response; test backups/restores; formalize vendor reviews; establish supply chain risk management. |
| Managed services focus | Standardize administrative access to customer environments, approval flows for customer changes, customer incident escalation, endpoint and backup tooling, and privileged sessions. |
| Deliverables | Implemented controls, procedures, standards, runbooks, ticket workflows, monitoring rules, baseline configurations, remediation evidence. |
| Exit criteria | Controls are operating and producing evidence for a representative period before assessment. |

### Phase 5: Authorization package buildout

| Item | Detail |
|---|---|
| Objective | Create the documentation and evidence package needed for readiness review, agency review, and 3PAO assessment. |
| Key actions | Draft the SSP, control implementation statements, policies, procedures, diagrams, inventory, CRM, POA&M, incident response plan, contingency plan, configuration management plan, security assessment support materials, and evidence index. |
| Managed services focus | Make control statements specific to managed operations: who approves, who performs, what tools are used, how customer authorization is handled, how federal environments are separated, and where evidence is retained. |
| Deliverables | SSP, attachments, policies, procedures, diagrams, inventory, customer responsibility matrix, evidence repository, POA&M, control matrix. |
| Exit criteria | Every applicable control has an owner, implementation statement, responsibility model, frequency, system, and evidence artifact. |

### Phase 6: 3PAO readiness and assessment preparation

| Item | Detail |
|---|---|
| Objective | Prepare for independent assessment by ensuring evidence quality, sample populations, technical scope, and package narratives are assessment-ready. |
| Key actions | Conduct mock interviews, evidence walkthroughs, scan validation, inventory reconciliation, control owner training, POA&M review, and SAR finding response planning. |
| Managed services focus | Prepare support, SOC, cloud operations, and customer administration teams for interviews and sampling across tickets, changes, incidents, access, vulnerabilities, and customer environments. |
| Deliverables | Readiness review results, updated POA&M, evidence tracker, interview schedule, sample populations, scan scope, assessment support plan. |
| Exit criteria | The organization can demonstrate control design and operating effectiveness with complete, dated, attributable, exportable evidence. |

### Phase 7: Agency authorization support

| Item | Detail |
|---|---|
| Objective | Support the agency review and authorization process after assessment. |
| Key actions | Respond to agency and FedRAMP review comments; support SAR debrief; update package documents; remediate findings; manage risk acceptance, deviation requests, significant change questions, and POA&M commitments. |
| Managed services focus | Ensure agency-facing materials clearly explain customer responsibilities, inherited cloud responsibilities, operational SLAs, incident notification paths, and managed-service access to customer environments. |
| Deliverables | Updated SSP, SAR response materials, POA&M updates, deviation requests, significant change documentation, agency response package. |
| Exit criteria | Agency has the information needed to make a risk-based authorization decision. |

### Phase 8: Continuous monitoring and annual assessment

| Item | Detail |
|---|---|
| Objective | Maintain the authorized posture through repeatable ConMon, remediation, and annual assessment processes. |
| Key actions | Operate monthly POA&M updates, vulnerability scans, inventory updates, incident reporting, significant change review, deviation management, configuration monitoring, access reviews, risk reviews, and annual assessment support. |
| Managed services focus | Monitor whether customer onboarding, offboarding, tooling changes, subcontractors, customer-specific exceptions, and environment changes affect the authorization boundary or shared responsibilities. |
| Deliverables | Monthly ConMon package, updated inventory, updated POA&M, vulnerability scan files and reports, incident records, deviation requests, significant change requests, annual assessment package. |
| Exit criteria | The organization can continuously demonstrate security posture, change control, vulnerability management, incident response, and agency-facing transparency. |

## Suggested 18-month implementation timeline

| Timeline | Milestone | Primary outcomes |
|---|---|---|
| Months 0-1 | Mobilize | Executive sponsor, program manager, target baseline, agency strategy, initial budget, RACI. |
| Months 1-2 | Scope and boundary | Boundary diagram, data flows, inventory, external services, inherited controls, customer responsibilities. |
| Months 2-4 | Gap assessment | Baseline applicability, evidence review, remediation backlog, risk register, initial POA&M. |
| Months 4-8 | Remediation sprint 1 | IAM, MFA, privileged access, logging, vulnerability scanning, change management, inventory, policies. |
| Months 7-10 | Remediation sprint 2 | Incident response, contingency planning, backup/restore testing, supplier reviews, secure configuration, evidence automation. |
| Months 8-12 | Package buildout | SSP, control narratives, diagrams, policies, procedures, evidence index, CRM, POA&M. |
| Months 11-13 | Readiness review | Mock assessment, evidence quality review, scan validation, control owner interviews, POA&M cleanup. |
| Months 13-16 | 3PAO assessment | SAP support, fieldwork, interviews, testing, SAR findings, remediation plan. |
| Months 15-18 | Agency review and authorization support | SAR debrief, package updates, POA&M commitments, agency responses, FedRAMP review support. |
| Ongoing | Continuous monitoring | Monthly ConMon, annual assessment, significant change management, recurring evidence collection. |

## Managed services control matrix

The matrix below is designed as an implementation starter. Exact control IDs and enhancements should be finalized against the selected FedRAMP baseline workbook and agency expectations. NIST SP 800-53 Rev. 5 provides the security and privacy control catalog used for control selection, implementation, and assessment across families such as Access Control, Audit and Accountability, Configuration Management, Incident Response, Risk Assessment, System and Communications Protection, System and Information Integrity, and Supply Chain Risk Management ([NIST SP 800-53 Rev. 5](https://csrc.nist.gov/pubs/sp/800/53/r5/upd1/final)).

| Control area | Likely control families | Control objective | Managed services implementation approach | Responsibility | Owner | Frequency | Evidence | Systems/tools | Design and assessment notes |
|---|---|---|---|---|---|---|---|---|---|
| System security planning | PL, PM | Define the system, boundary, roles, responsibilities, and security plan. | Maintain SSP, service description, boundary diagrams, data-flow diagrams, inventory, shared responsibility model, and rules of behavior for managed-services personnel. | CSP-owned, with inherited and shared sections | FedRAMP program manager/system owner | At least annually and upon significant change | SSP, diagrams, inventory, CRM, rules of behavior, approval records | GRC tool, diagram repository, CMDB | SSP must describe actual operations, not policy intent. |
| Risk management | RA, CA, PM | Identify, assess, track, and remediate risks. | Maintain risk register, readiness assessment results, POA&M, risk acceptance workflow, exception handling, and executive risk review cadence. | CSP-owned; agency/customer approval for some residual risks | Security/GRC | Monthly and upon new risk | Risk register, POA&M, risk acceptances, review minutes | GRC tool, ticketing system | FedRAMP ConMon requires POA&M maintenance for risks and weaknesses identified through assessments and monitoring ([FedRAMP Continuous Monitoring Overview](https://fedramp.gov/docs/rev5/playbook/csp/continuous-monitoring/overview/)). |
| Asset inventory | CM | Maintain complete inventory of in-scope components. | Track cloud resources, tools, endpoints, service accounts, customer administration tools, jump hosts, repositories, network components, containers, databases, and external services. | CSP-owned; inherited provider for underlying infrastructure inventory | Cloud operations/security | Monthly and upon change | Inventory export, reconciliation report, change records | CMDB, CSP inventory, EDR, scanner | FedRAMP identifies CM-8 inventory updates at least monthly or when changes occur ([FedRAMP Continuous Monitoring Overview](https://fedramp.gov/docs/rev5/playbook/csp/continuous-monitoring/overview/)). |
| Identity lifecycle | AC, IA, PS | Ensure only authorized users access in-scope systems. | Use documented joiner/mover/leaver workflow; require manager and system owner approval; provision through IdP groups; remove access upon termination or role change. | CSP-owned for provider staff; shared where customers control accounts | IAM owner/IT | Per request; review periodically | Access tickets, approvals, user exports, termination records | IdP, HRIS, ticketing, PAM | Sampling must reconcile HR population to active accounts. |
| Privileged access | AC, IA, AU | Restrict, approve, monitor, and review privileged access. | Enforce MFA, least privilege, PAM, named admin accounts, break-glass procedure, privileged session logging, and periodic privileged access reviews. | CSP-owned; shared for customer-owned admin roles | Security/IAM | Per request; review at least quarterly or agency-defined | PAM logs, admin list, approvals, review sign-offs, break-glass records | IdP, PAM, cloud consoles, SIEM | Privileged access to customer environments must be explicit in the boundary and CRM. |
| Remote access | AC, IA, SC | Secure remote administration paths. | Require approved VPN/ZTNA/PAM access, MFA, device posture checks, logging, session timeout, and restricted source networks for administrative access. | CSP-owned; inherited network controls may apply | Security/cloud operations | Continuous; review periodically | Remote access configuration, access logs, firewall rules, MFA settings | ZTNA/VPN, PAM, IdP, SIEM | Avoid unmanaged direct console access paths. |
| Customer environment administration | AC, CM, IR, AU | Control provider actions performed in customer environments. | Require customer-authorized work orders, least-privilege role assignment, change approval, activity logging, ticket linkage, and customer notification rules. | Shared | Managed services operations | Per customer activity | Customer tickets, work orders, approvals, activity logs, change records | ITSM, cloud consoles, PAM, SIEM | This is a key differentiator for managed services and should be covered in the CRM. |
| Logging and audit events | AU, SI | Generate, centralize, protect, and review security logs. | Define auditable events, centralize logs into SIEM, protect log integrity, synchronize time, monitor privileged activity, and retain logs per policy and agency commitments. | CSP-owned; inherited for underlying platform logs | Security operations | Continuous; review per runbook | Log source inventory, SIEM rules, alerts, review records, retention settings | SIEM, cloud logging, EDR, ticketing | Evidence should show both configuration and operational alert handling. |
| Security monitoring | AU, CA, SI, IR | Detect suspicious activity and escalate incidents. | Operate SOC monitoring, correlation rules, alert triage, escalation procedures, incident ticket creation, and periodic rule tuning. | CSP-owned; shared for customer-specific escalation | SOC/security operations | Continuous | Alert tickets, triage notes, rule inventory, escalation records | SIEM, SOAR, EDR, ITSM | Alert closure should include rationale and linkage to incident handling when applicable. |
| Vulnerability management | RA, SI, CA | Identify, prioritize, remediate, and report vulnerabilities. | Perform authenticated scans, container/image scans, web application scans, remediation ticketing, SLA tracking, exception/risk acceptance, and POA&M escalation. | CSP-owned; shared for customer assets where applicable | Security/cloud operations | Monthly or agency-defined; continuous for critical findings | Scan reports, raw scan files, tickets, closure evidence, POA&M, risk acceptances | Vulnerability scanner, ticketing, container scanner | FedRAMP ConMon requires monthly upload of updated POA&M, inventory, and vulnerability scan materials when required by agreements ([FedRAMP Continuous Monitoring Overview](https://fedramp.gov/docs/rev5/playbook/csp/continuous-monitoring/overview/)). |
| Patch management | SI, CM | Apply security updates in a timely and controlled manner. | Define severity-based patch SLAs, maintenance windows, emergency patch process, testing, deployment evidence, exceptions, and customer coordination. | CSP-owned; shared for customer-managed systems | Cloud operations/endpoint operations | Per SLA; monthly review | Patch reports, tickets, approvals, exception records | Patch tool, EDR/RMM, ITSM | Managed services must define whether patching is provider-performed or customer-approved. |
| Configuration management | CM | Establish and maintain secure baselines. | Maintain hardened baseline configurations, infrastructure-as-code review, configuration drift detection, approved deviations, and periodic configuration scans. | CSP-owned; inherited for platform baseline where applicable | Cloud operations/security engineering | Continuous; review periodically | Baseline standards, scan results, IaC pull requests, change records | IaC repo, CSP config tools, scanner | Baselines should cover cloud, OS, containers, network, endpoint, and managed-service tools. |
| Change management | CM, SA | Ensure changes are authorized, tested, documented, and monitored. | Require change tickets, risk classification, approval, test evidence, rollback plans, implementation logs, emergency change review, and significant change screening. | CSP-owned; agency/customer involvement for significant changes | Change manager/cloud operations | Per change | Change tickets, approvals, test results, deployment logs, rollback plans | ITSM, CI/CD, repository | FedRAMP ConMon includes significant change requests as post-authorization deliverables when applicable ([FedRAMP Agency Authorization Path](https://fedramp.gov/docs/rev5/playbook/csp/authorization/agency-authorization-path/)). |
| Incident response | IR | Detect, report, contain, eradicate, recover, and learn from incidents. | Maintain IR plan, severity criteria, federal/customer notification paths, escalation matrix, tabletop exercises, lessons learned, and evidence preservation process. | CSP-owned; shared for customer incidents and agency notification | Security operations/incident commander | Per incident; exercises at least annually or agency-defined | IR plan, incident tickets, timelines, communications, tabletop records, lessons learned | SIEM, SOAR, ITSM, comms tools | FedRAMP expects CSPs to respond to incidents and emergency directives as part of ConMon responsibilities ([FedRAMP Continuous Monitoring Overview](https://fedramp.gov/docs/rev5/playbook/csp/continuous-monitoring/overview/)). |
| Backup and recovery | CP | Restore service and data within defined objectives. | Define RTO/RPO, backup schedules, encryption, retention, restore tests, customer data restoration process, and DR exercise cadence. | CSP-owned; shared where customer controls data or environments | Cloud operations/backup owner | Backup per schedule; restore testing periodically | Backup job reports, restore test evidence, DR test reports, exceptions | Backup platform, cloud storage, ITSM | Managed services should separate provider platform recovery from customer environment recovery. |
| Encryption and key management | SC, IA | Protect data in transit and at rest. | Enforce TLS, storage encryption, database encryption, secret management, key rotation, access restrictions, and certificate inventory. | CSP-owned; inherited for cloud-managed encryption where documented | Security/cloud operations | Continuous; review periodically | TLS settings, encryption configs, KMS policies, key inventory, certificate inventory | KMS, secrets manager, cloud services | Distinguish inherited cloud encryption controls from application or managed-service controls. |
| Network protection | SC, AC, CM | Restrict and monitor network access. | Maintain network segmentation, security groups, firewall rules, WAF/API gateway, private connectivity, egress controls, and periodic rule reviews. | CSP-owned; inherited for cloud network fabric | Cloud operations/security | Continuous; review periodically | Network diagrams, firewall exports, security group reviews, WAF rules | Cloud network, firewall, WAF, SIEM | Firewall and security group evidence must reconcile to diagrams and inventory. |
| Endpoint and RMM tooling | CM, SI, AC, AU | Secure endpoints and remote management used by service teams. | Enforce device enrollment, EDR, disk encryption, patching, local admin restrictions, RMM access control, command logging, and device compliance. | CSP-owned; shared if customer endpoints are managed | Endpoint operations/security | Continuous; review monthly | Device inventory, EDR status, patch reports, RMM logs, compliance reports | MDM, EDR, RMM, ITSM | RMM tools are high-risk administrative pathways and should be explicitly controlled. |
| Software and automation security | SA, CM, SI | Secure scripts, automation, integrations, and managed-service tooling. | Use version control, peer review, secrets scanning, CI/CD approvals, artifact integrity checks, code scanning, and controlled deployment. | CSP-owned | Engineering/cloud operations | Per change and continuously | Pull requests, scans, approvals, deployment logs, secret scan results | Git, CI/CD, SAST, secrets manager | Scripts used to administer customer environments should be treated as in-scope operational tooling. |
| Supplier and external services | SR, SA, RA | Manage vendor and subcontractor risk. | Maintain vendor inventory, risk tiering, security reviews, contractual requirements, FedRAMP inheritance review, subcontractor access control, and periodic monitoring. | CSP-owned; inherited provider responsibilities documented | Vendor management/GRC | At onboarding and periodically | Vendor risk assessments, SOC/FedRAMP reports, contracts, monitoring records | Vendor management tool, GRC | External services that process federal data or support operations must be reflected in boundary and data flows. |
| Personnel security and training | PS, AT | Ensure personnel are vetted, trained, and accountable. | Perform onboarding, background screening where lawful/applicable, security awareness, role-based training, rules of behavior, sanctions process, and termination workflow. | CSP-owned | HR/security | At hire; annually; at termination | Training records, signed rules, onboarding/offboarding checklists, screening records | HRIS, LMS, ITSM | Support engineers and cloud admins need role-based training tied to federal operations. |
| Media and data handling | MP, SC, AC | Protect federal data and media. | Define data classification, handling, transfer, storage, sanitization, removable media restrictions, export controls, and customer data return/destruction procedures. | CSP-owned; shared for customer data handling | Security/privacy/operations | Continuous; review periodically | Data handling policy, DLP logs, destruction records, transfer approvals | DLP, storage, ITSM | Managed services must define whether customer data is viewed, stored, copied, exported, or only administered in place. |
| Physical and environmental controls | PE | Protect facilities and physical assets. | Inherit cloud data center controls where applicable; implement office and endpoint physical security for provider facilities and devices. | Inherited for cloud facilities; CSP-owned for offices/endpoints | Facilities/IT | Continuous; review periodically | Cloud provider package references, office access logs, device inventory | Cloud provider documentation, badge system | Do not claim inherited coverage without identifying the inherited provider and capability. |
| Privacy and data protection | PT, RA, AC | Protect PII and sensitive data. | Maintain data inventory, privacy impact inputs, data minimization, access restrictions, incident escalation, retention, and customer data processing commitments. | Shared | Privacy/security/legal | At onboarding and upon change | Data inventory, privacy review, retention schedule, access records | GRC, DLP, storage | Privacy controls may depend on agency requirements and customer data types. |
| Continuous monitoring | CA, RA, CM, SI, IR | Maintain authorization posture after assessment. | Operate monthly POA&M, vulnerability scans, inventory updates, incident reporting, significant change management, deviation requests, and annual assessment support. | CSP-owned; agency reviews ongoing risk | FedRAMP program manager/security | Monthly, annually, and as needed | ConMon package, updated POA&M, scan files, inventory, incident reports, annual assessment evidence | GRC, scanner, CMDB, repository | FedRAMP states CSPs maintain controls in the SSP, monitor control effectiveness, address vulnerabilities, respond to incidents, and provide information to agencies, the PMO, and assessors ([FedRAMP Continuous Monitoring Overview](https://fedramp.gov/docs/rev5/playbook/csp/continuous-monitoring/overview/)). |

## Evidence request starter list

| Request ID | Area | Evidence needed | Owner | Period covered | Notes |
|---|---|---|---|---|---|
| ER-01 | Boundary | Current boundary diagram, data-flow diagrams, network diagram, inventory, interconnections | System owner/cloud operations | Current | Reconcile all diagrams with inventory and SSP. |
| ER-02 | Access | Current user export for IdP, cloud consoles, PAM, ticketing, SIEM, RMM, backup, and customer admin tools | IAM owner | Current | Include privileged flag, role, status, last login, and creation date where available. |
| ER-03 | Access | New user, transfer, and termination samples | IT/HR | Assessment period | Include approval, provisioning, deprovisioning, and timing evidence. |
| ER-04 | Privileged access | Admin account inventory, PAM configuration, privileged access reviews, break-glass records | Security/IAM | Assessment period | Separate standing, temporary, emergency, and service account access. |
| ER-05 | Logging | Log source inventory, SIEM rules, alert tickets, retention settings, time synchronization evidence | SOC/security | Assessment period | Demonstrate both collection and review/response. |
| ER-06 | Vulnerability | Authenticated scan reports, raw scan files, remediation tickets, SLA metrics, exceptions, POA&M entries | Security/cloud operations | Monthly samples | Include OS, database, web app, container, and configuration scanning where applicable. |
| ER-07 | Change | Standard and emergency change tickets, approvals, testing, rollback, deployment logs | Change manager | Assessment period | Include significant change screening after authorization. |
| ER-08 | Configuration | Secure baseline standards, configuration scans, IaC reviews, deviation records | Cloud operations | Assessment period | Include cloud, OS, container, network, and endpoint baselines. |
| ER-09 | Incident response | IR plan, incident tickets, tabletop exercise, lessons learned, notification decisions | Security operations | Assessment period | Include false positives and escalations if no confirmed incidents occurred. |
| ER-10 | Backup and recovery | Backup configuration, job reports, restore tests, DR test records | Backup owner/cloud operations | Assessment period | Show successful recovery, not just backup completion. |
| ER-11 | Vendor risk | Vendor inventory, risk assessments, security reports, contract security terms, monitoring records | Vendor management | Current and assessment period | Include subcontractors and tooling providers supporting federal services. |
| ER-12 | Training/personnel | Security awareness, role-based training, signed rules of behavior, onboarding/offboarding records | HR/security | Assessment period | Include managed services engineers, SOC analysts, and cloud administrators. |
| ER-13 | Customer operations | Work orders, customer approvals, admin activity logs, customer change tickets, escalation records | Managed services operations | Assessment period | Essential for MSP/MSSP control testing. |
| ER-14 | Continuous monitoring | Monthly POA&M, inventory, vulnerability scans, incidents, deviations, significant changes, annual assessment support | FedRAMP program manager | Monthly/annual | FedRAMP describes monthly, annual, every-three-year, and as-needed ConMon deliverable cadences ([FedRAMP Continuous Monitoring Overview](https://fedramp.gov/docs/rev5/playbook/csp/continuous-monitoring/overview/)). |

## Customer responsibility matrix starter

| Control area | Provider responsibility | Customer responsibility | Inherited provider responsibility | Evidence available from provider | Customer evidence needed |
|---|---|---|---|---|---|
| Access management | Provide secure identity integration, role definitions, MFA enforcement for provider staff, PAM for provider admins | Approve customer users/admins, define customer roles, review customer-side access | Cloud identity or infrastructure controls where applicable | Access configuration, provider admin reviews, PAM logs | Customer user approvals, customer access reviews |
| Customer environment changes | Perform approved work, document changes, test where applicable, retain logs | Approve customer-impacting changes, validate business impact, approve maintenance windows | Cloud platform change controls where inherited | Change tickets, implementation logs, rollback evidence | Customer approvals and acceptance evidence |
| Vulnerability remediation | Scan provider-managed components, open remediation tickets, report unresolved weaknesses | Approve downtime, remediate customer-owned components, accept customer-specific risks | Cloud provider infrastructure vulnerability management | Scan reports, tickets, POA&M updates | Customer remediation tickets or risk acceptances |
| Incident response | Detect, triage, contain provider-side events, notify customer per agreement, preserve evidence | Make agency/customer notification decisions where customer owns the ATO, provide mission impact input | Cloud provider incident response for inherited infrastructure | Incident tickets, timelines, logs, notifications | Customer notification decisions, mission impact determinations |
| Backup and recovery | Operate backup tooling for provider-managed systems, test restores, report failures | Define customer recovery objectives and approve restoration priorities | Cloud storage durability and infrastructure recovery | Backup reports, restore tests | Customer RTO/RPO approvals and restore acceptance |
| Data handling | Protect provider-held customer data, enforce least privilege, restrict exports | Define data sensitivity, authorize data sharing/export, manage agency-specific retention | Cloud storage and physical controls where inherited | Data handling policy, access logs, transfer records | Customer data classification and retention requirements |

## Common gaps to remediate early

- **Undefined boundary**: The SSP, diagrams, inventory, tool list, and customer responsibility matrix do not match.
- **Overstated inheritance**: Controls are marked inherited without naming the provider, capability, or package evidence.
- **Ticket-only evidence**: Tickets exist, but they do not include approval, implementation, testing, closure, or timestamps.
- **Privileged access ambiguity**: Admin accounts, service accounts, break-glass accounts, and customer-environment access are not separately identified.
- **Vulnerability process weakness**: Scans are run, but findings are not tied to severity-based remediation SLAs, tickets, POA&M entries, or risk acceptance.
- **RMM and remote admin risk**: Remote management tooling is used operationally but omitted from the boundary, inventory, logging, or access reviews.
- **Customer responsibility gaps**: Contracts mention customer obligations, but the security package does not clearly define customer evidence and responsibilities.
- **ConMon immaturity**: Monthly POA&M, inventory, scan, incident, deviation, and significant change workflows are not operating before assessment.

## First 30, 60, and 90 days

### First 30 days

- Appoint executive sponsor, FedRAMP program manager, system owner, and security owner.
- Confirm target baseline and authorization strategy.
- Define service offering and preliminary authorization boundary.
- Create the master inventory of tools, cloud accounts, customer administration paths, external services, and privileged access paths.
- Start the customer responsibility matrix.
- Select GRC, evidence repository, and systems of record for access, change, vulnerability, incidents, vendors, and POA&M.

### First 60 days

- Complete boundary, data-flow, network, inventory, external service, and inherited-control documentation.
- Perform a control and evidence gap assessment.
- Build remediation backlog and initial POA&M candidates.
- Implement or tighten MFA, privileged access, access reviews, logging, vulnerability scanning, change control, and inventory reconciliation.
- Begin drafting core policies and procedures.

### First 90 days

- Start control implementation narratives and SSP sections.
- Produce repeatable evidence for access, change, vulnerability, incident, backup, logging, and vendor processes.
- Conduct first internal ConMon cycle with POA&M, inventory, scan outputs, incidents, deviations, and change review.
- Train managed services, SOC, cloud operations, and help desk teams on evidence expectations.
- Schedule readiness review milestones and potential 3PAO discussions.

## Success metrics

| Metric | Target behavior |
|---|---|
| Boundary reconciliation | SSP, diagrams, inventory, data flows, external services, and scan scope reconcile without unexplained differences. |
| Evidence completeness | Control evidence includes population, timestamp, owner, approval, outcome, and exceptions. |
| Access governance | All privileged and customer-environment access is approved, reviewed, logged, and removable on termination or role change. |
| Vulnerability governance | Findings are scanned, ticketed, remediated, risk accepted, or placed on POA&M within defined timelines. |
| Change governance | All production and customer-impacting changes have approval, testing, implementation, and rollback evidence. |
| ConMon readiness | Monthly POA&M, inventory, scans, incidents, deviations, and significant changes are collected before assessment. |
| Shared responsibility clarity | Each shared control has provider obligations, customer obligations, inherited elements, provider evidence, and customer evidence. |

## Recommended next artifacts

1. FedRAMP boundary and data-flow diagram package.
2. Detailed FedRAMP Moderate control applicability matrix with exact control IDs and enhancements.
3. SSP control implementation statements for high-risk families: AC, AU, CA, CM, IA, IR, RA, SC, SI, SR.
4. Managed services customer responsibility matrix.
5. Evidence request list and evidence tracker.
6. POA&M tracker with remediation owners and milestones.
7. Continuous monitoring calendar and monthly package checklist.
8. 3PAO readiness interview plan.

