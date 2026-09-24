# Sample Quarterly Access Review

> **Fictional evidence notice:** This access-review package contains fictional accounts, personnel, decisions, and results.

## Review Information

| Field | Value |
| --- | --- |
| Evidence ID | `EVID-012` |
| Review ID | `REVIEW-2026-Q3-PRIV-01` |
| Review period | Q3 2026 |
| System | Dispatch and Delivery Platform |
| Review type | Quarterly privileged and sensitive-access review |
| System Owner | Marcus Lee |
| GRC coordinator | Priya Shah |
| Review start | July 6, 2026 |
| Due date | July 17, 2026 |
| Final status | Complete with remediation |

---

## 1. Review Scope

The review covered:

- Privileged administrators
- Dispatch supervisors
- Users with broad shipment visibility
- Contractor and courier support accounts
- Temporary elevated access
- Service accounts
- Dormant accounts
- Accounts with approved exceptions

---

## 2. Population Validation

| Validation item | Result |
| --- | --- |
| Population generated from system source | Pass |
| Privileged accounts included | Pass |
| Contractor accounts included | Pass |
| Service accounts included | Pass |
| Dormant accounts included | Pass |
| Population reconciled to HR records | Pass |
| Population reconciled to contractor records | Pass with one discrepancy |
| Prior remediation included | Pass |
| Approved exceptions included | Pass |

**Population size:** 24 accounts  
**Population discrepancy:** One contractor support account lacked a current sponsor.

---

## 3. Review Decisions

| Record | Account | Workforce status | Access | Decision | Rationale |
| ---: | --- | --- | --- | --- | --- |
| 1 | `mthompson-admin` | Active employee | Dispatch Administrator | Certify | Current Dispatch Manager with approved administrative duties |
| 2 | `mlee-admin` | Active employee | Platform Administrator | Certify | Current System Owner |
| 3 | `jpatel-temp` | Active employee | Temporary Elevated Support | Revoke | Approved support period ended June 30 |
| 4 | `vendor-support-03` | Vendor | Vendor Support Administrator | Suspend | No current PLG sponsor identified |
| 5 | `dispatch-service-api` | Service account | API Integration | Certify with condition | Valid integration; credential rotation due |
| 6 | `rcole-supervisor` | Transferred employee | Dispatch Supervisor | Modify | User transferred to Warehouse Operations |
| 7 | `breakglass-dispatch` | Emergency account | Emergency Administrator | Certify | Required emergency account; quarterly test complete |
| 8 | `dispatch-audit` | Service account | Audit Export | Certify | Read-only audit function with current owner |

---

## 4. Decision Summary

| Decision | Count |
| --- | ---: |
| Certified | 19 |
| Certified with condition | 1 |
| Modified | 1 |
| Revoked | 1 |
| Suspended | 1 |
| Escalated | 1 |
| Total | 24 |

The escalated record involved a disputed entitlement requiring clarification from the System Owner and Security Lead. The issue was resolved before final closure.

---

## 5. Remediation

| Action ID | Account | Required action | Owner | Due date | Completion | Status |
| --- | --- | --- | --- | --- | --- | --- |
| `REM-001` | `jpatel-temp` | Remove temporary elevated role | IT Service Desk | July 8 | July 7 | Complete |
| `REM-002` | `vendor-support-03` | Suspend account pending sponsor validation | IT Service Desk | Immediate | July 7 | Complete |
| `REM-003` | `dispatch-service-api` | Rotate service credential | Platform Engineering | July 15 | July 14 | Complete |
| `REM-004` | `rcole-supervisor` | Remove Dispatch Supervisor and assign approved WMS viewer access | IT Service Desk | July 10 | July 9 | Complete |

---

## 6. Remediation Verification

| Action ID | Verifier | Verification method | Result | Date |
| --- | --- | --- | --- | --- |
| `REM-001` | Priya Shah | Entitlement export | Pass | July 8 |
| `REM-002` | Priya Shah | Account-status report | Pass | July 8 |
| `REM-003` | Information Security | Rotation and authentication record | Pass | July 15 |
| `REM-004` | Priya Shah | Current-versus-approved access comparison | Pass | July 10 |

---

## 7. Exception and Escalation

The vendor account remained suspended while the Vendor Manager determined whether PLG still required the support relationship.

The Vendor Manager confirmed that the contract had ended. IT permanently disabled the account on July 11, 2026.

No exception was approved.

---

## 8. Review Metrics

| Metric | Result | Target | Status |
| --- | ---: | ---: | --- |
| Review completed by due date | 100% | At least 98% | Green |
| Decisions completed | 100% | 100% | Green |
| Remediation completed on time | 100% | At least 95% | Green |
| Privileged accounts with current approval | 100% after remediation | 100% | Green |
| Population discrepancies | 1 of 24 | 0 | Amber |
| Evidence completeness | 100% | At least 98% | Green |

---

## 9. System Owner Attestation

I confirm that:

- The complete identified population was reviewed.
- Reviewers received sufficient access context.
- Each account received a decision.
- Required remediation was completed and verified.
- The unresolved vendor account was disabled.
- No High or Critical item remained open at closure.

| Field | Value |
| --- | --- |
| System Owner | Marcus Lee |
| Attestation date | July 17, 2026 |
| Final status | Closed |
