# Access Exception and Risk Acceptance Workflow

## Document Control

| Field | Value |
| --- | --- |
| Organization | Peachtree Logistics Group (fictional) |
| Workflow ID | `WF-007` |
| Workflow coordinator | GRC Analyst |
| Version | 1.0 |
| Status | Portfolio design artifact |

---

## 1. Purpose

This workflow governs temporary deviations from PLG’s IAM requirements.

It prevents operational workarounds from becoming:

- Undocumented
- Unapproved
- Permanent
- Unmonitored
- Unsupported by compensating controls
- Accepted by someone without authority

An approved exception does not mean that a control is unnecessary. It means that an authorized risk owner has temporarily accepted defined residual risk under documented conditions.

---

## 2. Exception Eligibility

An exception may be considered when:

- A technical limitation prevents compliance.
- A vendor platform lacks a required capability.
- A documented operational dependency exists.
- A temporary business need cannot be met through the standard process.
- Immediate implementation would cause disproportionate operational harm.
- A remediation project is underway.
- A safer practical alternative is unavailable.

---

## 3. Prohibited Exceptions

An exception may not be used to:

- Avoid routine work
- Eliminate accountability
- Conceal a control failure
- Bypass approval because of inconvenience
- Authorize known illegal activity
- Remain open indefinitely
- Permit self-approval
- Replace a permanent corrective-action plan
- Continue after expiration without reassessment

---

## 4. Required Exception Information

Each request must include:

- Exception ID
- Requester
- Business owner
- Risk owner
- Unmet requirement
- Affected system
- Affected users
- Affected information
- Business justification
- Reason the normal requirement cannot be met
- Alternatives considered
- Risk statement
- Likelihood
- Impact
- Inherent-risk score
- Compensating controls
- Residual-risk score
- Monitoring requirements
- Requested start date
- Requested expiration date
- Corrective-action plan
- Approval authority

---

## 5. Workflow

### Step 1 — Submission

The requester documents the proposed deviation and business need.

### Step 2 — Completeness Review

GRC confirms that:

- The unmet requirement is identified.
- The affected scope is clear.
- The requested duration is defined.
- The accountable business and risk owners are identified.
- Alternatives have been considered.

### Step 3 — Risk Assessment

GRC and Security evaluate:

- Threat or failure scenario
- Data sensitivity
- Privilege level
- Number of affected users
- Duration
- Operational impact
- Existing controls
- Potential misuse
- Detection capability
- Recovery capability

### Step 4 — Alternative Evaluation

The reviewers consider whether the risk can be reduced through:

- Narrower permissions
- Read-only access
- Shorter duration
- Additional approval
- Enhanced logging
- Manual reconciliation
- Increased review frequency
- Temporary isolation
- Alternative technology
- Delayed implementation

### Step 5 — Compensating Controls

Compensating controls must:

- Address the same risk as the unmet requirement.
- Be practical and enforceable.
- Have an accountable owner.
- Produce evidence.
- Operate for the entire exception period.
- Be monitored and tested where appropriate.

### Step 6 — Approval

The authorized risk owner:

- Approves
- Approves with conditions
- Requests modification
- Rejects

### Step 7 — Implementation and Monitoring

Approved conditions and compensating controls are implemented before the exception becomes active.

GRC monitors:

- Control operation
- Changes in risk
- Corrective-action progress
- Evidence completeness
- Expiration

### Step 8 — Closure or Renewal

Before expiration, the exception must be:

- Closed because the requirement is satisfied
- Closed because the access or activity ended
- Reassessed and renewed through a new approval
- Escalated because remediation remains incomplete

Renewal is not automatic.

---

## 6. Approval Authority

| Residual-risk level | Minimum approval |
| --- | --- |
| Low | System Owner |
| Moderate | System Owner within delegated authority |
| High | CIO / IT Director and Security Lead |
| Critical | COO or designated executive risk authority |

The requester may not approve their own exception.

---

## 7. Maximum Duration

| Risk level | Maximum initial duration |
| --- | --- |
| Low | 12 months |
| Moderate | 6 months |
| High | 90 days |
| Critical | 30 days unless executive authority documents otherwise |

Shorter periods should be used whenever practical.

---

## 8. Expired Exceptions

When an exception expires:

- The exception is no longer authorized.
- Related access must be removed or restricted.
- The unmet requirement must be implemented.
- A new exception must complete the full review process.
- Continued unauthorized activity must be escalated.
- Material exposure may become a formal finding.

---

## 9. Evidence Requirements

The evidence package includes:

- Completed request
- Unmet requirement
- Risk assessment
- Alternatives considered
- Compensating controls
- Residual-risk determination
- Approval
- Conditions
- Start and expiration dates
- Monitoring results
- Corrective-action status
- Closure or renewal decision

---

## 10. Failure Conditions

The workflow fails when:

- An exception is undocumented.
- The requester self-approves.
- The risk owner lacks authority.
- Compensating controls are missing.
- No expiration date exists.
- Monitoring does not occur.
- The exception continues after expiration.
- Renewal occurs without reassessment.
- Corrective action is not tracked.
- Evidence is insufficient.

---

## 11. Metrics

The workflow supports:

- `MET-006` — Number of active expired exceptions
- `MET-008` — Evidence completeness
- `MET-009` — Control-test exception rate

Additional measures include:

- Number of active exceptions
- Average exception age
- Exceptions by risk level
- Exceptions approaching expiration
- Percentage with complete compensating-control evidence
- Number of renewed exceptions
- Repeat exceptions involving the same requirement
