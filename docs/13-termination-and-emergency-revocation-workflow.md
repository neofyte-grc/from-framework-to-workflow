# Termination and Emergency Revocation Workflow

## Document Control

| Field | Value |
| --- | --- |
| Organization | Peachtree Logistics Group (fictional) |
| Workflow ID | `WF-006` |
| Workflow owners | HR Manager and IT Director |
| Version | 1.0 |
| Status | Portfolio design artifact |

---

## 1. Purpose

This workflow defines how PLG removes logical, physical, remote, and third-party access following termination, contract expiration, suspected compromise, or another urgent event.

The workflow is designed to prevent:

- Former-user access
- Unauthorized remote access
- Continued privileged access
- Use of active sessions or tokens
- Access through vendor-managed systems
- Unauthorized facility entry
- Use of unreturned devices or credentials
- Incomplete revocation evidence

---

## 2. Scope

The workflow applies to:

- Voluntary termination
- Involuntary termination
- Contractor disengagement
- Independent courier removal
- Contract expiration
- Abandonment of position
- Extended leave requiring suspension
- Suspected credential compromise
- Insider-threat concern
- Policy violation requiring emergency restriction
- Court, legal, safety, or security directive

---

## 3. Termination Classifications

| Classification | Description | Required response |
| --- | --- | --- |
| Standard | Planned voluntary separation | Disable by effective separation time |
| Contract expiration | Known end of temporary relationship | Remove by documented expiration |
| Involuntary | Sensitive or employer-initiated separation | Coordinated immediate disablement |
| Emergency | Suspected compromise, misuse, or safety risk | Immediate containment |
| Temporary suspension | Access restricted pending review | Disable or restrict as authorized |

---

## 4. Authoritative Trigger

For employees, HR provides the authoritative termination event.

For contractors, couriers, and vendors, the authorized sponsor or Vendor Manager provides the event.

The event must include:

- Person
- Workforce identifier
- Relationship type
- Manager or sponsor
- Effective date and time
- Termination classification
- Known systems
- Privileged-access status
- Remote-access status
- Device and badge information
- Special confidentiality instructions

---

## 5. Standard Termination Workflow

1. HR records the termination event.
2. The manager identifies systems, devices, records, badges, keys, and tokens.
3. IT identifies all logical accounts.
4. The System Owner identifies vendor-managed or application-specific accounts.
5. Security identifies privileged, remote, and security-tool access.
6. Facilities identifies physical-access credentials.
7. Access removal is scheduled for the effective time.
8. IT disables central identity accounts.
9. Active sessions and remote-access tokens are revoked.
10. Privileged access is removed.
11. Application-specific and vendor accounts are disabled.
12. Physical access is disabled.
13. Devices, badges, keys, and tokens are recovered.
14. Shared credentials are rotated when required.
15. A separate reviewer verifies completion.
16. Unresolved items are escalated.
17. Evidence is retained.

---

## 6. Involuntary-Termination Workflow

Involuntary termination requires coordinated timing among:

- HR
- The Department Manager
- IT
- Security
- Facilities
- Legal or executive leadership where applicable

Actions should occur on a need-to-know basis.

Access should be disabled immediately before or during the separation meeting according to the authorized plan.

The user must not receive advance technical notification that could undermine the coordinated response.

---

## 7. Emergency Revocation Workflow

Emergency revocation may be initiated when:

- Credentials are suspected to be compromised.
- Privileged misuse is suspected.
- A serious policy violation occurs.
- A safety concern exists.
- A user presents an immediate operational or security risk.
- A device containing sensitive information is lost or stolen.

### Emergency Procedure

1. An authorized person submits the emergency request.
2. Security validates the urgency and scope.
3. IT disables or restricts the affected accounts.
4. Active sessions and tokens are revoked.
5. Privileged access is removed.
6. Relevant logs and evidence are preserved.
7. The incident-response process is initiated when appropriate.
8. The account remains restricted until an authorized restoration decision.
9. All actions and timestamps are documented.

---

## 8. Revocation Checklist

The checklist should address:

- Microsoft 365
- Logistics and freight platform
- Warehouse management system
- Dispatch and delivery platform
- Billing and accounting system
- VPN and remote access
- Administrative accounts
- Mobile-device access
- API tokens
- Authentication tokens
- MFA devices
- Shared secrets
- Vendor-managed accounts
- Physical badges
- Keys
- Company laptops
- Mobile devices
- Warehouse scanners
- Documents and records

---

## 9. Escalation Requirements

| Condition | Required escalation |
| --- | --- |
| Critical account remains active | Immediately notify CIO and Security Lead |
| Privileged account cannot be disabled | Initiate emergency containment |
| Vendor removal cannot be confirmed | Escalate to System Owner and Vendor Manager |
| Device or credential is unreturned | Notify Manager, HR, and Security |
| Physical access cannot be disabled | Notify Facilities and Security |
| Evidence is incomplete | Escalate to GRC before closure |
| Suspected misuse exists | Initiate incident-response process |
| Revocation misses the SLA | Document and investigate a control failure |

---

## 10. Restoration Following Suspension

Suspended access may be restored only when:

- The authorized investigating or management role approves restoration.
- The user’s identity and status remain valid.
- The reason for suspension has been resolved.
- Credentials are reset where necessary.
- Privileges are reassessed.
- The restoration is documented.
- The final configuration is verified.

---

## 11. Evidence Requirements

The evidence package includes:

- Authoritative termination or emergency event
- Effective date and time
- Account inventory
- Disablement timestamps
- Active-session revocation
- Privileged-access removal
- Vendor-account confirmation
- Physical-access removal
- Device and credential disposition
- Shared-secret rotation where required
- Independent verification
- Unresolved-item escalation
- Final closure approval

---

## 12. Failure Conditions

The workflow fails when:

- Notification is late or incomplete.
- A logical or physical account remains active.
- Privileged access remains active.
- Active sessions are not revoked.
- Contractor or vendor access is overlooked.
- Shared credentials remain unchanged when rotation is required.
- Devices or badges remain unresolved without escalation.
- Disablement timestamps cannot be verified.
- Evidence is missing.
- The event closes with unresolved Critical or High-risk access.

---

## 13. Metrics

The workflow supports:

- `MET-003` — Average termination-to-disablement time
- `MET-005` — Overdue revocations
- `MET-008` — Evidence completeness
- `MET-009` — Control-test exception rate

Additional measures include:

- Percentage of terminations completed within SLA
- Percentage of vendor accounts confirmed disabled
- Percentage of termination records independently verified
- Number of unreturned devices or badges
- Number of incomplete revocation records
- Number of emergency revocations
- Repeat causes of late disablement
