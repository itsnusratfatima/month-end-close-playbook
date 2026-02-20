# Swimlane – Month-End Close Ownership

```mermaid
flowchart LR
    subgraph Data Systems
        A[Bank Feeds]
        B[ERP]
    end

    subgraph AI Engine
        C[Categorization Model]
        D[Matching Engine]
    end

    subgraph Accountant
        E[Exception Review]
        F[Approval]
    end

    A --> C
    B --> C
    C --> D
    D --> E
    E --> F
```
