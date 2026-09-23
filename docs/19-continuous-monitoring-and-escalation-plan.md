# Continuous Monitoring and Escalation Plan

## Document Control

| Field | Value |
| --- | --- |
| Organization | Peachtree Logistics Group (fictional) |
| Project | From Framework to Workflow |
| Plan owner | GRC Analyst |
| Executive owner | CIO / IT Director |
| Version | 1.0 |
| Status | Portfolio design artifact |

---

## 1. Purpose

This plan defines how PLG monitors IAM control performance, identifies changes in risk, escalates control failures, and drives corrective action.

Continuous monitoring is intended to provide leadership with timely information about:

- Control health
- Access risk
- SLA performance
- Exceptions
- Findings
- Remediation
- Material changes
- Emerging failure patterns

---

## 2. Monitoring Objectives

PLG’s monitoring process should:

- Detect overdue access actions.
- Identify inactive or orphaned accounts.
- Monitor privileged access.
- Identify expired temporary access.
- Identify expired exceptions.
- Track access-review completion.
- Evaluate evidence quality.
- Monitor corrective-action progress.
- Detect recurring failures.
- Escalate material risk.
- Trigger control reassessment after change.

---

## 3. Monitoring Cadence

| Cadence | Activity | Owner |
| --- | --- | --- |
| Daily | Failed terminations, Critical revocations, integration failures, and security alerts | IT and Security |
| Weekly | Provisioning backlog, SLA breaches, discrepancies, and unresolved tickets | IT Director |
| Monthly | Privileged access, exceptions, findings, evidence, and control-health dashboard | Security and GRC |
| Quarterly | Access reviews, risk register, trend analysis, and executive reporting | System Owners and GRC |
| Semiannual | Standard-access recertification and process review | System Owners |
| Annual | Full control assessment and document review | GRC and control owners |
| Event-driven | Incident, system change, organizational change, or material failure | Assigned owner |

---

## 4. Monitoring Sources

Monitoring uses:

- HR workforce reports
- Account inventories
- Entitlement reports
- Ticket reports
- Access-review results
- Privileged-access logs
- Authentication logs
- Exception records
- Assessment findings
- POA&M reports
- Incident records
- Vendor notifications
- Metric dashboards
- Change-management records

---

## 5. Escalation Levels

| Level | Condition | Response |
| --- | --- | --- |
| Level 1 | Low-impact isolated issue | Process owner corrects and documents |
| Level 2 | SLA breach or recurring Moderate issue | Manager and GRC perform root-cause review |
| Level 3 | High-risk access or material control failure | CIO and Security Lead direct remediation |
| Level 4 | Critical exposure, suspected misuse, or executive risk decision | COO and incident leadership engage immediately |

---

## 6. Escalation Triggers

Immediate or accelerated escalation is required when:

- A terminated user’s privileged account remains active.
- Unauthorized administrative access is identified.
- A Critical system cannot remove access.
- A suspected compromised account remains enabled.
- A required audit log is unavailable.
- A material access-review population is incomplete.
- A High-risk exception expires.
- Repeated failures suggest a systemic weakness.
- A POA&M item involving Critical risk becomes overdue.
- Evidence cannot support a material control conclusion.

---

## 7. Escalation Workflow

1. Detect and validate the condition.
2. Contain immediate exposure where authorized.
3. Notify the process owner.
4. Determine the affected risk, control, system, and population.
5. Assign severity.
6. Notify the required escalation authority.
7. Create a corrective action or incident record.
8. Establish an owner and target date.
9. Monitor progress.
10. Validate resolution.
11. Update risk, metrics, and documentation.
12. Communicate closure.

---

## 8. Material-Change Triggers

Control reassessment is required following:

- New business system
- Major system upgrade
- New logistics service
- Merger or acquisition
- Significant workforce growth
- New contractor model
- New sensitive-data use
- Material vendor change
- Major incident
- Repeated control failure
- Framework or legal change
- Change in authentication technology
- Change in remote-access architecture

---

## 9. Root-Cause Categories

Root-cause analysis may classify issues as:

- People
- Process
- Technology
- Data
- Training
- Governance
- Ownership
- Capacity
- Vendor dependency
- Automation failure
- Documentation
- Change management

Corrective actions should address the underlying cause rather than only the immediate symptom.

---

## 10. Reporting Requirements

Monitoring reports should identify:

- Reporting period
- Data source
- Metric or event
- Threshold
- Trend
- Affected risk
- Affected control
- Affected system
- Accountable owner
- Current action
- Target date
- Escalation status
- Decision required

---

## 11. Improvement Triggers

A workflow or control should be redesigned when:

- The same failure repeatedly occurs.
- Metrics remain Amber or Red.
- Evidence cannot support assessment.
- Operational staff consistently bypass the workflow.
- System changes invalidate the control.
- Manual work creates unacceptable delay.
- Control cost materially exceeds value.
- Users cannot understand their responsibilities.
- A compensating control becomes permanent.
- Risk exceeds the organization’s tolerance.

---

## 12. Evidence Requirements

Continuous-monitoring evidence includes:

- Dashboards
- Threshold alerts
- Review meeting records
- Escalation notifications
- Root-cause analyses
- Corrective-action plans
- POA&M updates
- Retest results
- Risk-register updates
- Closure approvals
