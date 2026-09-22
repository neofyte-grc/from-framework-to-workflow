# From Framework to Workflow

## Turning GRC Controls Into Operational Processes

![Project Status](https://img.shields.io/badge/status-in%20progress-yellow)
![Focus](https://img.shields.io/badge/focus-GRC%20Engineering-blue)
![Control Domain](https://img.shields.io/badge/domain-Identity%20%26%20Access%20Management-purple)

> A fictional GRC engineering case study demonstrating how governance requirements become accountable, measurable, evidence-producing operational workflows.

---

## Executive Overview

Peachtree Logistics Group (PLG) is a fictional regional logistics company headquartered in Atlanta, Georgia. PLG employs approximately 225 office, warehouse, dispatch, and driving personnel and also relies on independent couriers. Its mixed cloud and on-premises environment supports Microsoft 365, logistics and freight software, a warehouse management system, dispatch applications, and billing systems.

PLG has policies and informal access practices, but it lacks a consistent method for converting access-control requirements into repeatable operations. Requests, approvals, provisioning, reviews, revocations, exceptions, and evidence collection vary by system and department.

This project designs a governed identity and access management operating model that connects:

> Business requirement → Risk → Framework requirement → Control objective → Workflow → Owner → Evidence → Test → Metric → Exception → Improvement

The project emphasizes process engineering, accountability, human execution, and auditability—not checkbox compliance.

---

## Project Objectives

- Translate selected IAM requirements into executable control activities.
- Define accountable owners, approvers, performers, reviewers, and escalation authorities.
- Design joiner, mover, leaver, access-request, provisioning, review, privileged-access, revocation, and exception workflows.
- Establish evidence requirements and assessment procedures.
- Identify responsible automation opportunities while preserving human approval.
- Define KPIs, KRIs, thresholds, and escalation actions.
- Build end-to-end traceability from requirement through remediation.

---

## Scope

### In Scope

- Microsoft 365
- Cloud logistics and freight brokerage platform
- On-premises warehouse management system
- Dispatch and delivery platform
- Billing and accounting system
- Employee and contractor identities
- Standard, temporary, elevated, and privileged access
- Logical and related physical-access coordination
- Access evidence, testing, monitoring, exceptions, and remediation

### Out of Scope

- Production deployment or configuration
- Live penetration testing
- Independent audit, certification, or authorization
- Legal opinions or formal compliance determinations
- Real employee, contractor, customer, patient, or company-sensitive data
- Claims that PLG operates the designed controls in production

---

## Framework Alignment

| Source | Project Use |
| --- | --- |
| NIST Cybersecurity Framework 2.0 | Governance and Protect outcomes, including identity management, authentication, and access control |
| NIST SP 800-53 Release 5.2.0 | Selected AC, IA, AU, CA, CM, PS, RA, and PM controls |
| NIST SP 800-53A Release 5.2.0 | Control assessment concepts and examine, interview, and test methods |
| NIST SP 800-37 Rev. 2 | Risk-based selection, implementation, assessment, and continuous monitoring concepts |
| FedRAMP-style practices | Implementation statements, evidence, findings, and POA&M-style remediation tracking |

Framework alignment does not represent certification, authorization, or formal compliance.

---

## Core Workflows

| Workflow ID | Workflow | Primary Outcome |
| --- | --- | --- |
| `WF-001` | Joiner-Mover-Leaver | Access follows the workforce lifecycle |
| `WF-002` | Access Request and Approval | Access is justified and authorized |
| `WF-003` | Provisioning and Verification | Approved access is implemented accurately |
| `WF-004` | Periodic Access Review | Continued access is recertified or removed |
| `WF-005` | Privileged Access | Elevated access receives stronger governance |
| `WF-006` | Termination and Emergency Revocation | Access is removed rapidly and verified |
| `WF-007` | Exception and Risk Acceptance | Deviations are documented, approved, monitored, and expired |

---

## Project Deliverables

| # | Deliverable | Purpose | Status |
| ---: | --- | --- | --- |
| 00 | [Project Overview and Methodology](docs/00-project-overview-and-methodology.md) | Defines scope, method, identifiers, evidence rules, and completion criteria | 🚧 In Progress |
| 01 | [Organization and Operating Context](docs/01-organization-and-operating-context.md) | Documents PLG's business, workforce, systems, data, and operational constraints | 🚧 In Progress |
| 02 | [Business Problem and Control Scope](docs/02-business-problem-and-control-scope.md) | Defines the IAM problem, boundaries, outcomes, and exclusions | 🚧 In Progress |
| 03 | [Stakeholder Accountability and RACI](docs/03-stakeholder-accountability-and-raci.md) | Assigns ownership, decision rights, execution, evidence, and escalation duties | 🚧 In Progress |
| 04 | [Framework and Requirements Register](docs/04-framework-and-requirements-register.md) | Maps authoritative requirements to risks, controls, workflows, and evidence | 🚧 In Progress |
| 05 | [Control Objective Decomposition](docs/05-control-objective-decomposition.md) | Converts high-level requirements into implementable control activities | 🚧 In Progress |
| 06 | [Access Management Risk Register](docs/06-access-management-risk-register.md) | Records and prioritizes IAM risks and treatments | 🚧 In Progress |
| 07 | [Current-State and Future-State Analysis](docs/07-current-state-and-future-state-analysis.md) | Compares informal practices with the governed target state | 🚧 In Progress |
| 08 | [Joiner-Mover-Leaver Workflow](docs/08-joiner-mover-leaver-workflow.md) | Governs identity creation, change, and removal | 🚧 In Progress |
| 09 | [Access Request and Approval Workflow](docs/09-access-request-and-approval-workflow.md) | Standardizes requests, justification, review, and authorization | 🚧 In Progress |
| 10 | [Provisioning and Verification Workflow](docs/10-provisioning-and-verification-workflow.md) | Ensures accurate implementation and independent verification | 🚧 In Progress |
| 11 | [Periodic Access Review Workflow](docs/11-periodic-access-review-workflow.md) | Governs recertification, revocation, remediation, and escalation | 🚧 In Progress |
| 12 | [Privileged Access Management Workflow](docs/12-privileged-access-management-workflow.md) | Adds stronger controls for elevated access | 🚧 In Progress |
| 13 | [Termination and Emergency Revocation Workflow](docs/13-termination-and-emergency-revocation-workflow.md) | Coordinates urgent, verified access removal | 🚧 In Progress |
| 14 | [Access Exception and Risk Acceptance Workflow](docs/14-access-exception-and-risk-acceptance-workflow.md) | Governs time-bound deviations and compensating controls | 🚧 In Progress |
| 15 | [Evidence and Audit Trail Plan](docs/15-evidence-and-audit-trail-plan.md) | Defines evidence ownership, quality, protection, retention, and traceability | 🚧 In Progress |
| 16 | [Automation and Integration Requirements](docs/16-automation-and-integration-requirements.md) | Defines responsible automation requirements and fallback controls | 🚧 In Progress |
| 17 | [Control Failure Modes and Test Plan](docs/17-control-failure-modes-and-test-plan.md) | Identifies failure modes and designs control assessments | 🚧 In Progress |
| 18 | [KPI, KRI, and Control Health Model](docs/18-kpi-kri-and-control-health-model.md) | Defines performance, risk, and effectiveness measures | 🚧 In Progress |
| 19 | [Continuous Monitoring and Escalation Plan](docs/19-continuous-monitoring-and-escalation-plan.md) | Establishes monitoring cadence, thresholds, reporting, and escalation | 🚧 In Progress |
| 20 | [Implementation Roadmap and POA&M](docs/20-implementation-roadmap-and-poam.md) | Sequences improvements and tracks remediation | 🚧 In Progress |
| 21 | [Control Assessment and Traceability Report](docs/21-control-assessment-and-traceability-report.md) | Demonstrates end-to-end requirement-to-evidence traceability | 🚧 In Progress |
| 22 | [Executive Summary and Practitioner Reflection](docs/22-executive-summary-and-practitioner-reflection.md) | Communicates business value, limitations, and lessons learned | 🚧 In Progress |

---

## Repository Structure

```text
from-framework-to-workflow/
├── README.md
├── docs/
│   ├── 00-project-overview-and-methodology.md
│   ├── 01-organization-and-operating-context.md
│   ├── 02-business-problem-and-control-scope.md
│   ├── 03-stakeholder-accountability-and-raci.md
│   ├── 04-framework-and-requirements-register.md
│   ├── 05-control-objective-decomposition.md
│   ├── 06-access-management-risk-register.md
│   ├── 07-current-state-and-future-state-analysis.md
│   ├── 08-joiner-mover-leaver-workflow.md
│   ├── 09-access-request-and-approval-workflow.md
│   ├── 10-provisioning-and-verification-workflow.md
│   ├── 11-periodic-access-review-workflow.md
│   ├── 12-privileged-access-management-workflow.md
│   ├── 13-termination-and-emergency-revocation-workflow.md
│   ├── 14-access-exception-and-risk-acceptance-workflow.md
│   ├── 15-evidence-and-audit-trail-plan.md
│   ├── 16-automation-and-integration-requirements.md
│   ├── 17-control-failure-modes-and-test-plan.md
│   ├── 18-kpi-kri-and-control-health-model.md
│   ├── 19-continuous-monitoring-and-escalation-plan.md
│   ├── 20-implementation-roadmap-and-poam.md
│   ├── 21-control-assessment-and-traceability-report.md
│   └── 22-executive-summary-and-practitioner-reflection.md
├── policies/
│   ├── access-control-policy.md
│   ├── identity-lifecycle-management-standard.md
│   ├── access-review-standard.md
│   └── access-exception-and-escalation-standard.md
├── templates/
│   ├── access-request-form.md
│   ├── role-and-entitlement-catalog-template.md
│   ├── manager-access-review-template.md
│   ├── privileged-access-request-template.md
│   ├── termination-access-checklist.md
│   ├── access-exception-request-template.md
│   ├── control-evidence-log-template.md
│   ├── control-test-workpaper-template.md
│   └── poam-template.md
├── evidence/
│   ├── sample-completed-access-request.md
│   ├── sample-role-entitlement-record.md
│   ├── sample-provisioning-verification-record.md
│   ├── sample-quarterly-access-review.md
│   ├── sample-termination-access-record.md
│   ├── sample-access-exception-record.md
│   ├── sample-control-test-workpaper.md
│   └── sample-poam-record.md
├── diagrams/
│   ├── requirements-to-workflow-traceability.md
│   ├── iam-governance-operating-model.md
│   ├── joiner-mover-leaver-process-flow.md
│   ├── access-request-approval-flow.md
│   ├── access-review-and-remediation-flow.md
│   └── exception-and-escalation-flow.md
└── presentation/
    ├── executive-briefing.md
    └── portfolio-defense-guide.md
