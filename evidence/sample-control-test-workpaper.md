# Sample Control Test Workpaper

> **Fictional assessment notice:** This workpaper uses fictional populations, samples, evidence, and results. It does not represent an independent audit.

## Workpaper Information

| Field | Value |
| --- | --- |
| Test ID | `TEST-003` |
| Assessment | Q3 2026 IAM Control Review |
| Assessment period | July 1 through September 30, 2026 |
| Assessor | Priya Shah, GRC Analyst |
| Reviewer | Elena Morris, Internal Audit Manager |
| Test date | October 8, 2026 |
| Status | Final fictional workpaper |

---

## 1. Control Information

| Field | Value |
| --- | --- |
| Control ID | `CTRL-004` |
| Control title | Timely Access Removal |
| Requirement | `REQ-011` |
| Risk | `IAM-RISK-005` |
| Workflow | `WF-006` |
| Control owner | IT Director |
| Control performers | HR, IT, System Owners, and Facilities |
| Control type | Preventive and corrective |
| Frequency | Event-driven |

---

## 2. Control Objective

PLG removes logical, remote, privileged, vendor, and related physical access by the authorized separation time and verifies completion.

---

## 3. Control Description

HR or an authorized sponsor initiates a verified termination event containing the effective separation time.

IT and applicable System Owners disable accounts, revoke sessions, remove elevated access, and document completion. Facilities disables physical access. A separate reviewer confirms that all known access was addressed and escalates unresolved items.

---

## 4. Test Objective

Determine whether PLG’s fictional termination records demonstrate that:

- Authoritative events initiated access removal.
- Logical access was removed within the defined SLA.
- Dependent systems were addressed.
- Privileged access received priority.
- Physical-access issues were escalated.
- A verifier confirmed completion.
- Evidence supported closure.

---

## 5. Assessment Methods

- [x] Examine
- [x] Interview
- [x] Test
- [ ] Reperform

---

## 6. Population

| Field | Value |
| --- | --- |
| Population | Q3 2026 workforce and contractor separations |
| Population source | HR separation report and contractor termination register |
| Population size | 18 |
| Completeness validation | Reconciled to disabled central accounts and sponsor records |
| Validation result | Pass |

---

## 7. Sample

| Field | Value |
| --- | --- |
| Sample size | 6 |
| Sampling method | Risk-based |
| High-risk items | One involuntary termination, one administrator, two contractors |
| Selection rationale | Included higher-risk events and multiple workforce types |

---

## 8. Test Procedure

1. Obtain the complete separation population.
2. Select a risk-based sample.
3. Compare the authoritative effective time with account-disablement timestamps.
4. Confirm removal from all identified systems.
5. Confirm revocation of privileged and remote access.
6. Review physical-access disposition.
7. Confirm independent verification.
8. Identify exceptions and evaluate escalation.
9. Determine whether evidence supports closure.

---

## 9. Sample Results

| Sample | Event | Logical access result | Physical access result | Verification | Exception |
| ---: | --- | --- | --- | --- | --- |
| 1 | Voluntary employee termination | Pass | Pass | Pass | No |
| 2 | Involuntary administrator termination | Pass | Pass | Pass | No |
| 3 | Contractor expiration | Pass | Pass | Pass | No |
| 4 | Independent courier termination | Pass | Pass after escalation | Pass | Yes |
| 5 | Employee transfer and separation | Pass | Pass | Pass | No |
| 6 | Vendor support termination | Fail | Not applicable | Fail | Yes |

---

## 10. Exceptions

### Exception 1 — Courier Badge Recovery

The electronic badge was disabled shortly after the effective time, but the physical badge was recovered three days later.

The control contained the access risk because the badge could not open the facility. PLG documented and resolved the issue.

**Severity:** Low  
**Finding required:** No

### Exception 2 — Vendor Application Account

A vendor-managed support account remained active for approximately 19 hours after the relationship ended because the central termination workflow did not reach the vendor platform.

**Severity:** High  
**Finding:** `FIND-001`  
**Related POA&M:** `POAM-001`

---

## 11. Exception Rate

```text
2 exceptions ÷ 6 sampled events × 100 = 33.3%
