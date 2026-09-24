# Access Review and Remediation Flow

## Purpose

This diagram shows how PLG prepares, performs, remediates, verifies, and closes periodic access reviews.

```mermaid
flowchart TD
    A["Define review scope and due date"] --> B["Generate full account and entitlement population"]
    B --> C["Reconcile with HR, contractor, and role records"]
    C --> D{"Population complete?"}
    D -- No --> E["Resolve missing or unexplained records"]
    E --> C
    D -- Yes --> F["Assign accountable reviewers"]
    F --> G["Provide business context and instructions"]
    G --> H{"Reviewer decision"}
    H -- Certify --> I["Record continued business need"]
    H -- Revoke --> J["Create revocation task"]
    H -- Modify --> K["Create modification task"]
    H -- Escalate --> L["Route to System Owner or Security"]
    H -- Suspend --> M["Restrict access during investigation"]
    J --> N["IT completes remediation"]
    K --> N
    L --> O["Resolve decision or approve exception"]
    M --> O
    N --> P["Independent remediation verification"]
    O --> P
    I --> Q["Quality review"]
    P --> Q
    Q --> R{"Unresolved High or Critical issue?"}
    R -- Yes --> S["Escalate and keep review open"]
    R -- No --> T["System Owner attestation"]
    S --> P
    T --> U["Close review and retain evidence"]
```

---

## Quality Checks

Before closure, PLG confirms:

- The population was complete.
- Every account received a decision.
- Reviewers had sufficient context.
- Remediation was completed.
- Remediation was verified.
- Exceptions received approval.
- No unresolved High or Critical issue remained.
