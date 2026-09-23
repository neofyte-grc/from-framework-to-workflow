# Implementation Roadmap and POA&M

## Document Control

| Field | Value |
| --- | --- |
| Organization | Peachtree Logistics Group (fictional) |
| Project | From Framework to Workflow |
| Roadmap owner | CIO / IT Director |
| POA&M coordinator | GRC Analyst |
| Version | 1.0 |
| Status | Portfolio design artifact |

---

## 1. Purpose

This document sequences PLG’s proposed IAM improvements and establishes a POA&M-style process for tracking deficiencies through validated closure.

The roadmap prioritizes actions based on:

- Risk
- Operational dependency
- Implementation effort
- Resource availability
- Control relationships
- Evidence requirements

---

## 2. Implementation Principles

PLG should:

- Address Critical risks first.
- Establish ownership before automating.
- Standardize workflows before integrating systems.
- Build evidence into the workflow.
- Preserve operational continuity.
- Pilot high-impact changes.
- Validate control performance.
- Track unresolved deficiencies.
- Avoid closing actions without evidence.

---

## 3. Implementation Phases

### Phase 1 — Govern

**Objective:** Establish ownership and minimum IAM requirements.

**Key outputs:**

- Access Control Policy
- Identity Lifecycle Management Standard
- Stakeholder and RACI model
- Risk register
- System-owner assignments
- Initial role and entitlement catalog
- Approval matrix

### Phase 2 — Standardize

**Objective:** Create repeatable operational workflows.

**Key outputs:**

- Joiner-Mover-Leaver workflow
- Access request and approval workflow
- Provisioning and verification workflow
- Periodic access review workflow
- Privileged-access workflow
- Termination and emergency-revocation workflow
- Exception workflow

### Phase 3 — Evidence and Assess

**Objective:** Make control performance demonstrable.

**Key outputs:**

- Evidence catalog
- Evidence repository
- Control-test workpapers
- Access-review package
- Exception records
- Sample assessment
- Findings process

### Phase 4 — Automate

**Objective:** Reduce manual delay and error.

**Key outputs:**

- HR-to-IAM trigger
- Mover-access comparison
- Termination orchestration
- Review campaign generation
- Expiration monitoring
- SLA alerts
- Reconciliation reports
- Tested manual fallback

### Phase 5 — Monitor and Improve

**Objective:** Sustain control effectiveness.

**Key outputs:**

- KPI/KRI dashboard
- Control-health reporting
- Escalation process
- Quarterly governance review
- POA&M reporting
- Retesting
- Risk reassessment
- Continuous-improvement backlog

---

## 4. Proposed Roadmap

| Timeframe | Priority activities |
| --- | --- |
| Days 1–30 | Confirm ownership, approve minimum requirements, establish termination workflow, inventory privileged accounts |
| Days 31–60 | Create role catalogs, standardize requests, define SoD rules, launch evidence catalog |
| Days 61–90 | Implement periodic reviews, privileged-access controls, exception governance, and initial testing |
| Months 4–6 | Pilot automation, reconciliation, dashboards, and expanded system coverage |
| Months 7–12 | Mature monitoring, reduce standing privilege, validate controls, and close remaining findings |

The timeline is illustrative and would require stakeholder and resource validation.

---

## 5. POA&M Fields

Each POA&M item should include:

- POA&M ID
- Finding ID
- Finding source
- Affected risk
- Affected control
- Weakness description
- Severity
- Corrective action
- Owner
- Milestones
- Dependencies
- Resources
- Planned start
- Target completion
- Current status
- Residual risk
- Validation method
- Closure evidence
- Closure approval

---

## 6. Sample POA&M

| ID | Weakness | Risk | Corrective action | Owner | Target | Status |
| --- | --- | --- | --- | --- | --- | --- |
| `POAM-001` | Termination notification is inconsistent | High | Implement verified HR trigger and escalation timer | HR Manager | 30 days | Open |
| `POAM-002` | Role catalog is incomplete | High | Define approved roles and prohibited combinations | System Owners | 60 days | Open |
| `POAM-003` | Access reviews lack remediation verification | Moderate | Add closure validation and overdue reporting | GRC Analyst | 45 days | Open |
| `POAM-004` | Privileged accounts lack consistent expiration | High | Establish time-bound approval and monthly review | Security Lead | 60 days | Open |
| `POAM-005` | Contractor accounts lack consistent sponsors | High | Reconcile contractors and assign sponsors or revoke access | Vendor Manager | 30 days | Open |
| `POAM-006` | Evidence records are stored across multiple locations | Moderate | Establish controlled evidence repository and catalog | GRC Analyst | 60 days | Open |

---

## 7. Milestone Example

### `POAM-001` — Termination Notification

| Milestone | Owner | Target |
| --- | --- | --- |
| Define required HR event fields | HR Manager | Day 10 |
| Approve termination SLA | CIO and HR | Day 15 |
| Configure controlled notification workflow | IT Director | Day 20 |
| Test standard and emergency scenarios | GRC Analyst | Day 25 |
| Resolve test exceptions | Assigned owners | Day 28 |
| Approve production readiness | CIO | Day 30 |

---

## 8. Status Definitions

| Status | Meaning |
| --- | --- |
| Open | Corrective action has not started |
| In progress | Work is underway |
| At risk | Target date may be missed |
| Blocked | A dependency prevents progress |
| Pending validation | Implementation is complete but not validated |
| Closed | Corrective action has been validated |
| Risk accepted | Authorized owner accepted residual risk |
| Deferred | Authorized owner approved a revised schedule |

---

## 9. Closure Criteria

A POA&M item closes only when:

- Corrective action is implemented.
- Milestones are complete.
- Closure evidence is provided.
- The control is tested where appropriate.
- The underlying cause is addressed.
- Residual risk is documented.
- The assessor or GRC Analyst validates the result.
- The authorized owner approves closure.

Task completion alone does not prove that the control is effective.

---

## 10. Overdue Items

Overdue items require:

1. Updated status
2. Cause of delay
3. Current risk
4. Interim compensating controls
5. Revised milestones
6. New target date
7. Required approval
8. Escalation based on severity

Critical and High-risk items must not be silently extended.

---

## 11. Reporting

POA&M reports should include:

- Open items by severity
- Overdue items
- Items approaching due date
- Blocked items
- Repeat findings
- Average remediation age
- Items pending validation
- Closure rate
- Accepted residual risk
- Decisions required from leadership
