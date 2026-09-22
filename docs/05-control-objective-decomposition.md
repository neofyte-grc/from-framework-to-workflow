# Control Objective Decomposition

## Document Control

| Field | Value |
| --- | --- |
| Organization | Peachtree Logistics Group (fictional) |
| Project | From Framework to Workflow |
| Document owner | GRC Analyst |
| Version | 1.0 |
| Status | Portfolio design artifact |

---

## 1. Purpose

This document converts high-level IAM requirements into specific and executable control activities.

Each control is defined through:

- Objective
- Risk addressed
- Trigger
- Inputs
- Activity
- Responsible role
- Accountable owner
- Evidence
- Frequency
- Failure condition
- Escalation response
- Performance measure

---

## 2. Control Types

| Control type | Purpose |
| --- | --- |
| Preventive | Stops unauthorized or inappropriate access before it occurs |
| Detective | Identifies access failures, misuse, or control breakdowns |
| Corrective | Removes inappropriate access or resolves a control failure |
| Directive | Establishes required behavior or operating expectations |
| Compensating | Reduces risk when the primary control cannot be implemented |

---

## 3. Control Catalog

### `CTRL-001` — Account Lifecycle Authorization

| Attribute | Definition |
| --- | --- |
| Objective | Ensure accounts are created, changed, disabled, and removed only through authorized workforce events |
| Risks addressed | `IAM-RISK-001`, `IAM-RISK-005`, `IAM-RISK-006` |
| Requirements | `REQ-001`, `REQ-003`, `REQ-009`, `REQ-011`, `REQ-012` |
| Trigger | Joiner, mover, leave, termination, contract expiration, or emergency event |
| Inputs | HR event, manager confirmation, role, effective date, system list |
| Activity | Validate the event and initiate the appropriate account action |
| Responsible | HR and IT Service Desk |
| Accountable | IT Director |
| Evidence | `EVID-001`, `EVID-003`, `EVID-007`, `EVID-008` |
| Frequency | Event-driven |
| Failure condition | Account action is missing, late, inaccurate, or unauthorized |
| Escalation | CIO and Security Lead for High or Critical failures |
| Metric | `MET-003`, `MET-005` |

### `CTRL-002` — Least Privilege and Segregation of Duties

| Attribute | Definition |
| --- | --- |
| Objective | Limit access to approved job requirements and prevent incompatible permissions |
| Risks addressed | `IAM-RISK-002`, `IAM-RISK-003` |
| Requirements | `REQ-005`, `REQ-006` |
| Trigger | New access request, role change, access review, or exception |
| Inputs | Role catalog, entitlement catalog, SoD rules, business justification |
| Activity | Compare requested access with job need and prohibited combinations |
| Responsible | Department Manager and System Owner |
| Accountable | System Owner |
| Evidence | `EVID-004`, `EVID-005` |
| Frequency | Per request and during reviews |
| Failure condition | Excessive or conflicting access is approved |
| Escalation | Security Lead and GRC Analyst |
| Metric | `MET-002`, `MET-009` |

### `CTRL-003` — Provisioning Accuracy and Verification

| Attribute | Definition |
| --- | --- |
| Objective | Ensure implemented access matches the approved request |
| Risks addressed | `IAM-RISK-001`, `IAM-RISK-002` |
| Requirements | `REQ-003`, `REQ-004`, `REQ-008` |
| Trigger | Provisioning or access modification completion |
| Inputs | Approved request, assigned role, system account record |
| Activity | Compare actual access with authorized access |
| Responsible | IT Service Desk and designated verifier |
| Accountable | IT Director |
| Evidence | `EVID-003`, `EVID-011` |
| Frequency | Per transaction |
| Failure condition | Actual access differs from approval |
| Escalation | Immediate escalation for unauthorized privileged access |
| Metric | `MET-001`, `MET-008` |

### `CTRL-004` — Timely Access Removal

| Attribute | Definition |
| --- | --- |
| Objective | Remove obsolete or unauthorized access within established service levels |
| Risks addressed | `IAM-RISK-005`, `IAM-RISK-006` |
| Requirements | `REQ-003`, `REQ-011`, `REQ-012` |
| Trigger | Termination, transfer, leave, contract expiration, or emergency |
| Inputs | HR event, current access, target role, effective time |
| Activity | Disable or modify all applicable logical and physical access |
| Responsible | IT, Facilities, and System Owners |
| Accountable | IT Director |
| Evidence | `EVID-007`, `EVID-008` |
| Frequency | Event-driven |
| Failure condition | Obsolete access remains active beyond the SLA |
| Escalation | CIO and Security Lead |
| Metric | `MET-003`, `MET-005` |

### `CTRL-005` — Periodic Access Certification

| Attribute | Definition |
| --- | --- |
| Objective | Confirm that existing access remains appropriate and authorized |
| Risks addressed | `IAM-RISK-002`, `IAM-RISK-003`, `IAM-RISK-006` |
| Requirements | `REQ-003`, `REQ-006`, `REQ-015`, `REQ-017` |
| Trigger | Scheduled review or material change |
| Inputs | Complete account and entitlement population, HR status, role information |
| Activity | Certify, revoke, modify, or escalate access |
| Responsible | Department Managers |
| Accountable | System Owner |
| Evidence | Access-review package and remediation records |
| Frequency | Quarterly or semiannually based on risk |
| Failure condition | Review is incomplete, late, inaccurate, or unsupported |
| Escalation | CIO and GRC Analyst |
| Metric | `MET-004`, `MET-005` |

### `CTRL-006` — Privileged-Access Governance

| Attribute | Definition |
| --- | --- |
| Objective | Restrict, monitor, and periodically review elevated access |
| Risks addressed | `IAM-RISK-007` |
| Requirements | `REQ-005`, `REQ-006`, `REQ-007`, `REQ-013`, `REQ-014`, `REQ-018` |
| Trigger | Privileged-access request, emergency need, review date, or expiration |
| Inputs | Business need, scope, duration, approvals, monitoring requirements |
| Activity | Approve, provision, monitor, review, and revoke privileged access |
| Responsible | IT and Security |
| Accountable | Security Lead |
| Evidence | Privileged request, account record, logs, and review |
| Frequency | Event-driven and monthly |
| Failure condition | Privileged access lacks approval, monitoring, review, or expiration |
| Escalation | CIO and Security Lead |
| Metric | `MET-007` |

### `CTRL-007` — Exception and Risk-Acceptance Governance

| Attribute | Definition |
| --- | --- |
| Objective | Ensure deviations are risk-assessed, approved, time-bound, and monitored |
| Risks addressed | All applicable IAM risks |
| Requirements | `REQ-016`, `REQ-017`, `REQ-019` |
| Trigger | A requirement cannot be met |
| Inputs | Business justification, affected assets, risk, alternatives, duration |
| Activity | Evaluate risk, establish compensating controls, approve, monitor, and close |
| Responsible | GRC Analyst |
| Accountable | Authorized risk owner |
| Evidence | Exception record and monitoring results |
| Frequency | Event-driven and at scheduled review |
| Failure condition | Exception lacks authority, compensation, expiration, or monitoring |
| Escalation | Based on residual-risk level |
| Metric | `MET-006` |

### `CTRL-008` — IAM Policy Governance

| Attribute | Definition |
| --- | --- |
| Objective | Maintain approved and current access-control requirements |
| Risks addressed | `IAM-RISK-008` |
| Requirements | `REQ-002` |
| Trigger | Annual review or material change |
| Inputs | Framework updates, findings, incidents, operational changes |
| Activity | Review, approve, communicate, and update IAM governance documents |
| Responsible | GRC Analyst |
| Accountable | CIO |
| Evidence | Approved policy, review record, and communication evidence |
| Frequency | At least annually |
| Failure condition | Requirements become outdated or are not communicated |
| Escalation | CIO and COO |
| Metric | Policy-review completion |

### `CTRL-009` — Identity and Authentication Management

| Attribute | Definition |
| --- | --- |
| Objective | Ensure users are uniquely identified and appropriately authenticated |
| Risks addressed | `IAM-RISK-004` |
| Requirements | `REQ-008`, `REQ-009`, `REQ-010` |
| Trigger | Account creation, credential issuance, reset, compromise, or termination |
| Inputs | Verified identity, identifier, authentication requirements |
| Activity | Assign unique identifier and manage authenticators securely |
| Responsible | IT Service Desk |
| Accountable | Security Lead |
| Evidence | Identity, MFA, token, and credential records |
| Frequency | Event-driven |
| Failure condition | Shared, duplicate, weak, or untraceable authentication |
| Escalation | Security Lead |
| Metric | MFA and unique-account coverage |

### `CTRL-010` — Control Assessment

| Attribute | Definition |
| --- | --- |
| Objective | Evaluate control design and operating effectiveness |
| Risks addressed | `IAM-RISK-008` |
| Requirements | `REQ-015` |
| Trigger | Assessment schedule, material change, or significant failure |
| Inputs | Control definition, population, evidence, prior findings |
| Activity | Examine, interview, test, document results, and report findings |
| Responsible | GRC Analyst or independent assessor |
| Accountable | CIO |
| Evidence | Assessment workpapers and findings |
| Frequency | At least annually or risk-based |
| Failure condition | Assessment is incomplete, unsupported, or lacks independence |
| Escalation | CIO and Audit Committee or equivalent |
| Metric | `MET-009` |

### `CTRL-011` — Continuous Monitoring and Improvement

| Attribute | Definition |
| --- | --- |
| Objective | Detect control degradation and drive corrective action |
| Risks addressed | `IAM-RISK-008` |
| Requirements | `REQ-017`, `REQ-020` |
| Trigger | Monitoring schedule, threshold breach, change, or incident |
| Inputs | KPIs, KRIs, findings, incidents, exceptions, and system changes |
| Activity | Review trends, escalate breaches, assign remediation, and retest |
| Responsible | GRC Analyst |
| Accountable | CIO |
| Evidence | Dashboard, meeting record, POA&M, and retest evidence |
| Frequency | Monthly and quarterly |
| Failure condition | Material control weakness remains unidentified or unresolved |
| Escalation | CIO and COO |
| Metric | POA&M timeliness and control-health rating |

---

## 4. Control-Design Principles

PLG’s control design follows these principles:

- Every control addresses a documented risk.
- Every control maps to a requirement.
- Every control has one accountable owner.
- Evidence is created as part of the workflow.
- High-risk activities require stronger approval.
- Request, approval, provisioning, and verification are separated where practical.
- Exceptions are documented and temporary.
- Failures trigger escalation and corrective action.
- Metrics measure outcomes, not merely activity volume.
- Automation does not eliminate human accountability.
