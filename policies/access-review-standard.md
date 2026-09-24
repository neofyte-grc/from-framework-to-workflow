# Access Review Standard

## Document Control

| Field | Value |
| --- | --- |
| Organization | Peachtree Logistics Group (fictional) |
| Standard owner | GRC Analyst |
| Accountable owners | System Owners |
| Version | 1.0 |
| Status | Portfolio design artifact |
| Review frequency | Annually and following material change |

---

## 1. Purpose

This standard defines mandatory requirements for planning, conducting, documenting, remediating, and closing periodic access reviews.

The objective is to verify that access remains:

- Connected to an active identity
- Necessary for current duties
- Properly approved
- Consistent with least privilege
- Free from unresolved segregation-of-duties conflicts
- Appropriate for the information and system involved

---

## 2. Scope

This standard applies to:

- Employees
- Contractors
- Independent couriers
- Temporary workers
- Privileged users
- Standard user accounts
- Service accounts
- Shared accounts
- Remote access
- Application roles
- Group memberships
- Sensitive-data access
- Related physical access

---

## 3. Review Frequency

| Access category | Minimum frequency |
| --- | --- |
| Privileged access | Quarterly |
| Financial-system access | Quarterly |
| Medical-delivery information | Quarterly |
| Contractor and courier access | Quarterly |
| Remote administrative access | Quarterly |
| Service and shared accounts | Quarterly |
| Standard business access | Semiannually |
| Physical access | Semiannually |
| Event-driven review | Following a material change |

The System Owner may establish a more frequent schedule.

---

## 4. Review Planning

Before a review begins, GRC and the System Owner must define:

- Systems in scope
- Access categories
- Population period
- Reviewers
- Due date
- Escalation dates
- Evidence requirements
- Remediation SLA
- Quality-assurance method
- Final approver

---

## 5. Population Requirements

The population must include:

- Active accounts
- Disabled accounts awaiting deletion
- Dormant accounts
- Privileged accounts
- Service accounts
- Shared accounts
- Contractor accounts
- Accounts without an identified owner
- Temporary accounts
- Accounts subject to exceptions

The population must not be filtered solely to make the review easier.

---

## 6. Required Review Information

Reviewers must receive:

- User name
- Unique identifier
- Workforce type
- Employment status
- Department
- Manager or sponsor
- System
- Account
- Role
- Entitlements
- Business description of access
- Privileged status
- Account status
- Creation date
- Last-use date where available
- Approval reference
- Expiration date
- Existing exception
- Prior review decision

Technical entitlement names should be supplemented with business-friendly descriptions.

---

## 7. Reviewer Requirements

Reviewers must:

- Understand the user’s current responsibilities.
- Have authority over the access being reviewed.
- Receive sufficient information.
- Complete the review independently.
- Document each decision.
- Avoid certifying their own access.
- Escalate access they cannot evaluate.
- Complete the review by the due date.

Delegation must be documented and approved.

---

## 8. Allowed Decisions

| Decision | Definition |
| --- | --- |
| Certify | Access remains necessary and appropriate |
| Revoke | Access is no longer required |
| Modify | Access remains necessary but must be adjusted |
| Escalate | Additional authority or information is required |
| Suspend | Access should be restricted during investigation |

Blank decisions are not permitted.

---

## 9. Certification Criteria

Access may be certified only when:

- The identity is active.
- The manager or sponsor is current.
- Access supports present responsibilities.
- Privilege is proportionate.
- Required approval exists.
- Temporary access has not expired.
- No prohibited conflict exists.
- Required training is current.
- Applicable exceptions remain valid.
- The account is attributable to an owner.

---

## 10. Remediation Requirements

Revocation or modification decisions must create trackable remediation actions.

Remediation records must contain:

- User
- Account
- Entitlement
- Decision
- Requester or reviewer
- Assigned technician
- Due date
- Completion date
- Verification
- Final status

High-risk access must receive priority.

---

## 11. Remediation Verification

Review closure requires confirmation that:

- Revoked access was removed.
- Modified access matches the decision.
- Suspended access remains restricted.
- Escalated decisions were resolved.
- Exceptions were approved.
- Evidence is complete.

The person who performs a High-risk change should not be the only person verifying it.

---

## 12. Overdue Reviews

| Condition | Response |
| --- | --- |
| Approaching due date | Send reminder |
| One business day overdue | Escalate to reviewer’s manager |
| High-risk review overdue | Escalate to System Owner, Security, and GRC |
| Repeated delay | Document a control finding |
| No accountable reviewer | Suspend or restrict access based on risk |
| Revocation overdue | Escalate according to privilege and data sensitivity |

---

## 13. Quality Assurance

GRC should evaluate:

- Population completeness
- Reviewer authority
- Decision completion
- Unusual certification patterns
- Excessive blanket approvals
- Remediation completion
- Evidence quality
- Overdue actions
- Repeat exceptions
- Final attestation

A review with unreliable population data must not be represented as complete.

---

## 14. Evidence Requirements

The final review package must include:

- Scope
- Population
- Reconciliation
- Reviewer assignments
- Instructions
- Decisions
- Justifications where required
- Timestamps
- Remediation tickets
- Verification
- Escalations
- Exceptions
- Quality-assurance results
- System Owner attestation
- Final report

---

## 15. Metrics

The review process should measure:

- Reviews completed on time
- Reviewer completion rate
- Access certified
- Access revoked
- Access modified
- Orphaned accounts
- Inactive accounts
- Overdue revocations
- Average remediation time
- Review evidence completeness
- Repeat findings
- Privileged access with current certification

---

## 16. Exceptions

Any inability to meet this standard must follow the Access Exception and Escalation Standard.

An exception must not be used to:

- Eliminate periodic review
- Permit self-certification
- Exclude High-risk accounts
- Close unresolved revocations
- Hide an incomplete population

---

## 17. Disclaimer

PLG and this standard are fictional. This document is an educational portfolio artifact and does not represent an independent audit or production control.
