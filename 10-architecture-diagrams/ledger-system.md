```mermaid

graph TD

Transaction_API --> Ledger_Service

Ledger_Service --> Validation_Service

Validation_Service --> Ledger_DB

Ledger_Service --> Event_Stream

Event_Stream --> Audit_Service

Audit_Service --> Reporting_DB
