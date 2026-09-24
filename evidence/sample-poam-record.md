# Sample Plan of Action and Milestones Record

> **Fictional evidence notice:** This POA&M record contains fictional findings, systems, owners, dates, and remediation results.

## POA&M Identification

| Field | Value |
| --- | --- |
| POA&M ID | `POAM-001` |
| Finding ID | `FIND-001` |
| Finding source | Q3 2026 IAM Control Review |
| Date opened | October 11, 2026 |
| Severity | High |
| Current status | Closed |
| Closure date | November 24, 2026 |

---

## 1. Weakness

A vendor-managed support account remained active for approximately 19 hours after the associated third-party relationship ended.

The central identity account was disabled, but the termination process did not create a revocation task for the vendor application.

---

## 2. Affected Traceability

| Artifact | Reference |
| --- | --- |
| Requirement | `REQ-011` |
| Risk | `IAM-RISK-005` |
| Control | `CTRL-004` |
| Workflow | `WF-006` |
| Evidence | `EVID-007` |
| Test | `TEST-003` |
| Metric | `MET-003`, `MET-005` |

---

## 3. Root Cause

| Category | Analysis |
| --- | --- |
| Process | Termination checklist did not identify every vendor-managed platform |
| Technology | Vendor application lacked centralized deprovisioning |
| Ownership | System Owner did not receive a termination task |
| Evidence | Central account report was treated as full revocation confirmation |

---

## 4. Risk

**Risk statement:**

> Because vendor-managed application accounts are not consistently included in termination processing, a former third party may retain access, resulting in unauthorized activity or exposure of PLG information.

| Field | Value |
| --- | --- |
| Likelihood | 4 — Likely |
| Impact | 4 — Major |
| Current-risk score | 16 |
| Risk rating | High |
| Risk owner | CIO / IT Director |

---

## 5. Interim Controls

Until remediation was complete, PLG:

- Required the Vendor Manager to notify each vendor System Owner directly.
- Conducted a weekly terminated-user comparison against vendor-account lists.
- Restricted vendor support access to approved source locations.
- Escalated any unmatched terminated identity immediately.
- Required GRC confirmation before closing third-party terminations.

---

## 6. Corrective Action

PLG revised the termination process to:

1. Maintain an application-access inventory.
2. Identify vendor-managed systems associated with each identity.
3. Create application-specific revocation tasks.
4. Require System Owner completion evidence.
5. Prevent termination closure until dependent access is verified.
6. Perform recurring reconciliation between terminated identities and vendor accounts.

---

## 7. Milestones

| Milestone | Owner | Target date | Completion date | Status |
| --- | --- | --- | --- | --- |
| Inventory vendor-managed applications | Vendor Manager | October 21 | October 20 | Complete |
| Update termination checklist | GRC Analyst | October 25 | October 24 | Complete |
| Configure System Owner revocation tasks | IT Director | November 5 | November 3 | Complete |
| Train HR, IT, and System Owners | GRC Analyst | November 10 | November 9 | Complete |
| Test standard and emergency scenarios | Internal Assessor | November 18 | November 17 | Complete |
| Complete retest and closure review | GRC Analyst | November 25 | November 24 | Complete |

---

## 8. Validation Procedure

The validator:

1. Reviewed the revised termination checklist.
2. Confirmed the vendor application inventory.
3. Tested three fictional termination scenarios.
4. Confirmed creation of application-specific tasks.
5. Confirmed System Owner completion evidence.
6. Reconciled the terminated identities with vendor-account records.
7. Confirmed that termination closure required dependent-system verification.

---

## 9. Validation Results

| Test scenario | Expected result | Observed result |
| --- | --- | --- |
| Standard vendor termination | All dependent accounts disabled by effective time | Pass |
| Emergency vendor revocation | Immediate tasks and escalation generated | Pass |
| User with two vendor applications | Separate confirmations required | Pass |

---

## 10. Residual Risk

| Field | Value |
| --- | --- |
| Residual likelihood | 2 — Unlikely |
| Residual impact | 3 — Moderate |
| Residual-risk score | 6 |
| Residual-risk rating | Moderate |
| Risk-owner decision | Accepted within delegated authority |

---

## 11. Closure

| Field | Value |
| --- | --- |
| Corrective action implemented | Yes |
| Root cause addressed | Yes |
| Retest completed | Yes |
| Closure evidence complete | Yes |
| Closure recommended by | Priya Shah, GRC Analyst |
| Closure approved by | CIO / IT Director |
| Closure date | November 24, 2026 |
| Final status | Closed |

---

## 12. Lessons Learned

Central identity disablement does not prove that every application account has been removed.

Termination closure must account for the complete access boundary, including vendor-managed applications that do not integrate with the central identity system.
