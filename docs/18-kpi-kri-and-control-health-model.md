# KPI, KRI, and Control Health Model

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

This model defines how PLG measures IAM workflow performance, risk exposure, control effectiveness, and remediation progress.

The model distinguishes between:

- Key Performance Indicators
- Key Risk Indicators
- Control-effectiveness measures
- Operational service levels
- Escalation thresholds

---

## 2. Metric Types

| Type | Purpose |
| --- | --- |
| KPI | Measures whether a process meets its intended performance objective |
| KRI | Signals increasing exposure or likelihood of harm |
| Control metric | Measures whether a control operates as designed |
| SLA metric | Measures whether an activity is completed within the required time |
| Trend metric | Identifies improvement or deterioration over time |

---

## 3. Metric Catalog

| ID | Metric | Type | Target | Warning | Critical | Owner |
| --- | --- | --- | --- | --- | --- | --- |
| `MET-001` | Access requests completed within SLA | KPI | At least 95% | 90–94% | Below 90% | IT Director |
| `MET-002` | Requests with complete approval before provisioning | KPI | 100% | 98–99% | Below 98% | System Owners |
| `MET-003` | Termination access removed within required SLA | KPI/KRI | 100% | One late High-risk event | Any Critical account overdue | HR and IT |
| `MET-004` | Access reviews completed on time | KPI | At least 98% | 95–97% | Below 95% | System Owners |
| `MET-005` | Overdue revocations | KRI | Zero High-risk | One or two | Three or more, or any Critical | IT Director |
| `MET-006` | Active expired exceptions | KRI | Zero | One | Two or more | GRC Analyst |
| `MET-007` | Privileged accounts with current approval | KPI | 100% | 98–99% | Below 98% | Security Lead |
| `MET-008` | Required evidence complete and accepted | KPI | At least 98% | 95–97% | Below 95% | GRC Analyst |
| `MET-009` | Control-test exception rate | KRI | No more than 2% | More than 2–5% | More than 5% | GRC Analyst |
| `MET-010` | Temporary access removed by expiration | KPI | 100% | 98–99% | Below 98% | IT Director |
| `MET-011` | Active accounts matched to current workforce records | KPI | 100% | 99–99.9% | Below 99% | HR and IT |
| `MET-012` | POA&M items completed by target date | KPI | At least 90% | 80–89% | Below 80% | Corrective-action owners |

---

## 4. Metric Formulas

### `MET-001`

```text
Requests completed within SLA ÷ Total completed requests × 100
