# Framework and Requirements Register

## Document Control

| Field | Value |
| --- | --- |
| Organization | Peachtree Logistics Group (fictional) |
| Project | From Framework to Workflow |
| Document owner | GRC Analyst |
| Version | 1.0 |
| Status | Portfolio design artifact |

---

## 1. Purpose

This register documents the framework requirements used to design PLG’s IAM controls and workflows.

The register provides traceability between:

- Framework source
- PLG requirement
- Access-management risk
- Control objective
- Operational workflow
- Control owner
- Required evidence

The requirement descriptions are portfolio-level interpretations. Authoritative publications remain the normative sources.

---

## 2. Framework Sources

| Framework or publication | Project use |
| --- | --- |
| NIST Cybersecurity Framework 2.0 | Governance, identity management, authentication, access control, monitoring, and improvement outcomes |
| NIST SP 800-53 Release 5.2.0 | Security and privacy control requirements |
| NIST SP 800-53A Release 5.2.0 | Control-assessment procedures and methods |
| NIST SP 800-37 Rev. 2 | Risk-based control implementation, assessment, and monitoring concepts |
| FedRAMP-style documentation practices | Implementation statements, evidence, findings, and POA&M tracking |

---

## 3. Requirements Register

| ID | Source | PLG requirement interpretation | Related risk | Control | Workflow | Owner | Evidence |
| --- | --- | --- | --- | --- | --- | --- | --- |
| `REQ-001` | NIST CSF 2.0 PR.AA | PLG must manage identities and credentials for authorized users, services, and devices throughout their lifecycle | `IAM-RISK-001` | `CTRL-001` | `WF-001` | IT Director | `EVID-001`, `EVID-002` |
| `REQ-002` | AC-1 | PLG must establish, approve, communicate, review, and update access-control policy and procedures | `IAM-RISK-008` | `CTRL-008` | Governance | CIO | Approved policy and review record |
| `REQ-003` | AC-2 | PLG must create, enable, modify, review, disable, and remove accounts according to defined conditions | `IAM-RISK-001` | `CTRL-001` | `WF-001` | IT Director | `EVID-001`, `EVID-003`, `EVID-007` |
| `REQ-004` | AC-3 | PLG systems must enforce approved logical-access authorizations | `IAM-RISK-002` | `CTRL-003` | `WF-003` | System Owner | `EVID-003`, `EVID-011` |
| `REQ-005` | AC-5 | PLG must identify and enforce separation between incompatible duties | `IAM-RISK-003` | `CTRL-002` | `WF-002` | System Owner | `EVID-004` |
| `REQ-006` | AC-6 | PLG must limit users and processes to the minimum access required | `IAM-RISK-002` | `CTRL-002` | `WF-002` | Department Manager | `EVID-005` |
| `REQ-007` | AC-17 | PLG must authorize, monitor, and protect remote access | `IAM-RISK-004` | `CTRL-006` | `WF-005` | Security Lead | Remote-access approval and logs |
| `REQ-008` | IA-2 | PLG must uniquely identify and authenticate organizational users | `IAM-RISK-004` | `CTRL-009` | `WF-003` | Security Lead | Identity and MFA records |
| `REQ-009` | IA-4 | PLG must manage identifiers through creation, assignment, prevention of reuse where appropriate, and disablement | `IAM-RISK-001` | `CTRL-001` | `WF-001` | IT Director | Identifier and account records |
| `REQ-010` | IA-5 | PLG must securely manage authenticators throughout their lifecycle | `IAM-RISK-004` | `CTRL-009` | `WF-003` | Security Lead | Token and authenticator records |
| `REQ-011` | PS-4 | PLG must disable access and recover access devices following termination | `IAM-RISK-005` | `CTRL-004` | `WF-006` | HR and IT | `EVID-007` |
| `REQ-012` | PS-5 | PLG must review and adjust access following transfer or reassignment | `IAM-RISK-006` | `CTRL-004` | `WF-001` | Department Manager | `EVID-008` |
| `REQ-013` | AU-2 | PLG must identify the events that systems are required to log | `IAM-RISK-007` | `CTRL-006` | `WF-005` | Security Lead | Audit-event configuration |
| `REQ-014` | AU-6 | PLG must review and analyze relevant audit records for inappropriate activity | `IAM-RISK-007` | `CTRL-006` | `WF-005` | Security Lead | `EVID-009` |
| `REQ-015` | CA-2 | PLG must assess controls using defined procedures and an appropriate level of independence | `IAM-RISK-008` | `CTRL-010` | Assessment | GRC Analyst | Test workpapers |
| `REQ-016` | CA-5 | PLG must document and track corrective actions for control deficiencies | `IAM-RISK-008` | `CTRL-007` | Remediation | GRC Analyst | `EVID-010` |
| `REQ-017` | CA-7 | PLG must continuously monitor control effectiveness and changes affecting risk | `IAM-RISK-008` | `CTRL-011` | Monitoring | GRC Analyst | Dashboard and review records |
| `REQ-018` | CM-5 | PLG must restrict and monitor access to system-change capabilities | `IAM-RISK-007` | `CTRL-006` | `WF-005` | IT Director | Privileged-role records |
| `REQ-019` | RA-3 | PLG must assess risks associated with access-management weaknesses | All IAM risks | Risk assessment | Risk process | GRC Analyst | Risk register |
| `REQ-020` | PM-10 | PLG must integrate security and privacy into enterprise architecture and operational processes | `IAM-RISK-008` | `CTRL-011` | Governance | CIO | Architecture and governance records |

---

## 4. Requirement-to-Workflow Mapping

| Workflow | Primary requirements |
| --- | --- |
| `WF-001` Joiner-Mover-Leaver | `REQ-001`, `REQ-003`, `REQ-009`, `REQ-011`, `REQ-012` |
| `WF-002` Access Request and Approval | `REQ-004`, `REQ-005`, `REQ-006` |
| `WF-003` Provisioning and Verification | `REQ-004`, `REQ-008`, `REQ-009`, `REQ-010` |
| `WF-004` Periodic Access Review | `REQ-003`, `REQ-006`, `REQ-015`, `REQ-017` |
| `WF-005` Privileged Access | `REQ-005`, `REQ-006`, `REQ-007`, `REQ-013`, `REQ-014`, `REQ-018` |
| `WF-006` Termination and Emergency Revocation | `REQ-003`, `REQ-009`, `REQ-011` |
| `WF-007` Exception and Risk Acceptance | `REQ-016`, `REQ-017`, `REQ-019` |

---

## 5. Assessment Methods

Control assessments may use:

- **Examine:** Review policies, procedures, requests, approvals, logs, reports, tickets, and configurations.
- **Interview:** Discuss responsibilities and practices with control owners, operators, managers, and reviewers.
- **Test:** Perform or observe a control activity using fictional or appropriately protected sample information.

---

## 6. Implementation-Statement Standard

Each control implementation statement should explain:

1. Who performs the control?
2. What activity is performed?
3. When or how often is it performed?
4. Which systems and populations are covered?
5. What information is evaluated?
6. What evidence is generated?
7. What happens when an exception occurs?

---

## 7. Usage Limitation

This register supports a fictional portfolio case study.

It is not:

- A formal control baseline
- A legal interpretation
- A certification statement
- A FedRAMP authorization package
- An independent audit conclusion
- Proof that PLG satisfies any framework
