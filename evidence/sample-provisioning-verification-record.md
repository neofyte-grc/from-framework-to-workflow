# Sample Provisioning Verification Record

> **Fictional evidence notice:** The account, personnel, systems, timestamps, and results in this record are fictional.

## Evidence Identification

| Field | Value |
| --- | --- |
| Evidence ID | `EVID-011` |
| Verification record | `VERIFY-2026-0088` |
| Access request | `AR-2026-0042` |
| Provisioning ticket | `IAM-TKT-2026-0714` |
| Related workflow | `WF-003` — Provisioning and Verification |
| Related control | `CTRL-003` |
| Verification result | Pass after correction |

---

## 1. User and Request

| Field | Value |
| --- | --- |
| User | Jordan Ellis |
| Workforce identifier | `PLG-1047` |
| Department | Dispatch Operations |
| Approved role | Dispatcher I |
| Approved start | August 17, 2026, 6:00 AM |
| Privileged access | No |
| Temporary access | No |

---

## 2. Provisioning Record

| Field | Value |
| --- | --- |
| Provisioner | Daniel Brooks, IT Service Desk |
| Provisioning started | August 14, 2026, 2:56 PM |
| Provisioning completed | August 14, 2026, 3:42 PM |
| Account activation | Scheduled for August 17, 2026, 6:00 AM |
| MFA configured | Yes |
| Duplicate-account check | Pass |
| System evidence attached | Yes |

---

## 3. Approved Versus Assigned Access

| System | Approved access | Initially assigned access | Final assigned access | Result |
| --- | --- | --- | --- | --- |
| Microsoft 365 | Dispatch Operations Group | Dispatch Operations Group | Dispatch Operations Group | Pass |
| Logistics Platform | Dispatch Viewer | Dispatch Viewer | Dispatch Viewer | Pass |
| Dispatch Platform | Dispatcher I | Dispatcher I | Dispatcher I | Pass |
| WMS | Shipment Status Viewer | Shipment Status Viewer plus Inventory Lookup | Shipment Status Viewer | Corrected |
| Billing System | No access | No access | No access | Pass |

---

## 4. Verification Checklist

| Verification item | Result | Notes |
| --- | --- | --- |
| Correct identity | Pass | Workforce ID matched HR event |
| Correct account | Pass | Unique named account assigned |
| Account activation date | Pass | Scheduled for approved start |
| Approved roles assigned | Pass | Final access matched approval |
| Unapproved roles absent | Pass after correction | Inventory Lookup removed |
| MFA configured | Pass | Enrollment confirmed |
| Privileged access absent | Pass | No administrative groups assigned |
| Expiration configured where required | Not applicable | Ongoing employee access |
| SoD restrictions preserved | Pass | Billing access absent |
| Evidence complete | Pass | Ticket and system records attached |

---

## 5. Discrepancy

| Field | Value |
| --- | --- |
| Discrepancy ID | `DISC-2026-0017` |
| Severity | Moderate |
| Condition | WMS provisioning initially included Inventory Lookup |
| Approved access | Shipment Status Viewer only |
| Potential risk | User could view inventory information beyond the approved operational need |
| Detected by | Alicia Green, Access Verifier |
| Detection time | August 15, 2026, 10:12 AM |

---

## 6. Corrective Action

1. The verifier returned the ticket to IT.
2. IT removed the Inventory Lookup entitlement.
3. IT captured an updated entitlement record.
4. The verifier repeated the comparison.
5. The final access matched the approved role.
6. The discrepancy was included in monthly provisioning-quality reporting.

| Field | Value |
| --- | --- |
| Corrected by | Daniel Brooks |
| Correction completed | August 15, 2026, 11:03 AM |
| Retested by | Alicia Green |
| Retest completed | August 15, 2026, 11:28 AM |
| Retest result | Pass |

---

## 7. Root-Cause Classification

| Field | Value |
| --- | --- |
| Root-cause category | Process / role-selection error |
| Cause | Provisioner selected an outdated WMS access bundle |
| Systemic issue? | Not confirmed |
| Follow-up | Review WMS provisioning instructions and monitor repeat discrepancies |
| Finding required? | No, unless repeated |

---

## 8. Final Verification

| Field | Value |
| --- | --- |
| Verifier | Alicia Green |
| Verification date | August 15, 2026 |
| Final result | Pass |
| Manager notified | Yes |
| User notified | At activation |
| Ticket closure | August 17, 2026 |
| Remaining issue | None |

---

## 9. Evidence Conclusion

Independent verification identified and corrected an entitlement that exceeded the approved role before the user began work.

The record demonstrates why approval evidence and provisioning evidence must be compared before closure.
