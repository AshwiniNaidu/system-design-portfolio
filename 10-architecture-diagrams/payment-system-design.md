```mermaid

graph TD

Client --> API

API --> Payment_Service
API --> Fraud_Service
API --> Ledger_Service

Payment_Service --> Payment_Gateway

Ledger_Service --> Ledger_DB

Fraud_Service --> Risk_Engine

Risk_Engine --> ML_Model
