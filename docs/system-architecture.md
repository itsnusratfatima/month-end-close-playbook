# 🏗️ Month-End Close System Architecture

```mermaid
flowchart LR
    A[Users - Finance Team] --> B[Frontend - React App]
    B --> C[API Gateway]
    C --> D[Auth Service]
    C --> E[Close Management Service]
    C --> F[Reconciliation Engine]
    C --> G[Journal Entry Service]

    E --> H[(PostgreSQL - Close DB)]
    F --> I[(Transactions DB)]
    G --> J[(Ledger DB)]

    F --> K[Bank APIs]
    F --> L[ERP Integration]

    H --> M[Reporting Service]
    M --> N[BI Dashboard]
