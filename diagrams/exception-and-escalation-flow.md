# Exception and Escalation Flow

## Purpose

This diagram shows how PLG evaluates a control deviation, determines approval authority, monitors the exception, and closes or escalates it.

```mermaid
flowchart TD
    A["Requirement cannot be met"] --> B["Submit exception request"]
    B --> C{"Request complete?"}
    C -- No --> D["Return for required information"]
    D --> B
    C -- Yes --> E["Assess inherent risk"]
    E --> F["Evaluate safer alternatives"]
    F --> G{"Alternative meets business need?"}
    G -- Yes --> H["Use compliant alternative"]
    G -- No --> I["Define compensating controls"]
    I --> J["Calculate residual risk"]
    J --> K{"Approval authority"}
    K -- Low or Moderate --> L["System Owner decision"]
    K -- High --> M["CIO and Security decision"]
    K -- Critical --> N["Executive risk decision"]
    L --> O{"Approved?"}
    M --> O
    N --> O
    O -- No --> P["Reject and prevent activity"]
    O -- Yes --> Q["Implement conditions and monitoring"]
    Q --> R["Track corrective action and expiration"]
    R --> S{"Requirement resolved before expiration?"}
    S -- Yes --> T["Validate evidence and close"]
    S -- No --> U{"Renewal justified?"}
    U -- No --> V["Remove access or stop activity"]
    U -- Yes --> W["Complete new risk assessment"]
    W --> K
```

---

## Escalation Levels

| Level | Example | Authority |
| --- | --- | --- |
| 1 | Isolated Low-impact process issue | Process Owner |
| 2 | Repeat Moderate issue or SLA breach | Manager and GRC |
| 3 | High-risk access or material control failure | CIO and Security Lead |
| 4 | Critical exposure or suspected misuse | COO and incident leadership |

---

## Prohibited Outcomes

The process must not allow:

- Open-ended exceptions
- Automatic renewal
- Requester self-approval
- Missing compensating controls
- Continued activity after expiration
- Closure without evidence
