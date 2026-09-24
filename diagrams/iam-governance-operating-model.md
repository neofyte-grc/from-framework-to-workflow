# IAM Governance Operating Model

## Purpose

This diagram shows how PLG assigns IAM governance, operational execution, assurance, and escalation responsibilities.

```mermaid
flowchart TD
    A["COO<br/>Executive risk authority"] --> B["CIO / IT Director<br/>IAM accountable owner"]
    A --> C["Executive risk decisions"]
    B --> D["IAM Governance Group"]
    D --> E["HR<br/>Workforce events"]
    D --> F["Managers and System Owners<br/>Business approval"]
    D --> G["IT and Security<br/>Provisioning and monitoring"]
    D --> H["GRC<br/>Risk, evidence, and reporting"]
    E --> I["Joiner-Mover-Leaver workflows"]
    F --> I
    G --> I
    H --> J["Control assessment"]
    I --> K["Control evidence"]
    K --> J
    J --> L{"Material deficiency?"}
    L -- No --> M["Routine monitoring"]
    L -- Yes --> N["Finding and POA&M"]
    N --> B
    N --> C
```

---

## Role Summary

| Governance layer | Roles | Primary responsibility |
| --- | --- | --- |
| Executive | COO | Critical risk and resource decisions |
| Accountable owner | CIO / IT Director | IAM program performance |
| Business authority | Managers and System Owners | Business need and entitlement approval |
| Authoritative source | HR and Contractor Sponsors | Workforce and relationship status |
| Control operation | IT, Security, and Facilities | Provisioning, monitoring, and removal |
| Oversight | GRC Analyst | Risk, evidence, metrics, exceptions, and remediation |
| Assurance | Assessor or Internal Audit | Independent evaluation |

---

## Decision Principle

The model separates:

- Business approval
- Technical implementation
- Verification
- Risk acceptance
- Independent assessment

One individual should not control every stage of a High-risk access decision.
