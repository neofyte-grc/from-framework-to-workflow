# Provisioning and Verification Workflow

## Document Control

| Field | Value |
| --- | --- |
| Organization | Peachtree Logistics Group (fictional) |
| Workflow ID | `WF-003` |
| Workflow owner | IT Director |
| Version | 1.0 |
| Status | Portfolio design artifact |

---

## 1. Purpose

This workflow ensures that approved access is implemented accurately, securely, completely, and within the required timeframe.

It separates:

- Authorization
- Technical provisioning
- Verification
- Exception handling
- Closure

The workflow prevents an approved request from being treated as proof that the correct access was actually implemented.

---

## 2. Scope

This workflow applies to:

- New account creation
- Access additions
- Access modifications
- Role changes
- Temporary access
- Privileged access
- Remote access
- Authentication enrollment
- Group membership changes
- Access removal
- Access restoration following approved leave or suspension

---

## 3. Preconditions

Provisioning may begin only when:

- The user’s identity has been verified.
- Workforce or contractor status is active or approved for future activation.
- The request is complete.
- Required approvals are documented.
- The role or entitlement is clearly identified.
- Segregation-of-duties checks are complete.
- Start and expiration dates are present when required.
- Required training is complete.
- Exception approval is attached when applicable.

Requests that do not meet these requirements must be returned.

---

## 4. Provisioning Workflow

### Step 1 — Controlled Queue Intake

The IT Service Desk receives the approved request through a controlled work queue.

The request is assigned:

- A unique ticket number
- A provisioner
- A target completion date
- A priority
- A system or application
- A verification requirement

### Step 2 — Request Validation

The provisioner confirms:

- User identity
- Workforce identifier
- Manager or sponsor
- System
- Approved role
- Approved entitlements
- Effective date
- Expiration date
- Approval authority
- Applicable conditions

The provisioner must not expand access based on personal judgment or prior examples.

### Step 3 — Account Creation or Modification

The provisioner:

1. Creates or locates the unique user account.
2. Confirms that a duplicate active account does not exist.
3. Assigns only approved roles and groups.
4. Configures authentication requirements.
5. Applies MFA where required and supported.
6. Applies expiration or time limitation.
7. Records the technical action.
8. Captures system-generated evidence.

### Step 4 — Provisioning Self-Check

Before transferring the request for verification, the provisioner confirms:

- The correct user was selected.
- The correct system was modified.
- Assigned access matches the approval.
- No additional group or role was added.
- MFA and authentication settings are correct.
- Start and expiration dates are correct.
- The account status is appropriate.
- Evidence is attached.

### Step 5 — Independent Verification

A designated verifier compares:

- Approved access
- Actual assigned access
- Account status
- Authentication requirements
- Start date
- Expiration date
- Conditions
- Segregation-of-duties result

Independent verification is mandatory for:

- Privileged access
- Financial-system access
- Sensitive medical-delivery information
- High-risk entitlements
- Emergency access
- Access granted through an exception

For standard low-risk access, system-generated validation or risk-based sampling may be used if approved.

### Step 6 — Discrepancy Resolution

If the verifier identifies a discrepancy:

1. The ticket is reopened or held.
2. The discrepancy is classified.
3. Inappropriate access is removed or contained.
4. The provisioner corrects the configuration.
5. The verifier retests the result.
6. Material issues are escalated.
7. The cause is recorded.
8. Repeat failures are referred for corrective action.

### Step 7 — User and Manager Notification

After successful verification:

- The user receives appropriate access instructions.
- The manager receives completion confirmation.
- Temporary-access expiration is communicated.
- Conditions are communicated.
- Sensitive credentials are transmitted through an approved method.

### Step 8 — Closure

The request closes only when:

- Provisioning is complete.
- Verification is complete.
- Discrepancies are resolved.
- Required notifications are sent.
- Evidence is attached.
- The final access state is documented.

---

## 5. Verification Standards

The verifier must determine whether:

- The account belongs to the approved identity.
- The assigned role is correct.
- Actual entitlements match approved entitlements.
- No prohibited access is present.
- Authentication requirements are active.
- Temporary access has the correct expiration.
- Approval conditions were implemented.
- Evidence is sufficient.
- The account was not activated earlier than authorized.

The verifier must not rely solely on the provisioner’s statement that the work was completed.

---

## 6. Discrepancy Classification

| Severity | Example | Required response |
| --- | --- | --- |
| Critical | Unauthorized privileged or administrative access | Remove immediately and notify Security and the CIO |
| High | Sensitive or financial access exceeds approval | Restrict promptly, investigate, and document a finding |
| Moderate | Incorrect standard group or missing approved access | Correct within one business day |
| Low | Documentation error while actual access is correct | Correct the record before closure |

---

## 7. Special Provisioning Requirements

### 7.1 Privileged Access

Privileged access requires:

- A separate named account where supported
- MFA
- Defined scope
- Defined duration
- Enhanced logging
- Security approval
- Independent verification
- Expiration or periodic review

### 7.2 Temporary Access

Temporary access requires:

- Start date
- Expiration date
- Business justification
- Accountable owner
- Removal verification

### 7.3 Contractor and Courier Access

Contractor and courier access requires:

- Named sponsor
- Contract or service relationship
- Limited role
- Expiration date
- Separation from employee access where appropriate
- Confirmation of removal at relationship end

### 7.4 Emergency Access

Emergency access requires:

- Authorized emergency approver
- Defined duration
- Enhanced logging
- Post-use review
- Retrospective documentation
- Verified removal
- Credential rotation when necessary

---

## 8. Roles and Responsibilities

| Role | Responsibility |
| --- | --- |
| Department Manager | Confirms business need and receives completion notice |
| System Owner | Defines approved entitlements |
| IT Service Desk | Executes approved provisioning |
| Designated Verifier | Compares actual access with approval |
| Security Lead | Reviews privileged and high-risk discrepancies |
| GRC Analyst | Tracks evidence quality and recurring failures |
| IT Director | Owns service performance and material escalation |

---

## 9. Evidence Requirements

| Evidence ID | Evidence |
| --- | --- |
| `EVID-002` | Approved access request |
| `EVID-003` | Provisioning record |
| `EVID-004` | Segregation-of-duties result |
| `EVID-005` | Role and entitlement comparison |
| `EVID-006` | Authentication and MFA record |
| `EVID-011` | Independent verification record |

The evidence package should identify:

- User
- System
- Approved role
- Assigned access
- Provisioner
- Provisioning timestamp
- Verifier
- Verification timestamp
- Discrepancies
- Corrective actions
- Final status

---

## 10. Service-Level Targets

| Activity | Target |
| --- | --- |
| Standard provisioning | Within one business day after complete approval |
| Sensitive-access provisioning | Within two business days |
| Privileged-access provisioning | Within two business days after all approvals |
| Standard verification | Before ticket closure |
| High-risk discrepancy containment | Immediate |
| Moderate discrepancy correction | Within one business day |
| Temporary-access removal | By approved expiration time |

---

## 11. Failure Conditions

The workflow fails when:

- Access is provisioned without approval.
- The wrong identity is modified.
- Actual access exceeds approval.
- MFA is omitted where required.
- Temporary access lacks expiration.
- Privileged access is assigned to a standard account without approval.
- Verification is skipped.
- The provisioner serves as the only verifier for high-risk access.
- A discrepancy is closed without correction or risk disposition.
- Evidence is missing or incomplete.
- The request closes before verification.

---

## 12. Metrics

The workflow supports:

- `MET-001` — Provisioning completed within SLA
- `MET-002` — Requests with complete approval
- `MET-007` — Privileged accounts with current approval
- `MET-008` — Evidence completeness
- `MET-009` — Control-test exception rate

Additional operational measures may include:

- Provisioning discrepancy rate
- Average discrepancy-correction time
- Duplicate-account rate
- MFA enrollment rate
- Temporary-access expiration success rate
- Percentage of high-risk access independently verified
