# Access Management Risk Register

## Document Control

| Field | Value |
| --- | --- |
| Organization | Peachtree Logistics Group (fictional) |
| Project | From Framework to Workflow |
| Risk owner | CIO / IT Director |
| Risk coordinator | GRC Analyst |
| Version | 1.0 |
| Status | Portfolio design artifact |

---

## 1. Purpose

This register documents access-management risks affecting PLG’s people, processes, technology, data, facilities, and third-party relationships.

The register connects each risk to:

- Causes
- Potential events
- Business impacts
- Inherent-risk scores
- Control treatments
- Responsible owners
- Target residual-risk scores

---

## 2. Risk-Scoring Method

```text
Risk score = Likelihood × Impact
```

| Score | Rating | Treatment Expectation |
| ---: | --- | --- |
| 1–4 | Low | Monitor or accept with owner approval |
| 5–9 | Moderate | Define treatment and track progress |
| 10–16 | High | Prioritize treatment and management reporting |
| 17–25 | Critical | Escalate and apply immediate risk-reduction measures |

---

## 3. Risk Register

| ID | Risk Event | Primary Cause | Business Impact | Inherent L | Inherent I | Inherent Score | Primary Treatment | Owner | Target Residual Score |
| --- | --- | --- | --- | ---: | ---: | ---: | --- | --- | ---: |
| `IAM-RISK-001` | Accounts are created, changed, or retained without an authorized lifecycle event | Disconnected HR, sponsor, and IT processes | Unauthorized access, data exposure, and inaccurate account inventory | 4 | 4 | 16 High | `CTRL-001`, `WF-001` | IT Director | 6 Moderate |
| `IAM-RISK-002` | Users receive excessive or inaccurate permissions | Informal role design and incomplete least-privilege review | Unauthorized transactions, data exposure, and operational error | 4 | 4 | 16 High | `CTRL-002`, `CTRL-003`, `WF-002`, `WF-003` | System Owners | 6 Moderate |
| `IAM-RISK-003` | Incompatible duties are assigned to one individual | Missing conflict rules or approval challenge | Fraud, concealed error, and unreviewed high-impact activity | 3 | 5 | 15 High | `CTRL-002`, `WF-002` | CIO | 5 Moderate |
| `IAM-RISK-004` | Weak authentication, unmanaged remote access, or temporary access exposes PLG systems | Inconsistent MFA, device, and exception controls | Account compromise and unauthorized remote activity | 4 | 5 | 20 Critical | `CTRL-007`, `CTRL-009`, `WF-003`, `WF-007` | Security Lead | 8 Moderate |
| `IAM-RISK-005` | Former personnel or vendors retain access after separation | Late notice, incomplete system inventory, or failed handoff | Unauthorized activity, privacy exposure, and disruption | 4 | 5 | 20 Critical | `CTRL-004`, `WF-006` | HR Manager and IT Director | 5 Moderate |
| `IAM-RISK-006` | Transferred personnel retain access from prior responsibilities | Mover events treated as administrative changes only | Access accumulation and segregation-of-duties conflict | 4 | 4 | 16 High | `CTRL-001`, `CTRL-004`, `WF-001` | Department Managers | 6 Moderate |
| `IAM-RISK-007` | Privileged activity is unauthorized, unmonitored, or insufficiently attributable | Standing elevation, shared administration, or incomplete logging | System compromise, record alteration, and weak accountability | 3 | 5 | 15 High | `CTRL-006`, `WF-005` | Security Lead | 5 Moderate |
| `IAM-RISK-008` | IAM controls fail without timely detection, testing, or remediation | Fragmented governance, incomplete evidence, or overdue corrective action | Repeated control failure and unsupported assurance claims | 4 | 4 | 16 High | `CTRL-007`, `CTRL-008`, `CTRL-010`, `CTRL-011` | CIO and GRC Analyst | 6 Moderate |
| `IAM-RISK-009` | Shared, orphaned, duplicate, or service accounts cannot be tied to an accountable owner | Weak inventory, naming, ownership, and recertification practices | Loss of accountability and persistent unauthorized access | 3 | 4 | 12 High | `CTRL-001`, `CTRL-005`, `CTRL-009` | IT Director | 4 Low |
| `IAM-RISK-010` | Third-party access remains broader or longer than the approved business need | Sponsor turnover, vendor-managed platforms, or incomplete offboarding | External unauthorized access and contractual or privacy exposure | 4 | 4 | 16 High | `CTRL-001`, `CTRL-004`, `CTRL-007`, `WF-006`, `WF-007` | Vendor Sponsor | 6 Moderate |

---

## 4. Treatment Priorities

### Priority 1 — Termination and Third-Party Access

PLG should first reduce `IAM-RISK-005` and `IAM-RISK-010` by establishing authoritative termination events, complete access inventories, urgent disablement SLAs, vendor-platform confirmation, independent verification, and escalation for unresolved access.

### Priority 2 — Authentication and Privileged Access

PLG should reduce `IAM-RISK-004` and `IAM-RISK-007` through MFA, unique identities, controlled privileged elevation, current approval, session accountability, logging, and recurring review.

### Priority 3 — Least Privilege and Movers

PLG should reduce `IAM-RISK-002`, `IAM-RISK-003`, and `IAM-RISK-006` through role definitions, conflict checks, manager and System Owner approval, independent provisioning verification, and removal of access no longer required after transfers.

### Priority 4 — Governance and Detectability

PLG should reduce `IAM-RISK-001`, `IAM-RISK-008`, and `IAM-RISK-009` through policy ownership, complete account inventories, periodic certification, evidence-quality review, control testing, metrics, escalation, and POA&M tracking.

---

## 5. Risk Response Rules

| Rating | Response Rule |
| --- | --- |
| Critical | Notify accountable leadership promptly, apply interim safeguards, and track a formal treatment plan |
| High | Assign an owner, corrective actions, milestones, evidence requirements, and a target date |
| Moderate | Treat or formally accept based on cost, operational need, and compensating controls |
| Low | Monitor through routine control and review cycles |

Risk acceptance must be documented through `WF-007`. Acceptance does not remove the requirement to monitor expiration dates, compensating controls, or changes in exposure.

---

## 6. Monitoring Indicators

The risk register is monitored through the metric catalog, including:

- `MET-003` — Termination access removed within required SLA
- `MET-005` — Overdue revocations
- `MET-006` — Active expired exceptions
- `MET-007` — Privileged accounts with current approval
- `MET-009` — Control-test exception rate
- `MET-011` — Active accounts matched to current workforce records
- `MET-012` — POA&M items completed by target date

The GRC Analyst reviews the register quarterly and after material incidents, system changes, audit findings, acquisitions, major vendor changes, or significant workforce-process changes.

---

## 7. Residual-Risk Decision

Residual scores are targets based on the proposed control design. They are not claims of achieved effectiveness. A risk owner may approve residual risk only after reviewing implementation evidence, known exceptions, test results, dependencies, and treatment progress.

---

## 8. Portfolio Disclaimer

PLG, its risk events, scores, owners, control performance, and treatment decisions are fictional. This register demonstrates risk-analysis and control-design methods and is not a production risk assessment or legal compliance determination.
