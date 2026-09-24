# Access Request and Approval Flow

## Purpose

This diagram shows how PLG evaluates standard, additional, temporary, privileged, emergency, and exceptional access requests.

```mermaid
flowchart TD
    A["Access request submitted"] --> B{"Request complete?"}
    B -- No --> C["Return for missing information"]
    C --> A
    B -- Yes --> D["Validate identity and workforce status"]
    D --> E["Compare request with approved role"]
    E --> F["Evaluate least privilege"]
    F --> G["Check segregation of duties"]
    G --> H{"Conflict or policy deviation?"}
    H -- Yes --> I{"Can access be reduced or redesigned?"}
    I -- Yes --> J["Modify request"]
    J --> F
    I -- No --> K["Route to exception process"]
    H -- No --> L{"Access classification"}
    L -- Standard --> M["Manager and System Owner approval"]
    L -- Sensitive --> N["Manager, System Owner, and Data Owner approval"]
    L -- Privileged --> O["Manager, System Owner, and Security approval"]
    L -- Emergency --> P["Authorized emergency approval"]
    K --> Q{"Exception approved?"}
    Q -- No --> R["Reject request"]
    Q -- Yes --> S["Record conditions and expiration"]
    M --> T{"Approved?"}
    N --> T
    O --> T
    P --> T
    S --> T
    T -- No --> R
    T -- Yes --> U["Send authorized request to provisioning"]
```

---

## Approval Rules

| Access type | Minimum approval |
| --- | --- |
| Standard | Department Manager and System Owner |
| Sensitive | Manager, System Owner, and applicable Data Owner |
| Privileged | Manager, System Owner, and Security Lead |
| Emergency | Authorized security or incident authority |
| Exceptional | Authorized risk owner based on residual risk |

---

## Required Evidence

The flow should produce:

- Complete request
- Business justification
- Role comparison
- Least-privilege review
- SoD result
- Approvals
- Conditions
- Expiration
- Exception reference where applicable
- Final authorization
