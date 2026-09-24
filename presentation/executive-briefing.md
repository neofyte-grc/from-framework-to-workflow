# Executive Briefing

## From Framework to Workflow

**Organization:** Peachtree Logistics Group (fictional)  
**Prepared by:** Tommy Marshall  
**Portfolio focus:** GRC Engineering and IAM Control Implementation  
**Recommended length:** 12 slides  
**Audience:** Executive leadership, CIO, Security, GRC, HR, and operational management

---

## Slide 1 — From Framework to Workflow

### Turning GRC Controls Into Operational Processes

**Primary message:** PLG needs a consistent operating model that converts access requirements into owned, measurable, and evidence-producing work.

**Presenter note:** This fictional case study focuses on the gap between written access-control expectations and the way access decisions occur during daily operations.

---

## Slide 2 — PLG Operating Context

### Slide content

- Regional logistics company headquartered in Atlanta
- Approximately 225 personnel
- Warehousing, last-mile delivery, medical courier, and freight brokerage
- Employees, contractors, and independent couriers
- Mixed cloud and on-premises environment
- Time-sensitive operations across office, warehouse, dispatch, and mobile settings

### Systems in scope

- Microsoft 365
- Logistics and freight platform
- Warehouse management system
- Dispatch and delivery platform
- Billing and accounting system

**Presenter note:** PLG needs access controls that protect sensitive information without disrupting delivery operations.

---

## Slide 3 — IAM Business Problem

### Slide content

PLG’s IAM activities depend on:

- Email requests
- Manual handoffs
- Inconsistent approvals
- System-specific knowledge
- Ad hoc access reviews
- Scattered evidence

### Resulting exposure

- Excessive access
- Delayed termination
- Privilege accumulation
- Contractor-access gaps
- Incomplete evidence
- Unclear accountability

**Presenter note:** The business problem involves process consistency and accountability across systems and departments.

---

## Slide 4 — Priority Risks

| Priority | Risk | Inherent rating |
| ---: | --- | --- |
| 1 | Departed personnel retain access | Critical |
| 2 | Users receive excessive permissions | High |
| 3 | Transfers retain prior-role access | High |
| 4 | Privileged access lacks enhanced control | High |
| 5 | Contractor access lacks sponsorship or expiration | High |
| 6 | Findings remain unresolved | High |

**Presenter note:** Delayed access removal received the highest priority because a former user could retain access after PLG’s business relationship ends.

---

## Slide 5 — Requirements-to-Workflow Model

### Slide content

1. Business requirement
2. Risk
3. Framework requirement
4. Control objective
5. Operational workflow
6. Accountable owner
7. Evidence
8. Assessment
9. Metric
10. Remediation

### Key point

Every control must define who performs the work, what triggers it, which evidence proves completion, and what happens when it fails.

**Presenter note:** This traceability model connects governance documentation to operational execution and improvement.

---

## Slide 6 — Target IAM Workflows

| Workflow | Outcome |
| --- | --- |
| Joiner-Mover-Leaver | Access follows the workforce lifecycle |
| Access Request and Approval | Access has documented need and authorization |
| Provisioning and Verification | Assigned access matches approved access |
| Periodic Access Review | Obsolete access is identified and removed |
| Privileged Access | Elevated access receives stronger control |
| Termination and Emergency Revocation | Access is removed rapidly and completely |
| Exception and Risk Acceptance | Deviations remain documented and temporary |

**Presenter note:** The workflows cover the complete lifecycle rather than treating provisioning as the entire IAM process.

---

## Slide 7 — Accountability Model

### Executive authority

- COO approves policy and Critical risk decisions.

### Program accountability

- CIO owns IAM program performance.

### Business authority

- Managers validate business need.
- System Owners approve entitlements.

### Control operation

- HR initiates workforce events.
- IT provisions and removes access.
- Security governs privileged access.

### Oversight

- GRC manages risk, evidence, testing, metrics, exceptions, and remediation.

**Presenter note:** The model separates request, approval, implementation, verification, and assessment.

---

## Slide 8 — Evidence and Assessment

### Evidence produced by the workflows

- Workforce event
- Approved access request
- Provisioning record
- Role comparison
- SoD result
- Verification record
- Access-review package
- Revocation record
- Exception record
- POA&M record

### Assessment methods

- Examine documentation and system records
- Interview control owners and performers
- Test transactions and populations

**Presenter note:** Evidence is part of the process design. It should not require reconstruction only when an audit begins.

---

## Slide 9 — Metrics and Control Health

| Metric | Target |
| --- | ---: |
| Requests completed within SLA | At least 95% |
| Complete approval before provisioning | 100% |
| Terminations completed within SLA | 100% |
| Access reviews completed on time | At least 98% |
| Active expired exceptions | 0 |
| Privileged accounts with current approval | 100% |
| Evidence completeness | At least 98% |

### Control health

- Green: target met and no material unresolved issue
- Amber: warning threshold or remediation at risk
- Red: Critical threshold or unreliable control performance

**Presenter note:** One unresolved Critical account can outweigh an otherwise high completion rate.

---

## Slide 10 — Illustrative Assessment Finding

### Finding

A vendor-managed support account remained active for 19 hours after the relationship ended.

### Root cause

- Incomplete application inventory
- No vendor-specific revocation task
- Central account report treated as full confirmation

### Corrective action

- Maintain the complete application inventory
- Generate System Owner revocation tasks
- Require dependent-system confirmation
- Reconcile terminated identities with vendor accounts

**Presenter note:** This finding shows why central account disablement does not prove complete removal across the access boundary.

---

## Slide 11 — Implementation Roadmap

### Phase 1 — Govern

Approve ownership, policy, risk authority, and role standards.

### Phase 2 — Standardize

Implement the seven core workflows.

### Phase 3 — Evidence and Assess

Create the evidence catalog, testing process, and findings workflow.

### Phase 4 — Automate

Integrate workforce events, expiration, reconciliation, and escalation.

### Phase 5 — Monitor and Improve

Use metrics, control health, POA&M tracking, and reassessment.

**Presenter note:** PLG should establish ownership and stable processes before expanding automation.

---

## Slide 12 — Leadership Decisions

### Decisions requested

- Approve IAM ownership and decision authority.
- Prioritize termination and privileged-access controls.
- Require System Owner participation.
- Support role and entitlement development.
- Approve evidence and monitoring expectations.
- Fund priority remediation.
- Define residual-risk authority.

### Final message

The proposed model gives PLG a practical method for converting access requirements into repeatable work, reliable evidence, measurable performance, and accountable risk decisions.

---

## Presentation Disclaimer

PLG and all information in this presentation are fictional. The presentation documents a portfolio design exercise and does not represent a production implementation, independent audit, certification, authorization, or compliance determination.
