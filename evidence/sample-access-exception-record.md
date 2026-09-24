# Sample Access Exception Record

> **Fictional evidence notice:** This record demonstrates fictional exception and risk-acceptance documentation.

## Exception Identification

| Field | Value |
| --- | --- |
| Evidence ID | `EVID-013` |
| Exception ID | `EXC-2026-0006` |
| Related workflow | `WF-007` — Access Exception and Risk Acceptance |
| Related control | `CTRL-007` |
| Status | Approved and later closed |
| Residual-risk level | Moderate |

---

## 1. Request Information

| Field | Value |
| --- | --- |
| Request date | June 1, 2026 |
| Requester | Renee Carter, WMS Owner |
| Business owner | Warehouse Operations Manager |
| Risk owner | CIO / IT Director |
| Requested start | June 6, 2026 |
| Requested expiration | August 31, 2026 |
| Affected system | Warehouse Management System |

---

## 2. Unmet Requirement

PLG’s Identity Lifecycle Management Standard requires individual named accounts for interactive system use.

The legacy WMS scanning module could not support individual accounts for a limited group of shared warehouse scanners without a planned software update.

---

## 3. Business Justification

Warehouse personnel required continuous scanning capability for receiving and shipment staging.

Disabling the shared scanner workflow before the planned update would have interrupted warehouse operations. The exception permitted restricted shared scanner access while PLG completed the account-capability upgrade.

---

## 4. Scope

| Field | Value |
| --- | --- |
| Affected devices | Six warehouse scanners |
| Affected location | Atlanta Warehouse |
| Affected users | Authorized warehouse shift personnel |
| Access level | Scan and update assigned warehouse tasks |
| Restricted activities | Administration, inventory adjustment approval, user management |
| Sensitive data | Limited shipment and inventory information |
| Privileged access | No |

---

## 5. Alternatives Considered

| Alternative | Decision |
| --- | --- |
| Disable scanners | Rejected because it would interrupt receiving and shipment staging |
| Assign one device per user | Not feasible because the site had fewer devices than shift personnel |
| Use named web accounts | Module did not support the required scanning workflow |
| Restrict shared role and increase monitoring | Selected as temporary treatment |
| Accelerate WMS update | Included in corrective-action plan |

---

## 6. Risk Assessment

**Risk statement:**

> Because multiple authorized workers use a shared scanner identity, PLG may be unable to attribute an inappropriate transaction to one individual, resulting in weak accountability or delayed investigation.

| Field | Value |
| --- | --- |
| Likelihood | 3 — Possible |
| Impact | 4 — Major |
| Inherent-risk score | 12 |
| Inherent-risk rating | High |
| Related risk | `IAM-RISK-004` |

---

## 7. Compensating Controls

| Control | Owner | Frequency | Evidence |
| --- | --- | --- | --- |
| Restrict scanners to approved warehouse network | IT Director | Continuous | Network-access configuration |
| Restrict shared role to scanning functions | WMS Owner | Continuous | Entitlement record |
| Require individual badge sign-in before scanner checkout | Warehouse Manager | Per shift | Device checkout log |
| Record device identifier with each transaction | WMS Owner | Per transaction | WMS activity log |
| Supervisor reviews exception transactions | Warehouse Supervisor | Daily | Review log |
| Rotate shared credential | IT Service Desk | Every 14 days | Credential-change record |
| Reconcile scanner activity with shift roster | GRC Analyst | Monthly | Reconciliation record |

---

## 8. Residual Risk

| Field | Value |
| --- | --- |
| Residual likelihood | 2 — Unlikely |
| Residual impact | 3 — Moderate |
| Residual-risk score | 6 |
| Residual-risk rating | Moderate |
| Within approval authority | Yes |

---

## 9. Corrective-Action Plan

| Milestone | Owner | Target | Completion |
| --- | --- | --- | --- |
| Confirm individual-account capability in upgraded module | WMS Owner | June 15 | June 13 |
| Test named scanner accounts | IT and Warehouse Operations | July 15 | July 12 |
| Train warehouse supervisors | Warehouse Manager | August 10 | August 8 |
| Deploy named accounts | IT Director | August 25 | August 22 |
| Disable shared scanner account | IT Director | August 31 | August 22 |

---

## 10. Approval

| Approver | Decision | Date | Conditions |
| --- | --- | --- | --- |
| Warehouse Operations Manager | Approved | June 2, 2026 | Enforce checkout and daily review |
| Information Security Lead | Approved | June 3, 2026 | Restrict network and maintain logs |
| CIO / IT Director | Approved | June 3, 2026 | Exception expires no later than August 31 |
| GRC Analyst | Reviewed | June 4, 2026 | Monthly monitoring required |

---

## 11. Monitoring Results

| Month | Result | Issue | Response |
| --- | --- | --- | --- |
| June | Effective | One incomplete checkout entry | Supervisor coaching |
| July | Effective | No material exception | None |
| August | Effective | Named-account deployment completed early | Begin closure |

---

## 12. Closure

| Field | Value |
| --- | --- |
| Closure reason | Individual scanner accounts implemented |
| Shared account disabled | August 22, 2026 |
| Closure evidence | Account inventory, entitlement export, disablement record |
| Closure validated by | Priya Shah, GRC Analyst |
| Risk-owner acknowledgement | CIO / IT Director |
| Closure date | August 25, 2026 |
| Final status | Closed |

---

## 13. Evidence Conclusion

The exception documented the unmet requirement, business need, alternatives, risk, compensating controls, accountable owners, expiration, monitoring, and corrective action.

PLG closed the exception before its approved expiration after implementing individual named scanner accounts.
