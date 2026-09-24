# Portfolio Defense Guide

## From Framework to Workflow

**Prepared for:** Recruiter, hiring-manager, interview, and portfolio-review discussions  
**Prepared by:** Tommy Marshall  
**Project type:** Fictional GRC engineering case study

---

## 1. Two-Minute Project Overview

From Framework to Workflow is a fictional GRC engineering case study for Peachtree Logistics Group, a regional logistics company with approximately 225 personnel.

I focused on identity and access management because PLG’s mix of employees, independent couriers, mobile operations, cloud applications, and on-premises systems creates complex access-lifecycle risks.

The project starts with business risk and framework requirements, then translates them into control objectives, accountable roles, operational workflows, evidence requirements, test procedures, metrics, escalation paths, and remediation.

I designed seven primary workflows covering the joiner-mover-leaver lifecycle, access approval, provisioning and verification, periodic reviews, privileged access, emergency revocation, and exceptions.

The project demonstrates how I apply operations thinking to GRC. A control must work inside the organization. It needs a trigger, an owner, a clear handoff, a completion standard, evidence, and a response when something fails.

---

## 2. Thirty-Second Summary

I designed an IAM operating model that connects NIST-aligned requirements to the way access work would happen inside a fictional logistics company.

The project shows requirement mapping, risk assessment, workflow engineering, ownership, evidence, control testing, KPIs and KRIs, exception handling, and POA&M remediation.

---

## 3. The Business Problem

### Interview response

PLG had access-control requirements but lacked a consistent way to execute them across departments and systems.

Access requests depended on email and institutional knowledge. Transfer and termination processes could miss application accounts. Reviews could lack complete populations or understandable entitlement descriptions. Evidence existed across multiple locations.

I designed the target operating model to address that execution gap.

---

## 4. Why IAM?

### Interview response

IAM sits at the intersection of people, business processes, technology, and risk.

It also aligned well with the PLG scenario because the organization uses employees, contractors, independent couriers, mobile devices, vendor platforms, and time-sensitive operations.

IAM allowed me to demonstrate how governance requirements become recurring operational activities.

---

## 5. Why Use PLG Again?

### Interview response

Using the same fictional company creates continuity across my portfolio.

Project 1 assessed PLG’s broader security and IAM risks. Project 2 examined governance of an AI-assisted logistics use case. Project 3 takes selected access risks and engineers the operational controls.

The shared setting lets each project go deeper without pretending that unrelated one-time exercises represent real consulting engagements.

---

## 6. Frameworks Used

### Primary sources

- NIST Cybersecurity Framework 2.0
- NIST SP 800-53 Release 5.2.0
- NIST SP 800-53A Release 5.2.0
- NIST SP 800-37 Rev. 2
- FedRAMP-style evidence and POA&M practices

### Interview response

I used the frameworks as design references. I did not claim certification or compliance.

I paraphrased selected access, identity, audit, assessment, personnel, and program-management requirements and mapped them to PLG risks and workflows.

---

## 7. Key Design Decision

### Decision

The project focuses on one control domain rather than attempting to engineer every cybersecurity process.

### Interview response

I chose depth over superficial breadth.

The IAM lifecycle gave me enough scope to demonstrate control interpretation, process design, evidence, testing, metrics, exceptions, and remediation while keeping the repository traceable.

---

## 8. Traceability Model

### Model

Business requirement  
Risk  
Framework requirement  
Control objective  
Workflow  
Owner  
Evidence  
Test  
Metric  
Finding  
Remediation

### Interview response

I used consistent identifiers so a reviewer can trace a requirement through the entire control lifecycle.

For example, termination risk maps to `CTRL-004`, `WF-006`, `EVID-007`, `TEST-003`, `MET-003`, `FIND-001`, and `POAM-001`.

---

## 9. Strongest Artifacts

### Recommended interview walkthrough

1. `docs/04-framework-and-requirements-register.md`
2. `docs/05-control-objective-decomposition.md`
3. `docs/08-joiner-mover-leaver-workflow.md`
4. `docs/15-evidence-and-audit-trail-plan.md`
5. `docs/17-control-failure-modes-and-test-plan.md`
6. `docs/21-control-assessment-and-traceability-report.md`
7. `evidence/sample-control-test-workpaper.md`
8. `evidence/sample-poam-record.md`

### Why these matter

Together, these files show that the project moves from requirements through operations, assessment, and remediation.

---

## 10. Example Control Walkthrough

### Termination access removal

**Risk:** A departed person retains access.

**Requirement:** PLG must remove access following termination.

**Control:** HR initiates the event. IT and System Owners remove access. Facilities removes physical access. A separate reviewer verifies completion.

**Evidence:** Workforce event, account inventory, disablement timestamps, session revocation, physical-access record, and verification.

**Test:** Compare separation time with revocation timestamps across a risk-based sample.

**Metric:** Percentage completed within SLA and number of overdue revocations.

**Failure response:** Escalate immediately, document a finding, create a POA&M item, remediate, and retest.

---

## 11. Illustrative Finding

### Interview response

My sample control test identified a vendor-managed account that remained active after the associated third-party relationship ended.

The central account had been disabled, but the termination workflow did not reach the vendor platform.

The root cause involved an incomplete application inventory, weak task routing, and verification that relied too heavily on the central identity report.

The POA&M required application-specific tasks, System Owner confirmation, and reconciliation between terminated identities and vendor accounts.

---

## 12. Automation Approach

### Interview response

I identified automation opportunities but did not claim that I implemented them.

The design includes possible HR-triggered tickets, termination orchestration, review campaigns, expiration alerts, and reconciliation.

I preserved human accountability for business approval, privileged access, risk acceptance, disputed conflicts, and finding closure.

---

## 13. Human Factors

### Interview response

Managers may not understand technical entitlement names. Provisioners may work under time pressure. Warehouse and dispatch teams cannot stop operations for an unclear process.

I addressed those realities through business-friendly role descriptions, clear handoffs, service levels, escalation paths, manual fallback, and evidence created during the workflow.

---

## 14. Connection to Operations Experience

### Interview response

My logistics and operations background taught me how work depends on timing, ownership, handoffs, documentation, exception handling, and escalation.

I applied those same principles here.

An IAM control needs more than policy language. It needs to tell people what starts the process, who acts, which decision they make, how quickly they act, and how the organization proves completion.

---

## 15. Project Limitations

### Interview response

This is a fictional design project.

I did not configure production systems, interview real PLG stakeholders, test live accounts, or perform an independent audit.

A real implementation would require system inventories, stakeholder validation, configuration review, complete account populations, vendor evidence, legal and privacy input, and testing of operating effectiveness.

---

## 16. Claims I Can Make

I can say:

- I designed a fictional IAM governance and control operating model.
- I mapped selected NIST requirements to risks, controls, workflows, evidence, tests, and metrics.
- I developed fictional policies, standards, templates, evidence samples, findings, and remediation records.
- I demonstrated GRC engineering and process-design methods.
- I evaluated how controls could fail and how PLG would detect and correct those failures.

---

## 17. Claims I Should Avoid

I should not say:

- I implemented IAM at a 225-person company.
- I administered Microsoft 365 or PLG systems.
- I completed a formal NIST assessment.
- I performed a FedRAMP audit.
- I certified PLG as compliant.
- I tested real employee accounts.
- I remediated a real security finding.
- The proposed controls operated effectively in production.

---

## 18. Likely Interview Questions

### Why did you choose these specific NIST controls?

I selected controls that directly support the IAM lifecycle, including account management, access enforcement, least privilege, segregation of duties, identity and authentication, personnel termination, audit review, assessment, remediation, and continuous monitoring.

### How did you determine the risk ratings?

I used a five-point likelihood and impact model. The ratings are fictional but internally consistent. I prioritized termination risk because access belonging to a departed user can create severe exposure.

### What makes this GRC engineering?

The project converts requirements into executable workflows with owners, decisions, evidence, testing, metrics, failure handling, and remediation.

### How would you validate the design?

I would interview stakeholders, inspect system capabilities, obtain complete populations, walk through the workflows, test representative transactions, evaluate evidence, and confirm that metrics reflect actual performance.

### What would you implement first?

I would prioritize verified termination, privileged-access inventory, authoritative workforce triggers, role definitions, and complete system ownership.

### What was the hardest design problem?

Balancing timely logistics operations with consistent access governance. The controls need to prevent unauthorized access without creating avoidable delivery disruption.

### How did you address third-party access?

I required sponsors, limited roles, expiration, periodic review, lifecycle events, and application-level revocation confirmation.

### Why did you include sample evidence?

Evidence shows whether the workflow can support assessment. The samples demonstrate the records a functioning control should produce.

---

## 19. Five-Minute Demonstration Path

1. Open the README and explain the business problem.
2. Show the requirements register.
3. Trace one requirement into the control catalog.
4. Open the related workflow.
5. Show the sample evidence.
6. Show the test workpaper.
7. Show the finding and POA&M record.
8. Close with the control-health metrics.

This walkthrough demonstrates the full GRC engineering lifecycle without reviewing every repository file.

---

## 20. Closing Statement

This project reflects the kind of GRC work I want to perform: translating security requirements into processes that people can execute, organizations can measure, and assessors can verify.

My operations background helps me evaluate whether a control can function under real deadlines, system limitations, staffing constraints, and operational pressure.

---

## Portfolio Disclaimer

PLG and all information in this guide are fictional. The project demonstrates portfolio methods and developing expertise. It does not represent a production implementation, independent audit, certification, authorization, or legal compliance determination.
