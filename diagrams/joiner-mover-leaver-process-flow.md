# Joiner-Mover-Leaver Process Flow

## Purpose

This diagram presents the end-to-end identity lifecycle defined by `WF-001`.

```mermaid
flowchart TD
    A["Authoritative workforce event"] --> B{"Event type"}
    B -- Joiner --> C["Validate identity, role, manager, and start date"]
    B -- Mover --> D["Compare current access with target role"]
    B -- Leaver --> E["Identify all logical and physical access"]

    C --> F["Select standard access"]
    F --> G{"Nonstandard or privileged access?"}
    G -- Yes --> H["Complete risk-based approval"]
    G -- No --> I["Provision approved access"]
    H --> I
    I --> J["Verify assigned access"]
    J --> K["Activate at approved time"]

    D --> L["Identify obsolete and new access"]
    L --> M["Evaluate conflicts and overlap"]
    M --> N["Remove obsolete access"]
    N --> O["Provision approved new access"]
    O --> P["Verify final access state"]

    E --> Q["Disable central and application accounts"]
    Q --> R["Revoke sessions, tokens, and privilege"]
    R --> S["Remove physical and vendor access"]
    S --> T["Verify completion"]
    T --> U{"Unresolved item?"}
    U -- Yes --> V["Escalate and track"]
    U -- No --> W["Close lifecycle event"]
    V --> W
```

---

## Control Points

| Lifecycle stage | Primary control |
| --- | --- |
| Event initiation | Verified HR or sponsor event |
| Role selection | Approved role and entitlement catalog |
| Authorization | Manager and System Owner approval |
| Provisioning | Controlled technical work queue |
| Verification | Approved-versus-assigned comparison |
| Transfer | Current-versus-target access analysis |
| Termination | Time-based coordinated revocation |
| Closure | Evidence review and unresolved-item escalation |
