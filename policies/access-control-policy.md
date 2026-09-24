# Access Control Policy

## Document Control

| Field | Value |
| --- | --- |
| Organization | Peachtree Logistics Group (fictional) |
| Policy owner | CIO / IT Director |
| Policy coordinator | GRC Analyst |
| Approval authority | Chief Operating Officer |
| Version | 1.0 |
| Status | Portfolio design artifact |
| Effective date | Upon fictional approval |
| Review frequency | Annually and following material change |
| Classification | Public — Fictional portfolio content |

---

## 1. Purpose

This policy establishes PLG’s requirements for granting, modifying, reviewing, monitoring, and removing logical and related physical access.

The policy is intended to ensure that access is:

- Connected to a verified identity
- Supported by a legitimate business need
- Authorized by accountable personnel
- Limited according to least privilege
- Appropriate for current responsibilities
- Protected through suitable authentication
- Reviewed periodically
- Removed when no longer required
- Supported by reliable evidence

---

## 2. Scope

This policy applies to:

- Employees
- Contractors
- Independent couriers
- Temporary workers
- Interns
- Vendors
- Service providers
- Third parties
- Information systems
- Cloud platforms
- On-premises systems
- Mobile applications
- Remote-access services
- Physical-access systems
- Service and shared accounts
- Privileged and emergency accounts

The policy covers access to PLG information, systems, applications, devices, facilities, services, and technology resources.

---

## 3. Policy Objectives

PLG will:

1. Grant access only to authorized identities.
2. Base access on current business responsibilities.
3. Apply least privilege.
4. Enforce segregation of duties.
5. Require approval before provisioning.
6. Use unique user accounts where technically possible.
7. protect authenticators.
8. Apply stronger controls to privileged access.
9. Review access periodically.
10. Remove access promptly following termination or role change.
11. Govern temporary and emergency access.
12. Document and approve exceptions.
13. Monitor control performance.
14. Retain appropriate evidence.

---

## 4. Roles and Responsibilities

| Role | Responsibility |
| --- | --- |
| COO | Approves policy and resolves Critical residual-risk decisions |
| CIO / IT Director | Owns access-control operations and technical implementation |
| GRC Analyst | Coordinates requirements, risk, evidence, testing, and reporting |
| HR Manager | Provides authoritative employee lifecycle information |
| Department Manager | Validates business need and reviews user access |
| System Owner | Defines roles, approves entitlements, and certifies access |
| Information Security Lead | Governs privileged access, authentication, and monitoring |
| IT Service Desk | Provisions, modifies, and removes approved access |
| Contractor Sponsor | Owns contractor, courier, and third-party access need |
| Facilities | Manages badges, keys, and physical-access credentials |
| Users | Protect credentials and use access only for authorized purposes |

---

## 5. Identity Requirements

Every user must:

- Have a verified identity.
- Have an active relationship with PLG.
- Have an accountable manager or sponsor.
- Use a unique identifier where supported.
- Use only accounts assigned to them.
- Protect passwords, tokens, keys, and authentication devices.
- Report suspected compromise promptly.

Anonymous or untraceable access is prohibited unless specifically approved for a documented technical or business purpose.

---

## 6. Access Authorization

Access must be:

- Requested through an approved process.
- Supported by a documented business need.
- Compared with an approved role or entitlement.
- Approved before provisioning.
- Limited to the minimum necessary permissions.
- Assigned an expiration date when temporary.
- Evaluated for segregation-of-duties conflicts.
- Supported by an approved exception when a requirement cannot be met.

Approval must come from personnel with authority over the user, system, data, and risk involved.

---

## 7. Least Privilege

PLG will grant only the access necessary to perform approved responsibilities.

Access decisions should consider:

- Whether read-only access is sufficient
- Whether access can be limited by function
- Whether access can be limited by location
- Whether access can be limited by record type
- Whether temporary access is sufficient
- Whether a lower-risk role can meet the need
- Whether access creates conflicting duties

Access must not be granted solely because another person has similar access.

---

## 8. Segregation of Duties

PLG will identify and restrict incompatible responsibilities.

At minimum:

- Users may not approve their own elevated access.
- Users may not certify their own access.
- Provisioners may not serve as the sole verifier for high-risk access.
- Control operators should not independently assess controls they operate.
- Risk acceptance must be approved by an authorized risk owner.
- Financial-system roles must be reviewed for incompatible activities.
- Emergency access must receive retrospective review.

Unresolved conflicts must be denied or handled through the approved exception process.

---

## 9. Authentication

PLG will:

- Use unique user accounts where supported.
- Require passwords or other authenticators that meet approved standards.
- Use MFA for privileged, remote, and other designated high-risk access.
- Protect authentication secrets from unauthorized disclosure.
- Revoke or replace compromised authenticators.
- Disable authenticators when access is terminated.
- Restrict shared credentials.
- Review authentication controls following material system changes.

Users must not share passwords, authentication tokens, or MFA devices.

---

## 10. Privileged Access

Privileged access must:

- Have documented business justification.
- Receive manager, System Owner, and Security approval.
- Use a separate named account where supported.
- Use MFA where supported.
- Be limited in scope and duration.
- Be logged and monitored.
- Receive periodic review.
- Be removed when no longer required.

Standing privilege must be minimized. Time-bound or just-in-time elevation should be used where technically and operationally practical.

---

## 11. Temporary and Emergency Access

Temporary access must:

- Have a defined purpose.
- Have an accountable owner.
- Have a start date.
- Have an expiration date.
- Be reviewed and removed at expiration.

Emergency access must:

- Be approved by authorized personnel.
- Be limited to the emergency.
- Be logged.
- Receive prompt post-use review.
- Be removed after use.
- Have credentials rotated where required.

Emergency access must not become a substitute for standard access processes.

---

## 12. Contractor and Third-Party Access

Contractors, couriers, vendors, and other third parties must:

- Have a named PLG sponsor.
- Have a documented business relationship.
- Receive access limited to their assigned services.
- Have a defined start and end date.
- Use separate identity classifications where supported.
- Receive periodic review.
- Lose access when the relationship ends.
- Comply with applicable PLG security requirements.

Third-party access must not be treated as permanent employee access.

---

## 13. Joiner, Mover, and Leaver Requirements

### Joiners

Access must be based on an approved workforce event, current role, manager validation, and authorized entitlements.

### Movers

Role changes must trigger a comparison between current and required access. Obsolete access must be removed before or with the activation of new access.

### Leavers

Access must be removed by the effective separation time. Involuntary, emergency, and security-related separations require coordinated immediate action.

Logical and physical access removal must be coordinated.

---

## 14. Periodic Access Reviews

PLG must periodically review:

- Standard accounts
- Privileged accounts
- Contractor accounts
- Service accounts
- Shared accounts
- Remote-access permissions
- Sensitive-data access
- Physical-access credentials

Reviewers must have sufficient information to select:

- Certify
- Revoke
- Modify
- Escalate
- Suspend

Required remediation must be completed and verified.

---

## 15. Service and Shared Accounts

Service accounts must have:

- A documented purpose
- An accountable owner
- Minimum necessary permissions
- Protected credentials
- Monitoring
- Review frequency
- Decommissioning criteria

Shared accounts are prohibited unless a technical limitation requires them and an approved exception provides individual accountability, monitoring, credential rotation, and remediation.

---

## 16. Logging and Monitoring

PLG will log and monitor access-related events based on risk.

Relevant events may include:

- Account creation
- Account modification
- Account disablement
- Authentication failure
- Privileged access
- Permission changes
- Emergency access
- Security-setting changes
- Attempts to bypass restrictions

Material anomalies must be investigated and escalated.

---

## 17. Exceptions

Exceptions must:

- Identify the unmet requirement.
- Document business justification.
- Assess risk.
- Identify compensating controls.
- Name an accountable owner.
- Receive authorized approval.
- Have an expiration date.
- Be monitored.
- Be closed or reassessed before expiration.

Open-ended and self-approved exceptions are prohibited.

---

## 18. Evidence and Records

Control activities must produce evidence sufficient to demonstrate:

- Request
- Approval
- Provisioning
- Verification
- Review
- Revocation
- Exception
- Monitoring
- Remediation

Evidence must be protected, retrievable, attributable, and retained according to approved requirements.

---

## 19. Violations

Violations may result in:

- Access restriction
- Access revocation
- Corrective action
- Disciplinary action
- Contractual action
- Incident-response activity
- Legal referral where appropriate

Suspected violations must be reported to the Information Security Lead, the CIO, HR, or another authorized reporting channel.

---

## 20. Policy Review

This policy must be reviewed:

- At least annually
- Following a material system change
- Following a significant IAM incident
- Following a material control failure
- Following a framework or legal change
- When business operations materially change

Review evidence must document the reviewer, date, changes, approval, and communication.

---

## 21. Related Documents

- Identity Lifecycle Management Standard
- Access Review Standard
- Access Exception and Escalation Standard
- Joiner-Mover-Leaver Workflow
- Privileged Access Management Workflow
- Termination and Emergency Revocation Workflow
- Evidence and Audit Trail Plan
- Continuous Monitoring and Escalation Plan

---

## 22. Disclaimer

PLG and the policy described here are fictional. This policy is an educational portfolio artifact and does not represent legal advice, certification, authorization, or a production implementation.
