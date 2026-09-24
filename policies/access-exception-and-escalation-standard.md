# Access Exception and Escalation Standard

## Document Control

| Field | Value |
| --- | --- |
| Organization | Peachtree Logistics Group (fictional) |
| Standard owner | GRC Analyst |
| Executive owner | CIO / IT Director |
| Version | 1.0 |
| Status | Portfolio design artifact |
| Review frequency | Annually and following material change |

---

## 1. Purpose

This standard defines how PLG evaluates, approves, monitors, escalates, renews, and closes exceptions to IAM requirements.

It also establishes escalation requirements for control failures, overdue actions, unauthorized access, and unresolved risk.

---

## 2. Scope

This standard applies to:

- Access-control exceptions
- Technical limitations
- Temporary operational workarounds
- Segregation-of-duties conflicts
- Shared accounts
- Standing privileged access
- Delayed remediation
- Vendor limitations
- Expired access
- Control failures
- Evidence deficiencies
- Overdue access reviews
- Failed revocation

---

## 3. Exception Principles

Every exception must be:

- Necessary
- Specific
- Risk-assessed
- Approved
- Time-bound
- Supported by compensating controls
- Monitored
- Traceable
- Connected to corrective action
- Closed or reassessed before expiration

An exception is temporary risk treatment, not permanent permission to ignore a requirement.

---

## 4. Eligibility

An exception may be considered when:

- A technical limitation prevents compliance.
- A vendor platform lacks required functionality.
- A temporary operational dependency exists.
- Immediate remediation would create disproportionate harm.
- A remediation project is underway.
- No safer practical alternative is available.

---

## 5. Prohibited Uses

Exceptions must not:

- Avoid routine work.
- Conceal a control failure.
- Eliminate accountability.
- Authorize illegal activity.
- Remain open indefinitely.
- Be approved by the requester.
- Automatically renew.
- Replace a corrective-action plan.
- Continue after expiration without authorization.

---

## 6. Required Exception Information

An exception request must include:

- Exception ID
- Requester
- Business owner
- Risk owner
- Unmet requirement
- Affected systems
- Affected users
- Affected information
- Business justification
- Alternatives considered
- Risk statement
- Likelihood
- Impact
- Inherent risk
- Compensating controls
- Residual risk
- Monitoring
- Start date
- Expiration date
- Corrective action
- Requested approver

---

## 7. Approval Authority

| Residual risk | Minimum approval |
| --- | --- |
| Low | System Owner |
| Moderate | System Owner within delegated authority |
| High | CIO / IT Director and Information Security Lead |
| Critical | COO or designated executive risk authority |

Approval authority may not be delegated below the documented risk level.

---

## 8. Maximum Initial Duration

| Residual risk | Maximum initial duration |
| --- | --- |
| Low | 12 months |
| Moderate | 6 months |
| High | 90 days |
| Critical | 30 days unless executive authority documents otherwise |

Shorter durations should be used whenever practical.

---

## 9. Compensating Controls

Compensating controls must:

- Address the same risk as the unmet requirement.
- Be enforceable.
- Have an accountable owner.
- Operate throughout the exception period.
- Produce evidence.
- Be monitored.
- Be tested where appropriate.
- Reduce residual risk to an accepted level.

Examples include:

- Enhanced logging
- More frequent review
- Secondary approval
- Read-only access
- Restricted location
- Limited duration
- Manual reconciliation
- Additional supervision
- Network restriction
- Increased alerting

---

## 10. Monitoring

GRC must monitor:

- Active exceptions
- Approaching expirations
- Expired exceptions
- Compensating-control performance
- Corrective-action progress
- Changes in affected scope
- Changes in risk
- Repeat exceptions
- Renewal requests

---

## 11. Renewal

Renewal requires:

- A new review
- Updated business justification
- Updated risk assessment
- Updated alternatives analysis
- Validation of compensating controls
- Corrective-action status
- New expiration date
- Approval at the required authority

Renewal is not automatic.

---

## 12. Closure

An exception may close when:

- The requirement is implemented.
- The affected access is removed.
- The activity ends.
- A permanent approved control replaces the temporary control.
- The risk no longer exists.

Closure requires evidence and risk-owner acknowledgement.

---

## 13. Escalation Levels

| Level | Condition | Required response |
| --- | --- | --- |
| Level 1 | Low-impact isolated issue | Process owner corrects and documents |
| Level 2 | SLA breach or recurring Moderate issue | Manager and GRC perform root-cause review |
| Level 3 | High-risk access or material control failure | CIO and Security Lead direct remediation |
| Level 4 | Critical exposure or suspected misuse | COO and incident leadership engage immediately |

---

## 14. Immediate Escalation Events

Immediate escalation is required when:

- A terminated user’s privileged account remains active.
- Unauthorized privileged access is detected.
- Emergency revocation fails.
- A compromised identity remains enabled.
- A Critical exception expires.
- A material logging failure prevents accountability.
- A user bypasses a revoked restriction.
- A High-risk finding becomes materially overdue.
- Evidence suggests account misuse.
- An unauthorized account cannot be attributed.

---

## 15. Escalation Procedure

1. Detect and validate the condition.
2. Contain exposure when authorized.
3. Notify the process owner.
4. Identify the affected risk and control.
5. Assign severity.
6. Notify the required authority.
7. Create an incident, finding, exception, or POA&M item.
8. Assign an owner.
9. Establish a target date.
10. Monitor corrective action.
11. Validate resolution.
12. Document closure.

---

## 16. Evidence Requirements

Exception and escalation evidence includes:

- Request
- Risk assessment
- Alternatives
- Compensating controls
- Approval
- Conditions
- Expiration
- Monitoring
- Corrective action
- Escalation notices
- Decisions
- Validation
- Closure

---

## 17. Metrics

PLG should monitor:

- Active exceptions
- Exceptions by risk
- Average exception age
- Exceptions approaching expiration
- Expired exceptions
- Repeat exceptions
- Exceptions with incomplete evidence
- Escalation response time
- Overdue corrective actions
- Time to close Critical issues

---

## 18. Disclaimer

PLG and this standard are fictional. This document is an educational portfolio artifact and does not represent legal advice, formal risk acceptance, or production implementation.
