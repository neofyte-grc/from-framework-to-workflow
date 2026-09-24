# Privileged Access Request Template

## Request Information

| Field | Response |
| --- | --- |
| Request ID | `PAR-###` |
| Request date | |
| Request type | New / Modify / Renew / Emergency |
| Related ticket, change, or incident | |
| Requested start | |
| Requested expiration | |

---

## User Information

| Field | Response |
| --- | --- |
| User | |
| Workforce identifier | |
| Department | |
| Manager | |
| Job role | |
| Employment type | |
| Current standard account | |

---

## Requested Privilege

| Field | Response |
| --- | --- |
| System | |
| Privileged role | |
| Requested permissions | |
| Administrative tasks | |
| Environment | Production / Test / Development / Other |
| Remote administration required? | Yes / No |
| Standing access requested? | Yes / No |
| Separate account supported? | Yes / No |
| Time-bound elevation supported? | Yes / No |

---

## Business Justification

**Describe the tasks requiring privileged access:**

[Enter response]

**Explain why standard access is insufficient:**

[Enter response]

**Explain why time-bound access is or is not practical:**

[Enter response]

---

## Risk and Control Review

| Control question | Response |
| --- | --- |
| Least privilege confirmed? | Yes / No |
| Segregation-of-duties review complete? | Yes / No |
| Separate named account required? | Yes / No |
| MFA required? | Yes / No |
| Enhanced logging required? | Yes / No |
| Session monitoring required? | Yes / No |
| Additional training complete? | Yes / No |
| Emergency procedure applicable? | Yes / No |
| Exception required? | Yes / No |

---

## Monitoring Requirements

- [ ] Authentication events
- [ ] Permission changes
- [ ] Account creation
- [ ] Security-setting changes
- [ ] Restricted-data access
- [ ] Remote administrative activity
- [ ] Command or session logging
- [ ] Post-use review
- [ ] Other requirement listed below

**Additional monitoring:**

[Enter response]

---

## Approvals

| Approver | Decision | Date | Conditions |
| --- | --- | --- | --- |
| Department Manager | Approve / Reject / Return | | |
| System Owner | Approve / Reject / Return | | |
| Information Security Lead | Approve / Reject / Return | | |
| Risk Owner, if required | Approve / Reject / N/A | | |

---

## Provisioning

| Field | Response |
| --- | --- |
| Privileged account | |
| Assigned role | |
| Provisioner | |
| MFA confirmed | Yes / No |
| Logging confirmed | Yes / No |
| Expiration configured | Yes / No |
| Provisioning date | |

---

## Independent Verification

| Verification item | Result |
| --- | --- |
| Correct identity | Pass / Fail |
| Correct role | Pass / Fail |
| Least privilege | Pass / Fail |
| Separate account | Pass / Fail / N/A |
| MFA | Pass / Fail / N/A |
| Logging | Pass / Fail |
| Expiration | Pass / Fail |
| Approval complete | Pass / Fail |

| Field | Response |
| --- | --- |
| Verifier | |
| Verification date | |
| Discrepancy | |
| Resolution | |
| Final status | Active / Returned / Rejected / Revoked |

---

## Revocation

| Field | Response |
| --- | --- |
| Revocation trigger | Expiration / Transfer / Termination / Request / Security event |
| Revocation date and time | |
| Revoked by | |
| Verification completed by | |
| Logs preserved? | Yes / No |
| Final status | Closed / Escalated |
