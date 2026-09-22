# Business Problem and Control Scope

## Document Control

| Field | Value |
| --- | --- |
| Organization | Peachtree Logistics Group (fictional) |
| Project | From Framework to Workflow |
| Document owner | GRC Analyst |
| Version | 1.0 |
| Status | Portfolio design artifact |

---

## 1. Business Problem

PLG lacks a consistent, documented, and measurable process for translating identity and access management requirements into daily operational activities.

Access requests, approvals, provisioning, modifications, reviews, and revocations are handled differently across departments and systems. Many activities rely on email, spreadsheets, verbal communication, and the institutional knowledge of individual employees.

As a result, PLG cannot consistently demonstrate that:

- Every account belongs to an authorized person.
- Access reflects a current business need.
- Users receive only the permissions required for their roles.
- Conflicting duties are identified.
- Privileged access receives enhanced oversight.
- Role changes result in timely access adjustments.
- Departed personnel lose access promptly.
- Temporary access expires as intended.
- Access reviews use complete and accurate populations.
- Exceptions receive formal approval and expiration dates.
- Evidence is sufficient to prove control performance.

---

## 2. Problem Statement

> Because PLG relies on inconsistent and partially manual access-management practices, unauthorized, excessive, outdated, or untraceable access may remain active, potentially resulting in data exposure, fraud, privacy violations, operational disruption, weak accountability, or an inability to demonstrate control effectiveness.

---

## 3. Business Drivers

The IAM improvement effort is driven by:

- Growth in workforce and system use
- Dependence on cloud and vendor-managed applications
- Use of independent couriers
- Handling of sensitive customer and delivery information
- Medical-delivery workflows
- Increased remote and mobile access
- Need for stronger accountability
- Need for reliable audit evidence
- Need to reduce manual processing delays
- Need for measurable control performance

---

## 4. Control Scope

### 4.1 Workforce Events

The project covers:

- New employees
- New contractors
- Independent couriers
- Temporary personnel
- Role or department transfers
- Leave-of-absence events
- Contract expiration
- Voluntary termination
- Involuntary termination
- Emergency revocation

### 4.2 Access Types

The project covers:

- Standard role-based access
- Temporary access
- Elevated access
- Privileged administrative access
- Emergency access
- Third-party access
- Physical-access coordination
- Service and shared accounts where applicable

### 4.3 Control Activities

The project covers:

- Identity validation
- Access request submission
- Business justification
- Role selection
- Manager approval
- System-owner approval
- Segregation-of-duties review
- Risk-based approval
- Provisioning
- Independent verification
- Periodic access review
- Revocation
- Exception approval
- Evidence collection
- Control testing
- Metric reporting
- Escalation
- Remediation
- Retesting

---

## 5. Systems in Scope

| System | Primary use | Access concern |
| --- | --- | --- |
| Microsoft 365 | Email, collaboration, and records | Oversharing, account compromise, and accumulated permissions |
| Logistics and freight platform | Orders, shipments, customers, and carriers | Unauthorized record access or modification |
| Warehouse management system | Inventory and warehouse operations | Shared access and excessive warehouse permissions |
| Dispatch and delivery platform | Assignment, route, location, and delivery information | Mobile access and contractor separation |
| Billing and accounting system | Invoices, payments, and financial records | Fraud and segregation-of-duties conflicts |
| Physical-access systems | Badges, keys, and facility entry | Failure to coordinate logical and physical revocation |

---

## 6. Information in Scope

The control environment includes access to:

- Workforce records
- Customer information
- Delivery records
- Medical-delivery details
- PHI/ePHI indicators
- Payment information
- Billing records
- Contracts
- Vendor information
- Operational reports
- Authentication records
- Authorization records
- Audit logs
- Control evidence

---

## 7. Key Control Questions

The project will answer:

1. What event initiates each access process?
2. Which source establishes a person’s status?
3. Who validates the business need?
4. Who approves access?
5. How is least privilege evaluated?
6. How are conflicting duties identified?
7. Who provisions the access?
8. Who verifies the result?
9. How quickly must the activity occur?
10. What evidence proves completion?
11. What happens when the process fails?
12. Who may approve an exception?
13. How is residual risk accepted?
14. How is performance measured?
15. How are findings remediated and retested?

---

## 8. Target Outcomes

The target operating model should ensure that:

- Each account is connected to a verified identity.
- Each identity has an accountable manager or sponsor.
- Access has a documented business purpose.
- Approvals occur before provisioning.
- Least privilege guides entitlement decisions.
- Segregation-of-duties conflicts are identified.
- Temporary access has an expiration date.
- Privileged access receives enhanced controls.
- Workforce changes trigger access changes.
- Terminations trigger timely revocation.
- Access reviews result in verified remediation.
- Exceptions are documented and time-bound.
- Evidence is complete and protected.
- Control failures are escalated.
- Corrective actions are tracked to closure.

---

## 9. Success Measures

Project success will be evaluated using measures such as:

- Percentage of access requests completed within SLA
- Percentage of access requests with complete approvals
- Percentage of provisioned access matching approved access
- Average termination-to-disablement time
- Percentage of access reviews completed on time
- Number of overdue revocations
- Percentage of privileged accounts with current approval
- Number of expired exceptions
- Evidence completeness rate
- Control-test exception rate
- Percentage of findings remediated by the target date

---

## 10. Out-of-Scope Activities

The project does not include:

- Production deployment
- Live account provisioning
- Live account disablement
- Real employee or contractor records
- Penetration testing
- Password cracking
- Adversarial exploitation
- Vendor certification
- Legal analysis
- Independent audit
- Formal authorization
- Regulatory certification
- Claims of actual control operating effectiveness

---

## 11. Scope Limitations

The project is based on fictional assumptions and illustrative evidence.

A real PLG implementation would require:

- Stakeholder interviews
- Application-owner validation
- Technical configuration review
- Complete user and entitlement populations
- Vendor documentation
- Legal and privacy review
- Production testing
- Independent assessment
- Approved retention requirements
- Validated system capabilities

---

## 12. Conclusion

This project focuses on the operational gap between written requirements and daily work.

Its purpose is to show how PLG could transform access-control expectations into workflows that have:

- Defined triggers
- Clear ownership
- Risk-based decisions
- Repeatable actions
- Reliable evidence
- Measurable outcomes
- Escalation paths
- Corrective-action mechanisms
