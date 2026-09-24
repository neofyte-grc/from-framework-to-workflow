# Sample Termination Access Record

> **Fictional evidence notice:** This termination record contains fictional people, accounts, systems, dates, and results.

## Evidence Identification

| Field | Value |
| --- | --- |
| Evidence ID | `EVID-007` |
| Termination record | `TERM-2026-0031` |
| Related workflow | `WF-006` — Termination and Emergency Revocation |
| Related control | `CTRL-004` |
| Related risk | `IAM-RISK-005` |
| Final status | Closed with one resolved escalation |

---

## 1. Termination Event

| Field | Value |
| --- | --- |
| Person | Cameron Reed |
| Workforce identifier | `CTR-0284` |
| Workforce type | Independent courier |
| Sponsor | Andre Wilson, Courier Operations Manager |
| Separation type | Contract termination |
| Effective date and time | September 4, 2026, 5:00 PM |
| Privileged user | No |
| Remote user | Yes |
| Confidential handling | No |
| Authoritative event | `CTR-EVT-2026-0097` |

---

## 2. Known Access

| System or resource | Access |
| --- | --- |
| Microsoft 365 | Courier guest account |
| Dispatch and Delivery Platform | Independent Courier |
| Logistics Platform | Assigned Delivery Viewer |
| Mobile-device access | Approved personal device |
| Physical access | Temporary warehouse badge |
| Vendor systems | None |
| Privileged access | None |

---

## 3. Revocation Actions

| System or action | Completion time | Completed by | Verification | Status |
| --- | --- | --- | --- | --- |
| Microsoft 365 guest access | September 4, 5:01 PM | IT Service Desk | Account disabled | Complete |
| Dispatch Platform | September 4, 5:00 PM | Automated workflow | Account disabled | Complete |
| Logistics Platform | September 4, 5:03 PM | IT Service Desk | Entitlement removed | Complete |
| Active sessions | September 4, 5:04 PM | IT Service Desk | Tokens revoked | Complete |
| Mobile application session | September 4, 5:04 PM | IT Service Desk | Session invalidated | Complete |
| Temporary warehouse badge | September 4, 5:12 PM | Facilities | Badge disabled | Complete |
| Physical badge return | September 7 | Courier Operations | Badge recovered | Complete |

---

## 4. Device and Data Actions

- [x] Mobile application access removed
- [x] Active authentication tokens revoked
- [x] PLG delivery information removed from the application session
- [x] Sponsor reminded of record-handling requirements
- [x] Personal-device corporate profile removal confirmed
- [x] No company-owned device assigned
- [x] No shared credential identified

---

## 5. Escalation

| Field | Value |
| --- | --- |
| Issue | Warehouse badge was not returned at termination |
| Risk | Physical credential could be mistaken for active access |
| Immediate control | Badge disabled electronically at 5:12 PM |
| Owner | Courier Operations Manager |
| Escalated to | Facilities and Security |
| Due date | September 8, 2026 |
| Resolution | Badge recovered September 7 |
| Final risk | Low |

Electronic access was disabled on time. The physical badge remained outstanding but could no longer open the facility.

---

## 6. Verification

| Verification item | Result |
| --- | --- |
| All logical accounts identified | Pass |
| Central and application access removed | Pass |
| Active sessions revoked | Pass |
| Remote access removed | Pass |
| Privileged access removed | Not applicable |
| Physical access disabled | Pass |
| Badge disposition resolved | Pass after escalation |
| Evidence complete | Pass |

| Field | Value |
| --- | --- |
| Verifier | Alicia Green |
| Verification date | September 8, 2026 |
| Final status | Closed |

---

## 7. SLA Evaluation

| Measure | Requirement | Result |
| --- | --- | --- |
| Logical access removal | By effective separation time | Met |
| Active-session revocation | Immediate | Met |
| Physical access disablement | By effective separation time | Completed within 12 minutes |
| Unreturned badge escalation | Same business day | Met |
| Final verification | Within one business day after resolution | Met |

---

## 8. Evidence Conclusion

PLG removed all logical access at or immediately after the effective separation time.

The unreturned physical badge created an operational exception, but Facilities disabled it electronically and the responsible manager recovered it before final closure.
