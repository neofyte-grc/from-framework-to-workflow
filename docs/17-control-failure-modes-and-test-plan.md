# Control Failure Modes and Test Plan

## Document Control

| Field | Value |
| --- | --- |
| Organization | Peachtree Logistics Group (fictional) |
| Project | From Framework to Workflow |
| Assessment coordinator | GRC Analyst |
| Version | 1.0 |
| Status | Portfolio design artifact |

---

## 1. Purpose

This document identifies how IAM controls could fail and defines procedures for evaluating control design and illustrative operating effectiveness.

The assessment approach uses:

- Examine
- Interview
- Test

This is a fictional portfolio assessment and not an independent audit.

---

## 2. Failure-Mode Analysis

| Failure mode | Likely cause | Potential impact | Detection method |
| --- | --- | --- | --- |
| Account lacks approval | Workflow bypass or incomplete ticket | Unauthorized access | Account-to-request comparison |
| Wrong user receives access | Identity-selection error | Data exposure or disruption | Independent verification |
| Access exceeds approval | Provisioning error | Excessive privilege | Approval-to-entitlement comparison |
| SoD conflict is missed | Incomplete rules or manual review | Fraud or undetected error | Conflict analysis |
| Termination is delayed | Late notification or queue failure | Former-user access | HR-to-account reconciliation |
| Mover retains old access | Addition without removal analysis | Privilege accumulation | Current-versus-target review |
| Access review is incomplete | Incomplete population | Inappropriate access persists | Population reconciliation |
| Reviewer rubber-stamps access | Insufficient context or time | Invalid certification | Decision-pattern and sample review |
| Privileged access lacks MFA | Configuration or exception failure | Administrative compromise | Configuration review |
| Temporary access does not expire | Missing date or failed automation | Persistent unauthorized access | Expiration report |
| Exception remains active | Weak monitoring | Unaccepted residual risk | Exception-aging review |
| Evidence is incomplete | Manual collection failure | Control cannot be demonstrated | Evidence quality review |
| Finding closes without validation | Schedule pressure | Unresolved weakness | Closure-evidence review |

---

## 3. Assessment Objectives

The assessment will determine whether controls:

- Are clearly defined
- Address identified risks
- Have accountable owners
- Include appropriate approval
- Operate at the required frequency
- Produce sufficient evidence
- Detect and correct failures
- Escalate material exceptions
- Support reliable metrics
- Remain aligned with operational reality

---

## 4. Test Procedures

### `TEST-001` — Account Authorization

| Attribute | Definition |
| --- | --- |
| Control | `CTRL-001` |
| Objective | Determine whether created accounts had complete prior authorization |
| Population | Accounts created during the assessment period |
| Procedure | Select a risk-based sample and compare accounts with HR events, requests, and approvals |
| Expected result | Every account has a verified identity, manager, business need, and approval |
| Evidence | `EVID-001`, `EVID-002`, `EVID-003` |

### `TEST-002` — Provisioning Accuracy

| Attribute | Definition |
| --- | --- |
| Control | `CTRL-003` |
| Objective | Determine whether assigned access matches approved access |
| Population | Access transactions completed during the period |
| Procedure | Compare approved role and entitlement with actual system access |
| Expected result | No unexplained difference exists |
| Evidence | `EVID-002`, `EVID-003`, `EVID-011` |

### `TEST-003` — Termination Timeliness

| Attribute | Definition |
| --- | --- |
| Control | `CTRL-004` |
| Objective | Determine whether terminated-user access was removed within SLA |
| Population | Terminations during the period |
| Procedure | Compare effective separation time with disablement and session-revocation timestamps |
| Expected result | Access was removed within SLA or appropriately escalated |
| Evidence | `EVID-001`, `EVID-007` |

### `TEST-004` — Mover Access Adjustment

| Attribute | Definition |
| --- | --- |
| Control | `CTRL-004` |
| Objective | Determine whether obsolete access was removed following transfer |
| Population | Role and department changes |
| Procedure | Compare prior access, target role, approved additions, and completed removals |
| Expected result | Obsolete access is removed and new access is authorized |
| Evidence | `EVID-005`, `EVID-008` |

### `TEST-005` — Periodic Access Review

| Attribute | Definition |
| --- | --- |
| Control | `CTRL-005` |
| Objective | Determine whether the review used a complete population and verified remediation |
| Population | In-scope accounts and entitlements |
| Procedure | Examine population, reconciliation, decisions, remediation, verification, and attestation |
| Expected result | All access is reviewed and required remediation is verified |
| Evidence | `EVID-012` |

### `TEST-006` — Privileged Access

| Attribute | Definition |
| --- | --- |
| Control | `CTRL-006` |
| Objective | Determine whether privileged access is approved, protected, monitored, and current |
| Population | Privileged accounts |
| Procedure | Examine approvals, MFA, expiration, logging, use, and periodic review |
| Expected result | Every privileged account meets defined requirements |
| Evidence | `EVID-006`, `EVID-009` |

### `TEST-007` — Exception Governance

| Attribute | Definition |
| --- | --- |
| Control | `CTRL-007` |
| Objective | Determine whether exceptions are authorized and time-bound |
| Population | Active and recently closed exceptions |
| Procedure | Examine risk assessment, approval, compensation, monitoring, expiration, and closure |
| Expected result | Every exception satisfies the workflow requirements |
| Evidence | `EVID-013` |

### `TEST-008` — Evidence Completeness

| Attribute | Definition |
| --- | --- |
| Control | `CTRL-010` |
| Objective | Determine whether required evidence supports control conclusions |
| Population | Evidence records collected during the period |
| Procedure | Evaluate required attributes, sources, protection, and traceability |
| Expected result | Evidence is sufficient, reliable, and retrievable |
| Evidence | Evidence catalog and selected records |

---

## 5. Sampling Approach

Sample size should consider:

- Population size
- Control frequency
- Risk level
- Prior findings
- Degree of automation
- Number of locations
- Number of systems
- Workforce type
- Privilege level
- Known exceptions

High-risk and unusual transactions should be included deliberately.

---

## 6. Exception Severity

| Severity | Description |
| --- | --- |
| Critical | Immediate material exposure or complete control failure |
| High | Significant weakness affecting sensitive or privileged access |
| Moderate | Control weakness with meaningful but limited exposure |
| Low | Isolated documentation or minor process issue |

Severity should consider:

- Access sensitivity
- Privilege
- Duration
- Population affected
- Repeat occurrence
- Detectability
- Existing compensating controls
- Actual or potential impact

---

## 7. Finding Requirements

Each finding should include:

- Finding ID
- Condition
- Criteria
- Cause
- Effect or risk
- Affected control
- Affected population
- Evidence
- Severity
- Recommendation
- Corrective-action owner
- Target date
- Required validation

---

## 8. Retesting

A finding may close only after:

- Corrective action is implemented.
- Closure evidence is provided.
- The assessor evaluates the evidence.
- The control is retested where appropriate.
- Residual risk is documented.
- The authorized role approves closure.

---

## 9. Assessment Limitations

A real assessment would require:

- Complete populations
- Direct system access
- Stakeholder interviews
- Configuration evidence
- Reliable system logs
- Defined assessment period
- Approved sampling method
- Sufficient assessor independence
- Validated findings and management responses
