# Sample Role and Entitlement Record

> **Fictional evidence notice:** This artifact uses fictional role, system, and approval information for portfolio demonstration purposes.

## Evidence Identification

| Field | Value |
| --- | --- |
| Evidence ID | `EVID-005` |
| Catalog record | `ROLE-CAT-004` |
| Related control | `CTRL-002` — Least Privilege and Segregation of Duties |
| Related risk | `IAM-RISK-002` |
| Version | 1.0 |
| Status | Approved fictional record |

---

## 1. Role Definition

| Field | Value |
| --- | --- |
| Role name | Dispatcher I |
| Department | Dispatch Operations |
| Role owner | Dispatch Manager |
| Primary System Owner | Logistics Platform Owner |
| Business purpose | Coordinate active deliveries and maintain operational shipment status |
| Eligible workforce types | PLG employees |
| Eligible locations | Atlanta Operations Center and approved remote location |
| Risk rating | Moderate |
| Review frequency | Semiannually |
| Lifecycle status | Active |

---

## 2. Role Responsibilities

The Dispatcher I role may:

- Review assigned shipment information.
- Assign available employed drivers and approved couriers.
- Update operational delivery status.
- Record routine delivery exceptions.
- Communicate with drivers and operational personnel.
- Review read-only warehouse shipment readiness.
- Access customer information required for active delivery coordination.

The role may not:

- Modify customer billing.
- Approve invoices.
- Release payments.
- Create or modify user accounts.
- Change system security settings.
- Modify warehouse inventory.
- View shipments outside the approved operational scope without documented need.
- Access administrative functions.

---

## 3. Approved Entitlements

| System | Role or entitlement | Access level | Business purpose | Privileged? |
| --- | --- | --- | --- | --- |
| Microsoft 365 | Dispatch Operations Group | Standard user | Dispatch communication and approved document collaboration | No |
| Logistics and Freight Platform | Dispatch Viewer | Read and limited operational update | Review shipment information and update operational status | No |
| Dispatch and Delivery Platform | Dispatcher I | Create and update assignments | Assign drivers and manage delivery workflow | No |
| Warehouse Management System | Shipment Status Viewer | Read only | Confirm shipment readiness | No |
| Billing and Accounting System | None | No access | Not required for the role | No |

---

## 4. Restricted Entitlements

| Entitlement | Restriction reason | Required authority |
| --- | --- | --- |
| Customer Billing Administrator | Not required for dispatch duties | Finance Manager and System Owner |
| Warehouse Inventory Adjustment | Creates operational and SoD risk | Warehouse Manager and WMS Owner |
| User Administrator | Privileged technical access | IT Director and Security Lead |
| Global Shipment Export | Broad customer and route-data exposure | Logistics Platform Owner and Data Owner |
| Privileged Dispatch Administrator | Can change roles and platform settings | Security Lead and System Owner |

---

## 5. Prohibited Combinations

| Conflict ID | Conflicting permissions | Risk | Resolution |
| --- | --- | --- | --- |
| `SOD-001` | Driver assignment and invoice approval | User could influence a delivery and approve related financial activity | Billing approval must remain excluded |
| `SOD-002` | Shipment-status update and audit-log administration | User could alter activity and interfere with evidence | Audit administration must remain excluded |
| `SOD-003` | Courier assignment and courier-payment release | User could assign work and authorize payment | Payment release must remain excluded |
| `SOD-004` | WMS shipment viewing and inventory adjustment | Role requires status visibility but not inventory modification | WMS access remains read only |

---

## 6. Eligibility Requirements

| Requirement | Required? |
| --- | --- |
| Active employee status | Yes |
| Assigned Dispatch Manager | Yes |
| Security awareness training | Yes |
| Dispatch operations training | Yes |
| Acceptable-use acknowledgement | Yes |
| Approved device | Yes |
| MFA enrollment | Yes |
| Background requirement | Per PLG hiring process |

---

## 7. Provisioning Requirements

| Requirement | Standard |
| --- | --- |
| Account type | Named user account |
| MFA | Required |
| Remote access | Conditional access from approved device |
| Location restriction | Approved PLG or managed remote context |
| Logging | Authentication and application activity |
| Expiration | Workforce lifecycle event |
| Independent verification | Required for initial role assignment |
| Periodic review | Semiannual |

---

## 8. Approval Record

| Approver | Role | Decision | Date |
| --- | --- | --- | --- |
| Maya Thompson | Dispatch Manager | Approved | July 15, 2026 |
| Marcus Lee | Logistics Platform Owner | Approved | July 16, 2026 |
| Renee Carter | WMS Owner | Approved | July 16, 2026 |
| Priya Shah | GRC Analyst | Reviewed | July 17, 2026 |

---

## 9. Review and Change History

| Version | Date | Change | Author | Approver |
| --- | --- | --- | --- | --- |
| 1.0 | July 17, 2026 | Initial fictional role definition | Priya Shah | Marcus Lee |

---

## 10. Evidence Conclusion

The Dispatcher I record defines approved permissions, restricted permissions, prohibited combinations, eligibility requirements, provisioning controls, and review expectations.

The role supports least privilege by excluding billing, inventory modification, security administration, and other functions that are unnecessary for routine dispatch work.
