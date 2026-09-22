# Joiner-Mover-Leaver Workflow

## Document Control

| Field | Value |
| --- | --- |
| Organization | Peachtree Logistics Group (fictional) |
| Workflow ID | `WF-001` |
| Workflow owner | HR Manager and IT Director |
| Version | 1.0 |
| Status | Portfolio design artifact |

---

## 1. Purpose

This workflow governs identity and access activities throughout the workforce lifecycle.

It ensures that:

- New personnel receive authorized access.
- Role changes result in appropriate access changes.
- Obsolete access is removed.
- Departed personnel lose access promptly.
- Contractor and courier access has accountable sponsorship.
- Each lifecycle event produces traceable evidence.

---

## 2. Scope

The workflow applies to:

- Employees
- Contractors
- Temporary workers
- Independent couriers
- Interns
- Vendors with named access
- Standard accounts
- Privileged accounts
- Application accounts
- Remote access
- Physical-access coordination

---

## 3. Authoritative Source

HR is the authoritative source for employee workforce status.

The Contractor Sponsor or Vendor Manager is the authoritative business source for contractor, courier, temporary, and vendor-access status.

An access event must include:

- Full name
- Unique workforce identifier
- Employment or relationship type
- Manager or sponsor
- Department
- Job or service role
- Work location
- Start or effective date
- End date when applicable
- Termination sensitivity
- Required systems
- Special data-access requirements

---

## 4. Joiner Workflow

### 4.1 Trigger

The workflow begins when HR or an authorized sponsor submits an approved workforce event.

### 4.2 Procedure

1. HR creates the joiner event.
2. The manager confirms the role, department, location, start date, and required systems.
3. IT confirms that the identity does not already have an active duplicate account.
4. Standard access is selected from the approved role catalog.
5. Nonstandard access follows `WF-002`.
6. Sensitive or privileged access receives additional approval.
7. IT provisions access no earlier than the approved activation window.
8. MFA and applicable authentication controls are configured.
9. A designated reviewer compares assigned access with approved access.
10. Discrepancies are corrected before closure.
11. The manager and user receive completion notification.
12. Evidence is retained.

### 4.3 Joiner Control Rules

- No access may be provisioned from an unverified verbal request.
- Every joiner must have a manager or sponsor.
- Contractor and courier access must have an expiration date.
- Privileged access must not be included automatically in a standard role.
- Accounts must remain inactive until the approved activation time.
- Shared accounts may not replace individual accounts.

---

## 5. Mover Workflow

### 5.1 Trigger

A mover event includes:

- Department transfer
- Promotion
- Demotion
- Temporary assignment
- Location change
- Manager change
- Employment-type change
- Leave of absence
- Return from leave
- Change in contractor responsibilities

### 5.2 Procedure

1. HR records the effective role or department change.
2. The current manager confirms the user’s existing responsibilities.
3. The new manager confirms the target responsibilities.
4. IT generates a current-access inventory.
5. The current access is compared with the target role.
6. Obsolete access is identified for removal.
7. New access follows the appropriate approval path.
8. Segregation-of-duties conflicts are evaluated.
9. Obsolete access is removed before or with the activation of new access.
10. IT records the completed changes.
11. A designated reviewer verifies the final access state.
12. Unresolved access follows the exception and escalation process.

### 5.3 Remove-Before-Addition Principle

When practical, access no longer required by the prior role should be removed before new sensitive or conflicting access is activated.

If operational timing requires overlap:

- The overlap must be documented.
- The overlap must have an expiration time.
- Conflicts must be evaluated.
- Compensating monitoring must be defined.
- The appropriate owner must approve the overlap.

---

## 6. Leaver Workflow

### 6.1 Trigger

The leaver workflow begins when HR or an authorized sponsor records:

- Voluntary termination
- Involuntary termination
- Contract expiration
- Contractor disengagement
- Courier relationship termination
- Death
- Abandonment of position
- Emergency security revocation

### 6.2 Procedure

1. HR records the separation type and effective time.
2. HR limits notification details according to need-to-know requirements.
3. IT identifies all in-scope logical accounts.
4. Facilities identifies badges, keys, and physical-access credentials.
5. The manager identifies devices, tokens, records, shared secrets, and vendor accounts.
6. IT disables central accounts at the effective time.
7. System Owners disable dependent application accounts.
8. Active sessions and remote access are revoked.
9. Privileged access is removed.
10. Shared credentials known to the departing person are rotated where required.
11. Devices, badges, keys, and tokens are recovered or recorded as unresolved.
12. A separate reviewer confirms completion.
13. Unresolved items are escalated.
14. Evidence is retained.

---

## 7. Service-Level Targets

| Event | Target |
| --- | --- |
| Standard joiner | Access available by the approved start time |
| Standard mover | Completed within one business day of the effective change |
| Contractor expiration | Access removed by the documented expiration |
| Voluntary termination | Access removed by the effective separation time |
| Involuntary termination | Coordinated immediate disablement |
| Emergency security revocation | Immediate action upon authorized request |
| High-risk discrepancy | Immediate containment and escalation |
| Standard discrepancy | Corrected within one business day |

---

## 8. Roles and Responsibilities

| Role | Responsibility |
| --- | --- |
| HR Manager | Initiates and validates employee lifecycle events |
| Contractor Sponsor | Initiates and validates nonemployee lifecycle events |
| Department Manager | Confirms business role and access need |
| System Owner | Approves system-specific access |
| IT Service Desk | Provisions, modifies, and disables access |
| Security Lead | Reviews privileged and emergency access |
| Facilities | Manages physical-access credentials |
| GRC Analyst | Monitors evidence, exceptions, metrics, and failures |
| CIO / IT Director | Owns technical performance and escalation |

---

## 9. Evidence Requirements

| Evidence ID | Evidence |
| --- | --- |
| `EVID-001` | Authoritative workforce event |
| `EVID-002` | Approved access request |
| `EVID-003` | Provisioning or modification record |
| `EVID-005` | Role and entitlement comparison |
| `EVID-007` | Disablement and revocation record |
| `EVID-008` | Mover access-comparison record |
| `EVID-011` | Independent verification record |

---

## 10. Exceptions

Exceptions may include:

- Required temporary access overlap
- Vendor limitation preventing immediate automated removal
- Emergency-access activation
- Operational continuity requirement
- System outage affecting the normal process

Exceptions must:

- Identify the unmet requirement.
- Document the business need.
- Assess the risk.
- Establish compensating controls.
- Assign an owner.
- Receive authorized approval.
- Include an expiration date.
- Be monitored through closure.

---

## 11. Failure Conditions

The workflow is considered unsuccessful when:

- The workforce event is incomplete or unverifiable.
- Access is granted before approval.
- The wrong role is assigned.
- Obsolete access remains active.
- A terminated user remains enabled beyond the required time.
- Contractor access lacks expiration.
- Privileged access is included without enhanced approval.
- Verification is not completed.
- Required evidence is missing.
- Unresolved items are closed without risk disposition.

---

## 12. Metrics

The workflow supports:

- `MET-001` — Access requests completed within SLA
- `MET-002` — Requests with complete approvals
- `MET-003` — Termination-to-disablement performance
- `MET-005` — Overdue revocations
- `MET-008` — Evidence completeness
- `MET-009` — Control-test exception rate
