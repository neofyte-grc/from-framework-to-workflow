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
```

### `MET-002`

```text
Requests provisioned only after complete approval ÷ Total provisioned requests × 100
```

### `MET-003`

```text
Terminations completed within the applicable removal SLA ÷ Total termination events × 100
```

Any overdue Critical account is reported separately because a percentage can conceal a severe individual failure.

### `MET-004`

```text
Access reviews completed by the due date ÷ Total scheduled access reviews × 100
```

### `MET-005`

```text
Count of approved revocation decisions not completed by their required deadline
```

### `MET-006`

```text
Count of active exceptions whose approved expiration date has passed
```

### `MET-007`

```text
Privileged accounts with current approval ÷ Total active privileged accounts × 100
```

### `MET-008`

```text
Evidence items accepted as complete and relevant ÷ Total evidence items required × 100
```

### `MET-009`

```text
Tested items with one or more exceptions ÷ Total tested items × 100
```

### `MET-010`

```text
Temporary access grants removed by expiration ÷ Total expired temporary access grants × 100
```

### `MET-011`

```text
Active accounts matched to a current workforce or approved sponsor record ÷ Total active accounts × 100
```

### `MET-012`

```text
POA&M items completed by target date ÷ Total POA&M items due during the period × 100
```

---

## 5. Data Sources

| Source | Primary Metrics | Validation Expectation |
| --- | --- | --- |
| Service-management platform | `MET-001`, `MET-002`, `MET-003`, `MET-010` | Required fields, timestamps, approvals, and closure states are complete |
| HR and contractor records | `MET-003`, `MET-011` | Population reconciles to active and separated personnel records |
| Identity directory and application inventories | `MET-005`, `MET-007`, `MET-011` | Accounts are unique, active-state logic is defined, and ownership is known |
| Access-review platform or certification records | `MET-004`, `MET-005` | Campaign scope, decisions, due dates, and remediation are preserved |
| Exception register | `MET-006`, `MET-010` | Approval and expiration fields are mandatory and monitored |
| Evidence repository | `MET-008` | Evidence acceptance criteria and review outcomes are recorded |
| Assessment workpapers | `MET-009` | Population, sample, procedures, results, and exceptions are documented |
| POA&M register | `MET-012` | Owners, milestones, due dates, status, validation, and closure are current |

---

## 6. Control-Health Rating

Each control receives an overall health rating based on metric status, known exceptions, evidence quality, open findings, and remediation progress.

| Rating | Meaning | Required Action |
| --- | --- | --- |
| Green | Target achieved; no material unresolved issue | Continue routine monitoring |
| Amber | Warning threshold reached or a manageable exception exists | Assign corrective action and monitor more frequently |
| Red | Critical threshold reached, a material control failure exists, or evidence is unreliable | Escalate, apply interim safeguards, and track remediation |
| Gray | Insufficient reliable data to determine health | Correct the data or evidence gap; do not assume effectiveness |

The overall rating follows the most significant supported condition. A favorable average must not override an overdue Critical revocation, expired exception, unsupported privileged account, or other material event.

---

## 7. Reporting Cadence

| Activity | Cadence | Owner | Audience |
| --- | --- | --- | --- |
| Operational metric review | Weekly | IT Director and process owners | Control performers and System Owners |
| IAM control-health dashboard | Monthly | GRC Analyst | CIO, IT Director, Security Lead, HR Manager |
| Risk and trend review | Quarterly | GRC Analyst | Governance stakeholders and risk owners |
| Material threshold escalation | Event-driven | Metric owner | Accountable executive and affected control owners |
| Metric-definition review | Annually or after material change | GRC Analyst | CIO and control owners |

---

## 8. Escalation Rules

1. A red result is escalated according to the continuous-monitoring plan.
2. An overdue Critical termination or privileged-access issue receives immediate attention regardless of the monthly reporting cycle.
3. Two consecutive amber periods require a documented corrective action.
4. A gray rating lasting more than one reporting cycle becomes an evidence or data-quality finding.
5. Repeated exceptions are evaluated for systemic root cause rather than treated as isolated transactions.
6. Open corrective actions are linked to the applicable finding and POA&M identifier.

---

## 9. Metric Governance

Metric owners must document:

- Business definition and intended decision use
- Numerator, denominator, exclusions, and time window
- Source systems and extraction logic
- Data-quality checks and reconciliation method
- Target, warning, and critical thresholds
- Reporting frequency and accountable recipient
- Corrective-action and escalation expectations
- Definition changes and effective dates

Thresholds should be reevaluated when PLG changes systems, workforce models, risk appetite, contractual obligations, or control design.

---

## 10. Interpretation Limitations

Metrics are indicators, not standalone proof of control effectiveness. High completion percentages may hide material individual failures, and low exception counts may reflect incomplete detection. Management should interpret results alongside evidence quality, risk severity, test results, population completeness, trends, and known limitations.

---

## 11. Portfolio Disclaimer

PLG, its measurements, thresholds, results, systems, and control-health determinations are fictional. This model demonstrates GRC measurement design and does not represent production monitoring, independent assurance, or a compliance determination.
