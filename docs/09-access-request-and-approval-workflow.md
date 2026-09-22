# Access Request and Approval Workflow

## Document Control

| Field | Value |
| --- | --- |
| Organization | Peachtree Logistics Group (fictional) |
| Workflow ID | `WF-002` |
| Workflow owner | Department Manager |
| Version | 1.0 |
| Status | Portfolio design artifact |

---

## 1. Purpose

This workflow standardizes how PLG requests, evaluates, approves, rejects, and documents access.

The workflow ensures that access is:

- Connected to a verified identity
- Supported by a business need
- Appropriate for the user’s current role
- Limited according to least privilege
- Evaluated for segregation-of-duties conflicts
- Approved by authorized personnel
- Time-bound when temporary
- Supported by reliable evidence

---

## 2. Scope

The workflow applies to:

- Standard role-based access
- Additional access
- Temporary access
- Elevated access
- Privileged access
- Contractor access
- Independent courier access
- Remote access
- Sensitive-data access
- Emergency access
- Nonstandard access
- Access requiring an exception

---

## 3. Access Classifications

| Classification | Description | Minimum approval |
| --- | --- | --- |
| Standard | Access included in an approved role | Manager and System Owner |
| Additional | Access outside the standard role but within normal job duties | Manager and System Owner |
| Temporary | Access required for a defined period | Manager and System Owner |
| Sensitive | Access to restricted, medical-delivery, financial, or workforce data | Manager, System Owner, and data owner where applicable |
| Privileged | Administrative or elevated technical access | Manager, System Owner, and Security Lead |
| Emergency | Time-sensitive access needed to address a serious operational or security event | Authorized incident or security authority |
| Exceptional | Access that does not meet a normal requirement | Authorized risk owner through `WF-007` |

---

## 4. Required Request Information

Every request must include:

- Request ID
- Request date
- Requester
- User receiving access
- Unique workforce identifier
- Employment or contractor type
- Department
- Manager or sponsor
- System
- Role or entitlement
- Business justification
- Data or function required
- Requested start date
- Expiration date when applicable
- Access classification
- Related ticket or workforce event
- Required training status
- Requested approvers

Incomplete requests must not proceed to provisioning.

---

## 5. Workflow

### Step 1 — Request Submission

The requester submits the standardized access request.

The requester may be:

- The user
- The user’s manager
- HR
- An authorized sponsor
- A System Owner
- An authorized incident leader

### Step 2 — Completeness Validation

The request is reviewed for:

- Verified user identity
- Active workforce or contractor status
- Accountable manager or sponsor
- Complete system and entitlement details
- Business justification
- Required start and expiration dates
- Required training or agreements

### Step 3 — Role Comparison

The requested access is compared with:

- The user’s current role
- The approved role catalog
- Existing entitlements
- The target job responsibilities
- Data-classification requirements

### Step 4 — Least-Privilege Review

The manager and System Owner determine whether:

- The full entitlement is necessary.
- A lower-risk alternative exists.
- Read-only access is sufficient.
- Access can be limited by location, record type, or time.
- Temporary access is more appropriate than standing access.

### Step 5 — Segregation-of-Duties Review

The request is evaluated against defined prohibited combinations.

Potential conflicts include:

- Creating and approving payments
- Creating vendors and releasing vendor payments
- Modifying billing records and approving adjustments
- Provisioning access and independently verifying the same access
- Requesting and approving one’s own privileged access

### Step 6 — Approval Routing

The request follows the approval route associated with its classification.

### Step 7 — Decision

The request may be:

- Approved
- Approved with conditions
- Returned for more information
- Reduced to a lower level of access
- Routed to the exception process
- Rejected

### Step 8 — Provisioning Handoff

Approved requests are sent to `WF-003`.

The provisioning team must receive:

- Final approved role or entitlement
- Approver identities and timestamps
- Start date
- Expiration date
- Conditions
- Monitoring requirements
- Related exception number where applicable

---

## 6. Approval Standards

An approver must confirm that:

- The user has a valid relationship with PLG.
- The requested access supports current responsibilities.
- The request follows least privilege.
- Prohibited conflicts have been resolved.
- Sensitive access has the appropriate authority.
- Temporary access has an expiration date.
- Required training or agreements are complete.
- The approver has authority for the decision.

Approvers may not approve access solely because another user has similar access.

---

## 7. Rejection Criteria

A request must be rejected or returned when:

- The user’s identity cannot be verified.
- The user lacks an accountable manager or sponsor.
- The business justification is missing or inadequate.
- The requested access exceeds job requirements.
- A prohibited conflict cannot be resolved.
- Required training is incomplete.
- Temporary access lacks an expiration date.
- The requester attempts unauthorized self-approval.
- No System Owner exists.
- The request conflicts with policy.
- A required exception has not been approved.

---

## 8. Conditional Approval

An approval may include conditions such as:

- Read-only access
- Limited record scope
- Limited work location
- Limited duration
- Enhanced logging
- Manager review after 30 days
- Required training
- Secondary review
- Compensating monitoring
- Prohibition on specific transactions

Conditions must be visible to the provisioner and reviewer.

---

## 9. Service-Level Targets

| Request type | Target decision time |
| --- | --- |
| Standard access | One business day |
| Additional access | Two business days |
| Sensitive access | Three business days |
| Privileged access | Three business days |
| Emergency access | Immediate risk-based decision |
| Exception request | Based on risk and approval authority |

Operational urgency does not eliminate approval requirements. Emergency access must follow the defined emergency procedure.

---

## 10. Roles and Responsibilities

| Role | Responsibility |
| --- | --- |
| Requester | Submits complete and accurate information |
| User | Complies with access conditions |
| Department Manager | Validates business need |
| System Owner | Approves system-specific permissions |
| Data Owner | Approves access to specially restricted information |
| Finance Manager | Reviews financial SoD conflicts |
| Security Lead | Approves privileged and high-risk access |
| GRC Analyst | Supports exceptions, risk, and evidence |
| IT Service Desk | Provisions only fully approved access |

---

## 11. Evidence Requirements

The minimum evidence package includes:

- Completed request
- Business justification
- Role comparison
- Least-privilege review
- Segregation-of-duties result
- Manager approval
- System Owner approval
- Additional approval where required
- Approval timestamps
- Conditions
- Expiration date
- Exception reference where applicable
- Final decision

---

## 12. Failure Conditions

The workflow fails when:

- Access is provisioned before approval.
- An unauthorized person approves access.
- The requester self-approves restricted access.
- A required SoD review is omitted.
- Access exceeds the approved request.
- Temporary access lacks expiration.
- Approval conditions are not communicated.
- Required evidence is missing.
- A denied request is provisioned.
- An exceptional request bypasses `WF-007`.

---

## 13. Metrics

The workflow supports:

- `MET-001` — Percentage of requests completed within SLA
- `MET-002` — Percentage of requests with complete approvals
- `MET-007` — Percentage of privileged accounts with current approval
- `MET-008` — Evidence completeness
- `MET-009` — Control-test exception rate
