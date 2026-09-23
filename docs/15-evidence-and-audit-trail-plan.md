# Evidence and Audit Trail Plan

## Document Control

| Field | Value |
| --- | --- |
| Organization | Peachtree Logistics Group (fictional) |
| Project | From Framework to Workflow |
| Plan owner | GRC Analyst |
| Version | 1.0 |
| Status | Portfolio design artifact |

---

## 1. Purpose

This plan defines how PLG identifies, creates, collects, protects, reviews, retains, and disposes of IAM control evidence.

Evidence should allow a qualified reviewer to determine:

- What control activity occurred
- Who performed it
- Who approved it
- When it occurred
- Which person, account, system, or population was affected
- What decision was made
- Whether the control operated as designed
- Whether failures were identified and corrected

---

## 2. Evidence Principles

Evidence must be:

- Relevant
- Complete
- Accurate
- Timely
- Attributable
- Legible
- Protected
- Retrievable
- Traceable
- Appropriate for the assessment period

A screenshot alone may be insufficient when the control requires a complete population, approval history, timestamps, remediation, or system-generated logs.

---

## 3. Evidence Catalog

| Evidence ID | Evidence | Source | Custodian | Frequency | Related controls |
| --- | --- | --- | --- | --- | --- |
| `EVID-001` | Authoritative workforce event | HR system or approved HR record | HR Manager | Event-driven | `CTRL-001`, `CTRL-004` |
| `EVID-002` | Approved access request | Ticketing or workflow system | Department Manager | Event-driven | `CTRL-001`, `CTRL-002` |
| `EVID-003` | Provisioning record | System and ticket logs | IT Director | Event-driven | `CTRL-001`, `CTRL-003` |
| `EVID-004` | Segregation-of-duties result | Request workflow | System Owner | Per request and review | `CTRL-002` |
| `EVID-005` | Role and entitlement comparison | Role catalog and request record | System Owner | Per request and review | `CTRL-002` |
| `EVID-006` | Authentication and MFA record | Identity platform | Security Lead | Event-driven | `CTRL-009` |
| `EVID-007` | Disablement and revocation record | Identity, application, and ticket logs | IT Director | Event-driven | `CTRL-004` |
| `EVID-008` | Mover access-comparison record | Workflow or review record | Department Manager | Event-driven | `CTRL-004` |
| `EVID-009` | Privileged-activity review | Audit logs and review record | Security Lead | Monthly | `CTRL-006` |
| `EVID-010` | POA&M record | GRC repository | GRC Analyst | Monthly | `CTRL-007`, `CTRL-011` |
| `EVID-011` | Independent provisioning verification | Verification record | GRC or designated verifier | Event-driven | `CTRL-003` |
| `EVID-012` | Periodic access-review package | Review platform or controlled repository | System Owner | Quarterly or semiannually | `CTRL-005` |
| `EVID-013` | Exception and risk-acceptance record | GRC repository | GRC Analyst | Event-driven | `CTRL-007` |
| `EVID-014` | Control-test workpaper | Assessment repository | Assessor | Per assessment | `CTRL-010` |
| `EVID-015` | IAM control-health dashboard | Reporting platform | GRC Analyst | Monthly | `CTRL-011` |

---

## 4. Minimum Evidence Attributes

Each evidence record should identify:

- Evidence ID
- Related requirement
- Related risk
- Related control
- Related workflow
- System
- Transaction or population
- Control period
- Source
- Custodian
- Performer
- Approver
- Reviewer
- Creation date
- Collection date
- Review date
- Storage location
- Retention category
- Sensitivity
- Final status

---

## 5. Evidence Collection

Evidence may be collected through:

- System-generated reports
- Ticket exports
- Workflow history
- Approval records
- Configuration exports
- Audit logs
- Identity-platform reports
- HR event records
- Access-review reports
- Signed attestations
- Assessment workpapers
- Exception records
- POA&M reports

Manual evidence should identify who prepared it and how its accuracy was validated.

---

## 6. Evidence Quality Review

The reviewer should confirm:

1. The evidence covers the correct period.
2. The population is complete.
3. Required fields are present.
4. Approvals occurred before access was granted.
5. Timestamps are internally consistent.
6. The evidence came from an authoritative source.
7. The artifact has not been improperly altered.
8. Sensitive information is appropriately protected.
9. The evidence supports the stated conclusion.
10. Exceptions are visible and traceable.

---

## 7. Evidence Protection

Evidence repositories should use:

- Role-based access
- Least privilege
- MFA
- Change history
- Backup
- Integrity protection
- Access logging
- Periodic access review
- Secure transmission
- Approved disposal

Sensitive workforce, customer, financial, and medical-delivery information should be minimized or redacted when full detail is unnecessary.

---

## 8. Retention

Retention periods must be approved through PLG’s records-management, legal, contractual, privacy, and regulatory processes.

Until a formal schedule is approved:

- Evidence must not be deleted solely for convenience.
- Evidence owners must preserve records supporting open findings or investigations.
- Legal holds override routine disposal.
- Retention decisions must be documented.
- Portfolio samples must use fictional information only.

---

## 9. Evidence Traceability

Evidence should be traceable through the following chain:

> Requirement → Risk → Control → Workflow → Evidence → Test → Finding → Remediation

Evidence filenames or metadata should use the applicable evidence ID and control period.

---

## 10. Evidence Deficiencies

Evidence is deficient when it is:

- Missing
- Incomplete
- Untimely
- Unreadable
- Unattributable
- Unsupported
- Inconsistent with another authoritative source
- Altered without explanation
- Outside the assessment period
- Missing a required approval
- Missing the full population
- Unable to support the control conclusion

Material evidence deficiencies may result in a control finding.

---

## 11. Roles and Responsibilities

| Role | Responsibility |
| --- | --- |
| Control performer | Produces accurate evidence |
| Control owner | Ensures evidence requirements are met |
| Evidence custodian | Protects and retrieves evidence |
| GRC Analyst | Maintains the catalog and monitors completeness |
| Assessor | Evaluates evidence sufficiency |
| IT and Security | Preserve technical logs and reports |
| HR | Protects workforce-event evidence |
| Legal or records owner | Approves retention requirements |

---

## 12. Metrics

Evidence management supports:

- `MET-008` — Evidence completeness
- `MET-009` — Control-test exception rate

Additional measures include:

- Evidence collected on time
- Evidence rejected for quality
- Evidence missing required approval
- Evidence without an owner
- Average evidence-retrieval time
- Repeat evidence deficiencies
