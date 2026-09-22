# Current-State and Future-State Analysis

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

This document compares PLG’s assumed current IAM practices with the proposed target operating model.

The analysis identifies:

- Process gaps
- Ownership gaps
- Evidence gaps
- Technology dependencies
- Manual failure points
- Target-state requirements
- Implementation priorities

---

## 2. Current-State Summary

PLG’s assumed current environment relies on:

- Email-based access requests
- Verbal or informal approvals
- Manager knowledge of job requirements
- System-specific provisioning practices
- Manual spreadsheets
- Inconsistent role definitions
- Limited independent verification
- Ad hoc access reviews
- Delayed termination notification
- Incomplete vendor-account tracking
- Scattered evidence
- Limited control metrics

The existing practices may support daily operations, but they do not provide consistent governance, traceability, or assurance.

---

## 3. Current-State and Future-State Comparison

| Process area | Assumed current state | Target future state |
| --- | --- | --- |
| Workforce-event source | Email, phone call, or verbal notice | HR-controlled event containing required fields and timestamps |
| Identity verification | Varies by department | Defined identity-validation procedure |
| Access requests | Free-form email | Standard request form tied to roles and entitlements |
| Business justification | Inconsistent | Required for every nonstandard request |
| Role definitions | Informal or system-specific | Approved role and entitlement catalog |
| Approvals | Vary by system | Risk-based approval matrix |
| Least privilege | Manager judgment | Role comparison and documented exception process |
| Segregation of duties | Informal | Defined prohibited combinations and secondary approval |
| Provisioning | Manual system changes | Controlled queue with required evidence |
| Verification | Often performed by provisioner | Independent verification for higher-risk access |
| Transfers | New access added without full removal review | Current-versus-target comparison and obsolete-access removal |
| Terminations | Variable notification and timing | Coordinated, time-bound revocation workflow |
| Contractor access | May lack consistent sponsor or expiration | Named sponsor, limited role, and mandatory expiration |
| Temporary access | Manually tracked | Defined expiration and monitoring |
| Privileged access | Standard account may receive elevation | Separate account, enhanced approval, MFA, logging, and review |
| Access reviews | Ad hoc spreadsheet exercise | Defined population, context, decision, remediation, and attestation |
| Exceptions | Informal operational workaround | Risk-assessed, approved, monitored, and time-bound |
| Evidence | Stored across email and tickets | Controlled evidence catalog and repository |
| Testing | Reactive or audit-driven | Risk-based control-assessment plan |
| Metrics | Ticket volume and anecdotal issues | KPI, KRI, SLA, trend, and control-health reporting |
| Remediation | Informal follow-up | POA&M ownership, milestones, validation, and closure |

---

## 4. Gap Analysis

### Gap 1 — No Authoritative Workforce Trigger

**Condition:** Joiner, mover, and leaver events may arrive through different communication methods.

**Risk:** Access actions may be late, incomplete, or inaccurate.

**Target requirement:** HR must provide the authoritative event, effective time, workforce type, manager, role, and location.

### Gap 2 — Inconsistent Role Definitions

**Condition:** Managers request access using application-specific knowledge or prior examples.

**Risk:** Users may receive excessive or inappropriate permissions.

**Target requirement:** System Owners must maintain approved role and entitlement catalogs.

### Gap 3 — Weak Approval Consistency

**Condition:** Approval requirements differ across systems.

**Risk:** Sensitive or privileged access may be granted without appropriate authority.

**Target requirement:** PLG must establish a risk-based approval matrix.

### Gap 4 — Limited Segregation-of-Duties Analysis

**Condition:** Conflicting permissions may be evaluated manually or not at all.

**Risk:** One person may control incompatible business activities.

**Target requirement:** PLG must define prohibited combinations and escalation procedures.

### Gap 5 — Incomplete Provisioning Verification

**Condition:** The person who provisions access may also close the request.

**Risk:** Incorrect access may remain undetected.

**Target requirement:** Higher-risk access must receive independent verification.

### Gap 6 — Delayed Access Removal

**Condition:** Termination and transfer events may not reach every application owner.

**Risk:** Former or transferred personnel may retain access.

**Target requirement:** The revocation workflow must include dependent systems, vendor accounts, physical access, and verification.

### Gap 7 — Weak Review Quality

**Condition:** Reviewers may receive technical entitlement names without sufficient context.

**Risk:** Access may be incorrectly certified.

**Target requirement:** Review packages must include business-friendly entitlement descriptions, HR status, role, manager, and last-use information where available.

### Gap 8 — Informal Exceptions

**Condition:** Operational needs may lead to undocumented workarounds.

**Risk:** Temporary risk may become permanent.

**Target requirement:** Exceptions must include justification, risk, compensating controls, owner, approval, expiration, and monitoring.

### Gap 9 — Fragmented Evidence

**Condition:** Evidence is distributed across email, tickets, spreadsheets, and system logs.

**Risk:** PLG may be unable to demonstrate control performance.

**Target requirement:** Evidence must be cataloged, protected, retained, and traceable.

### Gap 10 — Limited Performance Monitoring

**Condition:** PLG lacks consistent IAM KPIs and KRIs.

**Risk:** Control degradation may remain undetected.

**Target requirement:** PLG must define metrics, thresholds, owners, reporting cadence, and escalation actions.

---

## 5. Target-State Design Principles

The target state will:

- Use HR as the authoritative workforce-status source.
- Require a manager or sponsor for every identity.
- Use defined roles wherever practical.
- Apply least privilege.
- Identify segregation-of-duties conflicts.
- Separate request, approval, provisioning, and verification.
- Apply stronger controls to privileged access.
- Make temporary access expire.
- Include vendor and physical access in offboarding.
- Generate evidence during workflow execution.
- Measure control performance.
- Escalate failures based on risk.
- Track corrective actions to verified closure.

---

## 6. Prioritized Improvements

| Priority | Improvement | Reason |
| ---: | --- | --- |
| 1 | Implement verified termination and emergency-revocation workflow | Addresses the Critical leaver-access risk |
| 2 | Establish authoritative JML triggers | Supports the entire identity lifecycle |
| 3 | Create role and entitlement catalogs | Enables least privilege and review quality |
| 4 | Standardize access requests and approvals | Reduces inconsistent authorization |
| 5 | Govern privileged access | Addresses high-impact administrative risk |
| 6 | Establish periodic access reviews | Detects accumulated or outdated access |
| 7 | Formalize exceptions | Prevents permanent undocumented bypasses |
| 8 | Create evidence and testing standards | Supports assurance and remediation |
| 9 | Introduce metrics and monitoring | Detects control degradation |
| 10 | Automate selected handoffs and reconciliation | Reduces delay and manual error |

---

## 7. Target-State Outcome

The target operating model changes IAM from a collection of separate technical tasks into a governed business process.

The future state provides:

- Consistent triggers
- Defined ownership
- Risk-based decisions
- Repeatable workflows
- Reliable evidence
- Measurable performance
- Formal escalation
- Continuous improvement
