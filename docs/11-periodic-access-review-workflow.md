# Periodic Access Review Workflow

## Document Control

| Field | Value |
| --- | --- |
| Organization | Peachtree Logistics Group (fictional) |
| Workflow ID | `WF-004` |
| Workflow owner | System Owner |
| Coordinator | GRC Analyst |
| Version | 1.0 |
| Status | Portfolio design artifact |

---

## 1. Purpose

This workflow defines how PLG periodically evaluates whether existing user access remains authorized, appropriate, and necessary.

The review process is designed to identify:

- Access belonging to inactive users
- Access no longer required for current duties
- Excessive permissions
- Privilege accumulation
- Segregation-of-duties conflicts
- Expired temporary access
- Unapproved privileged access
- Contractor access without a current sponsor
- Accounts without an identifiable owner
- Access that cannot be supported by reliable evidence

---

## 2. Scope

Periodic reviews cover:

- Employees
- Contractors
- Independent couriers
- Temporary workers
- Privileged administrators
- Standard user accounts
- Privileged accounts
- Service and shared accounts
- Application roles
- Group memberships
- Remote-access permissions
- Sensitive-data access
- Physical access where coordinated with IAM

---

## 3. Review Frequency

| Access category | Minimum frequency |
| --- | --- |
| Privileged access | Quarterly |
| Financial-system access | Quarterly |
| Medical-delivery information | Quarterly |
| Remote administrative access | Quarterly |
| Standard business-system access | Semiannually |
| Contractor and courier access | Quarterly |
| Service and shared accounts | Quarterly |
| Physical access | Semiannually |
| Event-driven access | Following a material change |

A System Owner may require more frequent review based on risk, incidents, findings, or operational change.

---

## 4. Review Population

The review population should include:

- User identifier
- User name
- Workforce type
- Employment status
- Department
- Manager or sponsor
- System
- Account name
- Role
- Entitlements
- Privileged status
- Account status
- Creation date
- Last sign-in or use date where available
- Approval reference
- Temporary-access expiration
- Existing exception
- Prior review decision

The population must be reconciled against authoritative HR, contractor, and system records before distribution.

---

## 5. Workflow

### Step 1 — Review Initiation

The GRC Analyst defines:

- Review period
- Systems in scope
- User population
- Reviewers
- Due date
- Escalation dates
- Required evidence
- Quality-assurance approach

### Step 2 — Population Generation

IT or the System Owner extracts all in-scope accounts and entitlements.

Filters must not remove:

- Disabled accounts awaiting deletion
- Dormant accounts
- Service accounts
- Shared accounts
- Privileged accounts
- Contractor accounts
- Accounts without an identified owner

### Step 3 — Population Reconciliation

The population is compared with:

- HR workforce records
- Contractor and courier records
- Approved role catalogs
- Prior access-review results
- Approved exceptions
- Termination and transfer records

Unexplained differences must be resolved or included in the review.

### Step 4 — Reviewer Assignment

Access is assigned to a reviewer with sufficient knowledge and authority.

Reviewers may include:

- Department Managers
- System Owners
- Data Owners
- Contractor Sponsors
- Security personnel

Users may not certify their own access.

### Step 5 — Reviewer Decision

The reviewer selects one of the following:

| Decision | Meaning |
| --- | --- |
| Certify | Access remains required and appropriate |
| Revoke | Access is no longer required |
| Modify | Some access remains appropriate, but changes are required |
| Escalate | The reviewer lacks sufficient information or authority |
| Suspend | Access should be restricted while the issue is investigated |

Every certification must be based on current job responsibilities and business need.

### Step 6 — Remediation

IT processes approved revocation and modification decisions.

High-risk access must be prioritized, including:

- Privileged access
- Access belonging to inactive users
- Access to medical-delivery information
- Financial access
- Unapproved remote access
- Access with a segregation-of-duties conflict

### Step 7 — Remediation Verification

A designated reviewer verifies that:

- Revoked access was removed.
- Modified access matches the decision.
- Suspended access remains restricted.
- Escalated decisions received appropriate resolution.
- Exceptions were formally documented.

### Step 8 — Attestation and Closure

The System Owner attests that:

- The complete population was reviewed.
- Reviewers had appropriate context.
- Decisions were recorded.
- Remediation was completed or formally escalated.
- Evidence is complete.

---

## 6. Reviewer Guidance

Reviewers should consider:

- Is the person still active?
- Does the access support current duties?
- Is the level of access proportionate?
- Is privileged access necessary?
- Does the access conflict with another responsibility?
- Is the account being used?
- Does temporary access remain within its approved period?
- Does a contractor still have an active sponsor?
- Is an approved exception current?
- Would removal create an operational issue requiring escalation?

Reviewers must not certify access solely because it existed during the previous review.

---

## 7. Overdue Review Handling

| Condition | Required response |
| --- | --- |
| Review approaching due date | Automated or manual reminder |
| Review overdue by one business day | Escalate to reviewer’s manager |
| High-risk review overdue | Escalate to System Owner, Security, and GRC |
| Review repeatedly overdue | Document a control finding |
| Access has no accountable reviewer | Suspend or restrict based on risk |
| Revocation remains overdue | Escalate according to access sensitivity |

---

## 8. Evidence Requirements

The review package must include:

- Review scope
- Complete population
- Population-reconciliation record
- Reviewer assignments
- Reviewer instructions
- Decisions and justifications
- Reviewer timestamps
- Remediation tickets
- Verification results
- Escalations
- Approved exceptions
- Final System Owner attestation
- Completion summary

---

## 9. Failure Conditions

The workflow fails when:

- The population is incomplete.
- Inactive accounts are excluded.
- Reviewers lack sufficient access context.
- Users certify their own access.
- Decisions are missing.
- Reviewers rubber-stamp the population.
- Revocations are not completed.
- Remediation is not verified.
- Overdue reviews are not escalated.
- Evidence does not support the conclusion.
- The review closes with unresolved high-risk access.

---

## 10. Metrics

The workflow supports:

- `MET-004` — Access reviews completed on time
- `MET-005` — Overdue revocations
- `MET-007` — Privileged accounts with current approval
- `MET-008` — Evidence completeness
- `MET-009` — Control-test exception rate

Additional measures may include:

- Percentage of access certified
- Percentage of access revoked
- Percentage of access modified
- Number of orphaned accounts
- Number of inactive accounts
- Average remediation time
- Reviewer response rate
- Repeat access-review exceptions
