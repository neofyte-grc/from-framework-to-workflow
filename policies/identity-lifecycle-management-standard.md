# Identity Lifecycle Management Standard

## Document Control

| Field | Value |
| --- | --- |
| Organization | Peachtree Logistics Group (fictional) |
| Standard owner | CIO / IT Director |
| Process owners | HR Manager and IT Director |
| Version | 1.0 |
| Status | Portfolio design artifact |
| Review frequency | Annually and following material change |

---

## 1. Purpose

This standard defines mandatory requirements for creating, modifying, suspending, reviewing, and removing workforce and third-party identities.

It operationalizes PLG’s Access Control Policy across the joiner, mover, and leaver lifecycle.

---

## 2. Scope

This standard applies to:

- Employees
- Contractors
- Independent couriers
- Temporary workers
- Interns
- Vendors
- Privileged administrators
- Service accounts
- Shared accounts
- Logical access
- Remote access
- Related physical access

---

## 3. Authoritative Sources

HR is the authoritative source for employee status.

The approved Contractor Sponsor or Vendor Manager is the authoritative business source for:

- Contractors
- Independent couriers
- Temporary personnel
- Vendor users

Technology systems must not independently determine whether a person remains authorized without reference to the appropriate authoritative source.

---

## 4. Required Identity Attributes

Every identity record must include:

- Unique workforce or relationship identifier
- Full name
- Workforce type
- Department or service area
- Manager or sponsor
- Job or service role
- Work location
- Start date
- End date where applicable
- Current status
- Required systems
- Privileged status
- Last lifecycle event
- Related approval record

---

## 5. Joiner Requirements

Before access is provisioned:

1. The person’s identity must be verified.
2. An approved workforce or contractor event must exist.
3. A manager or sponsor must be assigned.
4. The role and department must be documented.
5. Required systems must be identified.
6. Standard access must be selected from an approved role catalog.
7. Nonstandard access must receive additional approval.
8. Contractor and courier access must have an expiration date.
9. Privileged access must follow the privileged-access workflow.
10. Access must not activate before the approved start time.

---

## 6. Mover Requirements

A mover event must be initiated for:

- Transfer
- Promotion
- Demotion
- Temporary assignment
- Location change
- Department change
- Manager change
- Leave of absence
- Return from leave
- Employment-type change
- Change in contractor responsibilities

The mover process must:

1. Identify current access.
2. Identify target-role access.
3. Determine obsolete permissions.
4. Determine required new permissions.
5. Evaluate segregation-of-duties conflicts.
6. Remove obsolete access before or with new access.
7. Document approved temporary overlap.
8. Verify the final access state.

---

## 7. Leaver Requirements

Leaver events must include:

- Effective date and time
- Separation classification
- Manager or sponsor
- Known systems
- Privileged-access status
- Remote-access status
- Devices
- Badges and keys
- Special confidentiality requirements

Access must be removed by the effective separation time.

The process must address:

- Central identity
- Microsoft 365
- Business applications
- Remote access
- Privileged access
- Active sessions
- MFA tokens
- API or authentication tokens
- Vendor accounts
- Physical access
- Devices
- Shared secrets

---

## 8. Service-Level Requirements

| Event | Required completion |
| --- | --- |
| Standard joiner | By the approved start time |
| Standard mover | Within one business day of the effective change |
| Contractor expiration | By the documented expiration |
| Voluntary termination | By the effective separation time |
| Involuntary termination | Coordinated immediate disablement |
| Emergency revocation | Immediate authorized action |
| High-risk discrepancy | Immediate containment |
| Standard discrepancy | Within one business day |

---

## 9. Contractor and Courier Requirements

Nonemployee identities must:

- Have a named sponsor.
- Have a documented service relationship.
- Be classified separately from employees where supported.
- Receive access limited to their assignment.
- Have an expiration date.
- Be reviewed at least quarterly.
- Be disabled when the relationship ends.
- Be included in account reconciliation.

A sponsor’s departure or transfer must trigger reassignment or revocation of sponsored access.

---

## 10. Temporary Access

Temporary access must include:

- Business justification
- Approver
- Start date
- Expiration date
- Scope
- Monitoring requirements
- Removal verification

Temporary access must not be converted into standing access without a new authorization decision.

---

## 11. Privileged Identities

Privileged identities must:

- Be uniquely assigned.
- Use separate accounts where supported.
- Use MFA where supported.
- Receive Security approval.
- Be limited in scope and duration.
- Produce audit logs.
- Receive quarterly review.
- Be removed when no longer required.

---

## 12. Service Accounts

Service accounts must have:

- A unique account name
- Documented purpose
- Business owner
- Technical owner
- Minimum required privilege
- Protected authenticator
- Rotation requirement
- Monitoring requirement
- Review date
- End-of-life criteria

Service accounts may not be used for routine interactive user activity unless specifically approved.

---

## 13. Shared Accounts

Shared accounts require an approved exception.

The exception must document:

- Technical limitation
- Business need
- Authorized users
- Credential protection
- Individual-attribution mechanism
- Monitoring
- Rotation
- Review
- Remediation plan
- Expiration

---

## 14. Provisioning Requirements

Provisioners must:

- Use a controlled work queue.
- Verify request completeness.
- Implement only approved access.
- Record the person performing the action.
- Record the completion timestamp.
- Attach system-generated evidence.
- Apply expiration where required.
- Configure authentication controls.
- Send the result for verification.

---

## 15. Verification Requirements

Independent verification is mandatory for:

- Privileged access
- Financial-system access
- Medical-delivery information
- Emergency access
- Access granted through an exception
- Other High-risk entitlements

Verification must compare approved access with actual assigned access.

---

## 16. Reconciliation Requirements

At a defined frequency, PLG must compare:

- Active workers with active accounts
- Terminated workers with enabled accounts
- Approved access with assigned access
- Contractor end dates with account expiration
- Privileged approvals with privileged accounts
- Temporary approvals with active temporary access
- Service accounts with accountable owners

Unexplained differences must be investigated.

---

## 17. Evidence Requirements

Lifecycle evidence includes:

- Workforce event
- Access request
- Approval
- Role comparison
- Provisioning record
- Verification
- Modification record
- Disablement record
- Session revocation
- Physical-access removal
- Exception
- Final closure

---

## 18. Exceptions and Escalation

Activities that cannot meet this standard must follow the Access Exception and Escalation Standard.

Critical failures include:

- Active privileged account belonging to a terminated user
- Unauthorized account creation
- Untraceable administrative account
- Failed emergency revocation
- Access restored without authorization

Critical failures require immediate escalation to the CIO and Information Security Lead.

---

## 19. Compliance Measurement

Performance should be measured through:

- Lifecycle events completed within SLA
- Accounts matched to active workforce records
- Terminations completed on time
- Mover access removed on time
- Temporary access removed at expiration
- Contractor accounts with active sponsors
- Privileged accounts with current approval
- Verification completion
- Evidence completeness

---

## 20. Disclaimer

PLG and this standard are fictional. This document is an educational portfolio artifact and does not demonstrate production implementation or operating effectiveness.
