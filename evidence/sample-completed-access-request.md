# Sample Completed Access Request

> **Fictional evidence notice:** PLG, the individuals, accounts, approvals, and records in this artifact are fictional. This sample demonstrates the expected structure of control evidence and does not document a real access request.

## Evidence Identification

| Field | Value |
| --- | --- |
| Evidence ID | `EVID-002` |
| Request ID | `AR-2026-0042` |
| Related workflow | `WF-002` — Access Request and Approval |
| Related controls | `CTRL-001`, `CTRL-002` |
| Related risks | `IAM-RISK-001`, `IAM-RISK-002` |
| Request status | Approved and completed |
| Evidence period | Q3 2026 |
| Classification | Fictional portfolio evidence |

---

## 1. Request Information

| Field | Value |
| --- | --- |
| Request date | August 10, 2026 |
| Requested start date | August 17, 2026 |
| Requested expiration date | Not applicable — ongoing employee access |
| Requester | Maya Thompson, Dispatch Manager |
| Related workforce event | `HR-EVT-2026-0118` |
| Provisioning ticket | `IAM-TKT-2026-0714` |

---

## 2. User Information

| Field | Value |
| --- | --- |
| User | Jordan Ellis |
| Workforce identifier | `PLG-1047` |
| Workforce type | Employee |
| Department | Dispatch Operations |
| Job role | Dispatcher I |
| Manager | Maya Thompson |
| Work location | Atlanta Operations Center |
| Workforce status | Active |
| Start date | August 17, 2026 |

---

## 3. Requested Access

| System | Requested role or entitlement | Access level | Classification |
| --- | --- | --- | --- |
| Microsoft 365 | Dispatch Operations Group | Standard collaboration | Standard |
| Logistics and Freight Platform | Dispatch Viewer | Read and update assigned shipment status | Standard |
| Dispatch and Delivery Platform | Dispatcher I | Create and update driver assignments | Standard |
| Warehouse Management System | Shipment Status Viewer | Read only | Additional |
| Billing and Accounting System | None | None | Not requested |

---

## 4. Business Justification

Jordan Ellis was hired as a Dispatcher I. The role requires access to active shipment records, driver assignments, route status, delivery exceptions, and dispatch communications.

Read-only warehouse status access is required to confirm whether shipments are ready for driver assignment. The role does not require inventory adjustment, customer billing, payment approval, user administration, or privileged system access.

---

## 5. Least-Privilege Review

| Review question | Result |
| --- | --- |
| Access aligned with approved Dispatcher I role? | Yes |
| Lower access level available? | No for dispatch assignment functions |
| Read-only access sufficient for WMS? | Yes |
| Billing access required? | No |
| Privileged access required? | No |
| Temporary access appropriate? | No |
| Duplicate access identified? | No |

**Reviewer conclusion:** The requested permissions represent the minimum access necessary for the Dispatcher I role.

---

## 6. Segregation-of-Duties Review

| Field | Result |
| --- | --- |
| SoD review required? | Yes |
| Rules evaluated | Dispatch assignment versus billing approval; WMS viewing versus inventory adjustment |
| Conflict identified? | No |
| Reviewer | Marcus Lee, Logistics Platform Owner |
| Review date | August 11, 2026 |
| Review result | Pass |

Jordan may assign drivers and update operational shipment status but cannot approve invoices, adjust customer billing, release vendor payments, or modify warehouse inventory.

---

## 7. Prerequisites

| Requirement | Status |
| --- | --- |
| Security awareness training | Complete — August 12, 2026 |
| Acceptable-use acknowledgement | Complete — August 12, 2026 |
| Confidentiality acknowledgement | Complete — August 12, 2026 |
| Approved device assigned | Confirmed |
| MFA enrollment required | Confirmed |
| Dispatch training assigned | Confirmed |

---

## 8. Approval Record

| Approver | Role | Decision | Date and time | Conditions |
| --- | --- | --- | --- | --- |
| Maya Thompson | Department Manager | Approved | August 11, 2026, 9:18 AM | Access limited to Dispatcher I role |
| Marcus Lee | Logistics Platform Owner | Approved | August 11, 2026, 11:06 AM | No billing or administrative access |
| Renee Carter | WMS Owner | Approved | August 11, 2026, 2:21 PM | WMS access limited to read-only shipment status |
| Information Security | Additional approval | Not required | Not applicable | No privileged access requested |

---

## 9. Final Authorization

| Field | Value |
| --- | --- |
| Approved role | Dispatcher I |
| Approved start | August 17, 2026, 6:00 AM |
| Expiration | Not applicable |
| MFA required | Yes |
| Monitoring | Standard authentication and application logging |
| Exception required | No |
| Final decision | Approved |
| Decision date | August 11, 2026 |

---

## 10. Provisioning Summary

| Field | Value |
| --- | --- |
| Provisioner | Daniel Brooks, IT Service Desk |
| Provisioning completed | August 14, 2026, 3:42 PM |
| Account activation scheduled | August 17, 2026, 6:00 AM |
| MFA enrollment | Completed |
| Verification required | Yes |
| Verification result | Pass |
| Request closure date | August 17, 2026 |

---

## 11. Evidence Conclusion

The request contained a verified workforce event, documented business need, role comparison, least-privilege review, segregation-of-duties result, authorized approvals, provisioning evidence, and independent verification.

No exception or unresolved discrepancy was identified.
