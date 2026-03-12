```mermaid

graph TD

User --> CDN

CDN --> API_Gateway

API_Gateway --> Auth_Service
API_Gateway --> Tenant_Service
API_Gateway --> Billing_Service
API_Gateway --> Analytics_Service

Analytics_Service --> Event_Stream

Event_Stream --> Data_Warehouse

Billing_Service --> Payment_Gateway
