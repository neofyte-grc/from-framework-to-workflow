# Stakeholder Accountability and RACI

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

This document assigns responsibility, accountability, approval authority, evidence ownership, and escalation duties across PLG’s identity and access management lifecycle.

The model is intended to prevent:

- Unclear ownership
- Self-approval
- Unauthorized provisioning
- Incomplete verification
- Unresolved access-review decisions
- Informal risk acceptance
- Delayed escalation
- Weak evidence custody

---

## 2. RACI Definitions

| Designation | Meaning |
| --- | --- |
| Responsible | Performs or coordinates the activity |
| Accountable | Owns the outcome and has final decision authority |
| Consulted | Provides subject-matter input |
| Informed | Receives status or decision information |

Each activity should have one clearly identified accountable role.

---

## 3. Stakeholder Register

| Role ID | Stakeholder | Primary accountability |
| --- | --- | --- |
| `ROLE-001` | COO | Executive sponsorship and critical-risk decisions |
| `ROLE-002` | CIO / IT Director | IAM technology, provisioning, and technical performance |
| `ROLE-003` | GRC Analyst | Requirements, risk, controls, evidence, testing, and reporting |
| `ROLE-004` | HR Manager | Authoritative workforce-status information |
| `ROLE-005` | Department Manager | Business-need validation and user-access certification |
| `ROLE-006` | System Owner | Entitlement design and system-specific authorization |
| `ROLE-007` | IT Service Desk | Provisioning, modification, disablement, and ticket evidence |
| `ROLE-008` | Information Security Lead | Privileged access, monitoring, and security escalation |
| `ROLE-009` | Finance Manager | Financial-system access and segregation-of-duties decisions |
| `ROLE-010` | Vendor Manager | Third-party access coordination and vendor escalation |
| `ROLE-011` | Physical Security / Facilities | Badge, key, and facility-access management |
| `ROLE-012` | Internal Auditor / Assessor | Independent control assessment |
| `ROLE-013` | User or Requester | Accurate request information and policy compliance |
| `ROLE-014` | Contractor Sponsor | Business ownership for contractor and courier access |

---

## 4. Stakeholder Responsibilities

### 4.1 COO

The COO:

- Sponsors the IAM program.
- Resolves cross-functional accountability conflicts.
- Reviews material IAM risks.
- Accepts Critical residual risk when appropriate.
- Supports resource and remediation decisions.

### 4.2 CIO / IT Director

The CIO or IT Director:

- Owns IAM technical operations.
- Ensures provisioning and revocation processes are maintained.
- Defines technical service levels.
- Resolves system-integration issues.
- Escalates material technical control failures.

### 4.3 GRC Analyst

The GRC Analyst:

- Maintains the requirements register.
- Coordinates risk assessments.
- Documents control objectives.
- Maintains evidence and testing expectations.
- Tracks metrics, exceptions, findings, and POA&M items.
- Reports control health to leadership.

### 4.4 HR Manager

The HR Manager:

- Maintains authoritative workforce-status information.
- Initiates joiner, mover, and leaver events.
- Confirms effective dates.
- Protects sensitive termination information.
- Escalates delayed or failed workforce notifications.

### 4.5 Department Manager

The Department Manager:

- Validates business need.
- Selects the appropriate business role.
- Reviews requested access for least privilege.
- Certifies or revokes access during periodic reviews.
- Escalates unclear or disputed entitlements.

### 4.6 System Owner

The System Owner:

- Defines available roles and entitlements.
- Approves sensitive and nonstandard access.
- Identifies incompatible permissions.
- Reviews access populations.
- Accepts eligible risk within delegated authority.

### 4.7 IT Service Desk

The IT Service Desk:

- Executes approved provisioning and removal.
- Records timestamps and technical actions.
- Identifies provisioning discrepancies.
- Maintains service-ticket evidence.
- Escalates requests that lack complete approval.

### 4.8 Information Security Lead

The Information Security Lead:

- Reviews privileged and high-risk access.
- Defines enhanced authentication and monitoring.
- Investigates suspected misuse.
- Reviews emergency-access activity.
- Escalates security events and material control failures.

---

## 5. RACI Matrix

| Activity | COO | CIO | GRC | HR | Manager | System Owner | IT | Security |
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
| Establish IAM policy | I | A | R | C | C | C | C | C |
| Initiate joiner event | I | I | I | R/A | C | I | I | I |
| Initiate mover event | I | I | I | R/A | C | I | I | I |
| Initiate leaver event | I | I | I | R/A | C | I | I | C |
| Validate business need | I | I | I | C | R/A | C | I | I |
| Define business roles | I | C | C | C | R | A | C | C |
| Approve standard access | I | I | I | C | R | A | I | I |
| Approve privileged access | I | C | C | I | R | C | I | A |
| Check segregation of duties | I | I | C | I | C | A | I | C |
| Provision access | I | A | I | I | I | C | R | C |
| Verify provisioning | I | C | A | I | C | C | R | C |
| Conduct periodic review | I | I | C | I | R | A | C | C |
| Remove access | I | A | I | C | C | C | R | C |
| Approve Moderate exception | I | C | R | I | C | A | I | C |
| Approve High exception | I | A | R | I | C | C | I | C |
| Approve Critical exception | A | R | C | I | I | C | I | C |
| Maintain evidence catalog | I | C | R/A | C | C | C | C | C |
| Assess control effectiveness | I | C | R | I | I | C | C | C |
| Approve finding closure | I | C | R/A | C | C | C | C | C |

---

## 6. Segregation-of-Duties Principles

PLG will apply the following principles:

- A requester may not approve their own elevated access.
- A provisioner may not be the sole verifier for high-risk access.
- A user may not certify their own access.
- A control operator should not independently assess the same control.
- A risk owner may accept risk only within documented authority.
- Finance-system access must be checked for incompatible duties.
- Emergency-access use requires retrospective review.
- Shared accounts may not replace individual accountability.

---

## 7. Decision Authority

| Decision | Minimum authority |
| --- | --- |
| Standard role-based access | Department Manager and System Owner |
| Sensitive-data access | Department Manager and System Owner |
| Privileged access | Department Manager, System Owner, and Security Lead |
| Emergency access | Security Lead or authorized incident leader |
| Moderate residual-risk exception | System Owner |
| High residual-risk exception | CIO / IT Director |
| Critical residual-risk exception | COO |
| Control-finding closure | GRC Analyst with control-owner validation |

---

## 8. Governance Cadence

| Cadence | Meeting or review | Participants |
| --- | --- | --- |
| Daily | Critical revocation and access-event monitoring | IT, HR, and Security |
| Weekly | IAM operational review | IT, GRC, HR, and process owners |
| Monthly | Control-health review | CIO, Security, GRC, and System Owners |
| Quarterly | Access certification and risk review | Managers, System Owners, GRC, and leadership |
| Event-driven | Material incident or control failure | Relevant owners and executive authority |

---

## 9. Escalation Path

1. The performer attempts routine resolution.
2. The process owner reviews unresolved issues.
3. GRC documents the control or risk impact.
4. The CIO and Security Lead address High-risk issues.
5. The COO receives Critical-risk or cross-functional escalation.
6. An incident-response process is initiated when misuse or compromise is suspected.

---

## 10. Accountability Principles

PLG’s operating model is based on the following principles:

- Every control has an accountable owner.
- Every user has an accountable manager or sponsor.
- Every entitlement has an accountable System Owner.
- Every exception has an accountable risk owner.
- Every finding has a corrective-action owner.
- Every escalation has a defined recipient and response time.
- Every closure decision is supported by evidence.
