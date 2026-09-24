# Project Overview and Methodology

## Document Control

| Field | Value |
| --- | --- |
| Organization | Peachtree Logistics Group (fictional) |
| Project | From Framework to Workflow |
| Project subtitle | Turning GRC Controls Into Operational Processes |
| Primary domain | Identity and Access Management |
| Document owner | GRC Analyst |
| Version | 1.0 |
| Status | Portfolio design artifact |
| Classification | Public — Fictional portfolio content |
| Review frequency | Annually or following a material project change |

---

## 1. Purpose

This project demonstrates how selected governance, risk, and compliance requirements can be translated into operational identity and access management workflows.

The project moves beyond identifying what an organization should do. It documents how access controls would operate during routine business activities, including:

- Workforce onboarding
- Employee and contractor role changes
- Access requests and approvals
- Account provisioning
- Independent verification
- Periodic access reviews
- Privileged-access management
- Termination and emergency revocation
- Control exceptions
- Evidence collection
- Control testing
- Performance monitoring
- Escalation and remediation

The intended outcome is an IAM operating model that people can execute, managers can own, technical teams can support, and assessors can evaluate.

---

## 2. Project Statement

Peachtree Logistics Group lacks a consistent method for converting access-control requirements into repeatable daily operations.

Access decisions currently depend on informal communications, manual handoffs, inconsistent approvals, and system-specific practices. This creates the possibility that users could receive excessive access, retain permissions after changing roles, or remain active after leaving the organization.

This project creates a governed target-state model that connects:

> Business requirement → Risk → Framework requirement → Control objective → Workflow → Owner → Evidence → Test → Metric → Exception → Escalation → Improvement

---

## 3. Project Objectives

The project will:

1. Establish PLG’s business, workforce, system, and data context.
2. Identify and prioritize access-management risks.
3. Select applicable framework requirements.
4. Convert high-level requirements into specific control objectives.
5. Define accountable owners and decision authorities.
6. Design executable access-management workflows.
7. Establish evidence and audit-trail requirements.
8. Define control assessment procedures.
9. Identify responsible automation opportunities.
10. Create KPIs, KRIs, thresholds, and escalation rules.
11. Track deficiencies through a POA&M-style remediation process.
12. Demonstrate end-to-end control traceability.

---

## 4. Scope

### 4.1 In Scope

The project covers:

- Microsoft 365
- Cloud logistics and freight brokerage platform
- On-premises warehouse management system
- Dispatch and delivery platform
- Billing and accounting system
- Employee, contractor, and independent courier identities
- Standard, temporary, elevated, and privileged access
- Workforce joiner, mover, and leaver events
- Access requests, approvals, provisioning, and verification
- Periodic access reviews
- Access revocation
- Access exceptions and risk acceptance
- Control evidence
- Control testing
- Metrics, escalation, and remediation
- Logical access and related physical-access coordination

### 4.2 Out of Scope

The following activities are outside the project:

- Production deployment or configuration
- Live penetration testing
- Exploitation of systems or accounts
- Independent audit or certification
- Formal authorization
- Legal opinions
- Formal regulatory determinations
- Direct inspection of vendor-controlled environments
- Use of real employee, contractor, customer, patient, or company-sensitive information
- Claims that PLG operates the designed controls in production

---

## 5. Methodology

### Phase 1 — Establish Context

Document PLG’s:

- Business services
- Workforce groups
- Systems and applications
- Information types
- Operating constraints
- Trust boundaries
- Stakeholders
- Dependencies

### Phase 2 — Identify and Assess Risk

Develop access-related risk statements using the following structure:

> Because of a condition or control weakness, a threat or failure event may occur, resulting in an operational, security, privacy, financial, compliance, or reputational impact.

Likelihood and impact are scored separately. The combined score determines inherent and residual risk.

### Phase 3 — Interpret Requirements

Select applicable requirements from:

- NIST Cybersecurity Framework 2.0
- NIST SP 800-53 Release 5.2.0
- NIST SP 800-53A Release 5.2.0
- NIST SP 800-37 Rev. 2
- FedRAMP-style documentation practices

Requirements are paraphrased for the fictional PLG environment. Authoritative publications remain the normative sources.

### Phase 4 — Decompose Controls

Each selected requirement is translated into:

- Control objective
- Control activity
- Trigger
- Inputs
- Responsible actor
- Approver
- Decision rules
- Outputs
- Evidence
- Frequency
- Failure conditions
- Escalation requirements

### Phase 5 — Engineer Workflows

Operational workflows are developed for:

- Joiner-Mover-Leaver events
- Access requests
- Approvals
- Provisioning
- Verification
- Periodic reviews
- Privileged access
- Termination and emergency revocation
- Exceptions and risk acceptance

### Phase 6 — Define Evidence and Testing

For each significant control, the project defines:

- Evidence source
- Evidence owner
- Collection frequency
- Required attributes
- Storage and protection expectations
- Test objective
- Test population
- Sample approach
- Assessment procedure
- Expected result
- Exception handling

### Phase 7 — Measure and Improve

Control performance and risk are monitored through:

- KPIs
- KRIs
- Thresholds
- Control-health ratings
- Escalation rules
- Root-cause analysis
- Corrective actions
- POA&M tracking
- Retesting
- Residual-risk decisions

---

## 6. Identifier Convention

| Artifact | Format | Example |
| --- | --- | --- |
| Requirement | `REQ-###` | `REQ-001` |
| Risk | `IAM-RISK-###` | `IAM-RISK-001` |
| Control objective | `CTRL-###` | `CTRL-001` |
| Workflow | `WF-###` | `WF-001` |
| Role | `ROLE-###` | `ROLE-001` |
| Evidence item | `EVID-###` | `EVID-001` |
| Test procedure | `TEST-###` | `TEST-001` |
| Metric | `MET-###` | `MET-001` |
| Automation requirement | `AUTO-###` | `AUTO-001` |
| Exception | `EXC-###` | `EXC-001` |
| Finding | `FIND-###` | `FIND-001` |
| POA&M item | `POAM-###` | `POAM-001` |

Identifiers support traceability across risks, requirements, controls, workflows, evidence, tests, metrics, findings, and remediation.

---

## 7. Risk-Scoring Method

Likelihood and impact are scored from 1 through 5.

### Likelihood Scale

| Score | Rating | Description |
| ---: | --- | --- |
| 1 | Rare | Event is highly unlikely |
| 2 | Unlikely | Event could occur but is not expected |
| 3 | Possible | Event may occur under normal conditions |
| 4 | Likely | Event is expected to occur periodically |
| 5 | Almost certain | Event is expected to occur frequently |

### Impact Scale

| Score | Rating | Description |
| ---: | --- | --- |
| 1 | Minimal | Limited impact with routine recovery |
| 2 | Minor | Localized disruption or limited exposure |
| 3 | Moderate | Noticeable operational, financial, or security impact |
| 4 | Major | Significant disruption, exposure, or management involvement |
| 5 | Severe | Critical operational, legal, safety, privacy, or reputational impact |

### Risk Calculation

```text
Risk score = Likelihood × Impact
```

### Risk-Rating Bands

| Score | Rating | Required Response |
| ---: | --- | --- |
| 1–4 | Low | Accept or monitor through routine control operation |
| 5–9 | Moderate | Assign treatment, owner, and target date |
| 10–16 | High | Prioritize treatment and report progress to management |
| 17–25 | Critical | Escalate promptly and apply immediate risk-reduction measures |

Residual risk is reassessed after planned controls and compensating measures are considered. Scores support prioritization; they do not replace accountable management judgment.

---

## 8. Evidence Method

Each key control is designed to produce reviewable evidence showing who performed the activity, what was decided, when it occurred, which system or population was affected, and how completion was verified.

Evidence is evaluated using five quality characteristics:

| Characteristic | Question |
| --- | --- |
| Relevance | Does the artifact support the requirement or control being tested? |
| Completeness | Does it cover the required population, fields, approvals, and result? |
| Accuracy | Does it agree with authoritative sources and system records? |
| Timeliness | Was it created and reviewed within the required period? |
| Integrity | Is its source, custody, version, and protection reasonably established? |

Portfolio evidence must use fictional data. A sample artifact demonstrates evidence design, not real-world operating effectiveness.

---

## 9. Traceability Method

The project maintains the following traceability chain:

```text
Framework source → Requirement → Risk → Control → Workflow → Evidence → Test → Metric → Finding → Remediation
```

The chain allows a reviewer to move in both directions: from an external expectation to operational proof, or from a failed activity back to the requirement and risk it affects.

Traceability is documented primarily in:

- `04-framework-and-requirements-register.md`
- `05-control-objective-decomposition.md`
- `15-evidence-and-audit-trail-plan.md`
- `17-control-failure-modes-and-test-plan.md`
- `21-control-assessment-and-traceability-report.md`

---

## 10. Quality-Assurance Method

The project is considered internally consistent when:

1. Identifiers are unique and used consistently.
2. Every key requirement maps to a risk and control response.
3. Every key control has an owner, performer, frequency, evidence, test, and metric.
4. Workflow decision points identify approval, verification, exception, and escalation responsibilities.
5. Policies, standards, templates, and samples support the documented workflows.
6. Sample findings connect to corrective-action records.
7. Relative repository links resolve.
8. Markdown tables and diagrams render without unclosed fences.
9. Fictional artifacts are clearly labeled.
10. Completion claims do not imply certification or operating effectiveness.

---

## 11. Completion Criteria

Project 3 is complete when the repository contains:

- Project context, scope, methodology, and stakeholder accountability
- Framework interpretation and requirements traceability
- Control objectives and an IAM risk register
- Current-state and future-state analysis
- Seven operational IAM workflows
- Evidence, automation, testing, metrics, and monitoring plans
- An implementation roadmap and POA&M
- A control assessment and executive summary
- Policies and standards supporting the target operating model
- Reusable control templates
- Clearly labeled fictional evidence samples
- Renderable process and traceability diagrams
- Executive briefing and portfolio-defense material
- A final repository audit confirming file presence, link integrity, identifier consistency, and Markdown structure

---

## 12. Limitations

This project does not include penetration testing, production configuration review, legal interpretation, independent assurance, or validation of a real organization’s control operation. Vendor environments are not directly assessed. Risk ratings, people, systems, transactions, evidence, test results, findings, and remediation records are illustrative.

---

## 13. Portfolio Disclaimer

Peachtree Logistics Group and all information in this project are fictional. The project is an educational GRC engineering case study and does not represent a production implementation, independent audit, certification, authorization, or legal compliance determination.
