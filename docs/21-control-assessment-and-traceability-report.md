# Control Assessment and Traceability Report

## Document Control

| Field | Value |
| --- | --- |
| Organization | Peachtree Logistics Group (fictional) |
| Project | From Framework to Workflow |
| Assessment coordinator | GRC Analyst |
| Version | 1.0 |
| Status | Fictional portfolio assessment |
| Assessment type | Design and illustrative operating-effectiveness review |

---

## 1. Executive Assessment Statement

This fictional assessment evaluates whether PLG’s proposed IAM controls are logically designed to address identified access risks and whether the example evidence model could support future operating-effectiveness testing.

The assessment does not represent:

- A production control assessment
- An independent audit
- A certification
- A FedRAMP authorization
- A legal compliance determination
- Proof of actual operating effectiveness

---

## 2. Assessment Objectives

The assessment evaluates whether:

- Risks are clearly defined.
- Requirements are mapped appropriately.
- Control objectives address the risks.
- Workflows contain executable activities.
- Ownership and accountability are defined.
- Evidence requirements are sufficient.
- Test procedures are repeatable.
- Metrics support monitoring.
- Exceptions feed remediation.
- Traceability is maintained.

---

## 3. Assessment Scope

The assessment covers:

- `CTRL-001` — Account Lifecycle Authorization
- `CTRL-002` — Least Privilege and Segregation of Duties
- `CTRL-003` — Provisioning Accuracy and Verification
- `CTRL-004` — Timely Access Removal
- `CTRL-005` — Periodic Access Certification
- `CTRL-006` — Privileged-Access Governance
- `CTRL-007` — Exception and Risk-Acceptance Governance
- `CTRL-008` — IAM Policy Governance
- `CTRL-009` — Identity and Authentication Management
- `CTRL-010` — Control Assessment
- `CTRL-011` — Continuous Monitoring and Improvement

---

## 4. Assessment Methods

### Examine

Review:

- Policies
- Standards
- Workflows
- Risk register
- Requirements register
- Role catalog
- Access requests
- Approval records
- System reports
- Logs
- Review packages
- Exceptions
- Findings
- POA&M records

### Interview

Discuss responsibilities with:

- HR
- Managers
- System Owners
- IT
- Security
- GRC
- Facilities
- Contractor Sponsors

### Test

Evaluate fictional samples by:

- Comparing approvals with assigned access
- Comparing termination times with disablement times
- Reviewing privileged-access requirements
- Evaluating access-review decisions
- Inspecting exceptions
- Verifying remediation evidence

---

## 5. Traceability Matrix

| Requirement | Risk | Control | Workflow | Evidence | Test | Metric |
| --- | --- | --- | --- | --- | --- | --- |
| `REQ-003` | `IAM-RISK-001` | `CTRL-001` | `WF-001` | `EVID-001`, `EVID-002`, `EVID-003` | `TEST-001` | `MET-002` |
| `REQ-004` | `IAM-RISK-002` | `CTRL-003` | `WF-003` | `EVID-003`, `EVID-011` | `TEST-002` | `MET-001` |
| `REQ-005` | `IAM-RISK-003` | `CTRL-002` | `WF-002` | `EVID-004` | `TEST-002` | `MET-009` |
| `REQ-006` | `IAM-RISK-002` | `CTRL-002` | `WF-002` | `EVID-005` | `TEST-002` | `MET-002` |
| `REQ-011` | `IAM-RISK-005` | `CTRL-004` | `WF-006` | `EVID-007` | `TEST-003` | `MET-003`, `MET-005` |
| `REQ-012` | `IAM-RISK-006` | `CTRL-004` | `WF-001` | `EVID-008` | `TEST-004` | `MET-005` |
| `REQ-013` | `IAM-RISK-007` | `CTRL-006` | `WF-005` | `EVID-009` | `TEST-006` | `MET-007` |
| `REQ-014` | `IAM-RISK-007` | `CTRL-006` | `WF-005` | `EVID-009` | `TEST-006` | `MET-007` |
| `REQ-015` | `IAM-RISK-008` | `CTRL-010` | Assessment | `EVID-014` | `TEST-008` | `MET-009` |
| `REQ-016` | `IAM-RISK-008` | `CTRL-007` | `WF-007` | `EVID-010`, `EVID-013` | `TEST-007` | `MET-006` |
| `REQ-017` | `IAM-RISK-008` | `CTRL-011` | Monitoring | `EVID-015` | `TEST-008` | `MET-008`, `MET-012` |

---

## 6. Design Assessment

| Control | Design assessment | Rationale |
| --- | --- | --- |
| `CTRL-001` | Adequately designed | Defines authoritative triggers, approvals, actions, and evidence |
| `CTRL-002` | Adequately designed with dependency | Requires a complete role catalog and SoD rules |
| `CTRL-003` | Adequately designed | Separates provisioning and verification for higher-risk access |
| `CTRL-004` | Adequately designed | Includes timing, dependent systems, physical access, and escalation |
| `CTRL-005` | Adequately designed with dependency | Requires complete populations and knowledgeable reviewers |
| `CTRL-006` | Adequately designed | Includes enhanced approval, MFA, logging, review, and expiration |
| `CTRL-007` | Adequately designed | Establishes risk authority, compensation, monitoring, and expiration |
| `CTRL-008` | Adequately designed | Establishes governance and review expectations |
| `CTRL-009` | Adequately designed | Defines unique identity and authenticator requirements |
| `CTRL-010` | Adequately designed | Defines evidence and assessment expectations |
| `CTRL-011` | Adequately designed | Connects metrics, escalation, findings, and remediation |

---

## 7. Illustrative Findings

### `FIND-001` — Incomplete Vendor-Account Termination Evidence

**Severity:** High  
**Affected risk:** `IAM-RISK-005`  
**Affected control:** `CTRL-004`

**Condition:** The sample termination package does not confirm removal from every vendor-managed application.

**Risk:** A departed user could retain access outside the central identity system.

**Recommendation:** Require System Owner confirmation for dependent applications and reconcile vendor accounts with termination events.

**Related POA&M:** `POAM-001`

### `FIND-002` — Insufficient Entitlement Context

**Severity:** Moderate  
**Affected risk:** `IAM-RISK-010`  
**Affected control:** `CTRL-005`

**Condition:** Reviewers receive technical group names without business descriptions.

**Risk:** Reviewers may certify inappropriate access because they do not understand the entitlement.

**Recommendation:** Add business descriptions, risk level, data scope, and role alignment to review packages.

**Related POA&M:** `POAM-003`

### `FIND-003` — Incomplete Exception Closure Criteria

**Severity:** Moderate  
**Affected risk:** `IAM-RISK-008`  
**Affected control:** `CTRL-007`

**Condition:** The sample exception identifies an expiration date but does not define the evidence needed for closure.

**Risk:** The exception could remain unresolved or be renewed without sufficient validation.

**Recommendation:** Require measurable closure criteria and remediation evidence.

### `FIND-004` — Privileged-Access Expiration Inconsistency

**Severity:** High  
**Affected risk:** `IAM-RISK-007`  
**Affected control:** `CTRL-006`

**Condition:** Some privileged roles are proposed as standing access without documented justification.

**Risk:** Excessive administrative access could remain active.

**Recommendation:** Require time-bound access where practical and documented approval for standing privilege.

**Related POA&M:** `POAM-004`

---

## 8. Readiness Conclusion

The target design provides a coherent IAM governance model with:

- Defined risks
- Framework traceability
- Control ownership
- Executable workflows
- Evidence expectations
- Assessment procedures
- Metrics
- Escalation
- Remediation

Production readiness would require:

- Stakeholder validation
- Complete system and entitlement inventories
- Approved policies
- Implemented workflows
- Technical configuration
- Representative evidence
- Independent testing
- Confirmed operating effectiveness
- Validated vendor participation
- Approved retention requirements

---

## 9. Overall Conclusion

The project demonstrates how governance requirements can be translated into accountable and measurable operations.

The design is suitable as a portfolio demonstration of GRC engineering, but it must not be represented as a production implementation or formal compliance assessment.
