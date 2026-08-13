# System Architecture

```mermaid
flowchart TD
    A[Factory Manager / Staff] --> B[WhatsApp]
    B --> C[n8n Intake]
    C --> D{Classify Update}
    D --> E[Production]
    D --> F[Sales]
    D --> G[Expenses]
    D --> H[Payments]
    D --> I[Deliveries]
    D --> J[Buyers]
    D --> K[Raw Materials]
    D --> L[Farm Feed]
    D --> M[Pig Farm]
    E --> N[Google Sheets Operations Database]
    F --> N
    G --> N
    H --> N
    I --> N
    J --> N
    K --> N
    L --> N
    M --> N
    N --> O[Inventory / Balance Calculations]
    N --> P[Management Reporting]
    O --> Q[WhatsApp Acknowledgement]
    P --> R[Morning / Evening Summary]
```

## Design principle

The automation keeps the staff interface simple: factory staff send operational information through a channel they already use, while the system performs classification, structured storage and calculation behind the scenes.
